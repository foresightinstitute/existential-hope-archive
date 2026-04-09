# Hyper-Entity Extraction Pipeline: Prompts

This document records the full LLM-powered pipeline used to extract, deduplicate, research, score, curate, and write up hyper-entities from the Existential Hope archive. Each stage lists the model, temperature, system prompt, user prompt(s), and any output schemas. Variable placeholders use `{variable_name}` syntax.

## Pipeline Overview

```
Extraction  -->  Deduplication  -->  Web Research  -->  Scoring  -->  Curation  -->  Report Generation
(Sonnet)         (Haiku)             (Haiku+web)       (Haiku)      (Python)       (Sonnet)
```

---

## 1. Extraction

**Purpose:** Extract hyper-entity candidates from source documents (podcast transcripts, world-gallery submissions, research reports).

**Model:** `claude-sonnet-4-6`, temperature `0`

**System prompt:**

```
You are an expert at identifying concrete, specific technological or institutional proposals in text. You return valid JSON only.
```

### Entity output schema

All three prompt variants share this schema instruction appended to the end:

```
Return a JSON array of extracted entities. Each entity must have these fields:
{
  "name": "string - use the speaker's name for it if given, or the most specific name from the text",
  "source_quote": "string - VERBATIM quote from the source (1-3 sentences)",
  "source_quote_context": "string - brief note on where in the doc the quote appears, e.g. 'Discussion of nuclear energy around timestamp 15:23' or 'Section on governance mechanisms'",
  "speaker": "string or null - who proposed/discussed this",
  "one_liner": "string - one sentence explaining what this is",
  "mechanism": "string - 2-4 sentences on how it works",
  "exists_today": "string - what partial implementations exist already"
}

If nothing qualifies, return an empty JSON array: []
```

### Prompt variant 1: Short (world-gallery entries)

```
This is a brief speculative world sketch. Extract 0-2 SPECIFIC technologies, institutions, or systems described that someone could actually build or fund. If nothing is concrete enough to have a mechanism of action, return an empty list. Do NOT extract vague concepts or genre labels.

{ENTITY_SCHEMA_INSTRUCTION}
```

### Prompt variant 2: Podcast (transcripts)

```
Extract SPECIFIC proposals, systems, architectures, or technologies discussed by the speaker that are:
1. NAMED or CONCRETE enough that someone could write a spec for it
2. NOT YET BUILT at scale (may have prototypes or research)
3. DISCUSSED SERIOUSLY with some mechanism explained (not throwaway mentions)

ANTI-PATTERNS (do NOT extract these):
- Generic field descriptions ('AI-enhanced governance')
- Vague compound nouns you invented
- Already widely deployed technology
- Abstract values or principles

Most transcripts yield 0-3 candidates. If nothing qualifies, return an empty list.

{ENTITY_SCHEMA_INSTRUCTION}
```

### Prompt variant 3: Report (research reports, split by section)

```
This is a section from a research report titled '{section_heading}'. Extract only proposals that are NOVEL and have SPECIFIC implementation mechanisms described in this section.

Strict criteria -- an entity must have ALL of:
1. A specific NAME or label given by the authors
2. A concrete MECHANISM (how it works, not just what it aims to do)
3. NOVELTY -- it is NOT a well-known existing technology or framework

ANTI-PATTERNS (do NOT extract these):
- Well-known existing technologies (blockchain, federated learning, differential privacy, smart contracts, etc.)
- References to other people's published work or existing projects
- Vague policy recommendations ("we should create better governance")
- Generic categories of technology ("AI-enhanced monitoring systems")
- Abstract principles, values, or goals
- Restatements of problems without a proposed solution

Most sections yield 0-2 entities. Many sections yield 0. Return an empty array [] if nothing in this section is novel AND specific enough.

{ENTITY_SCHEMA_INSTRUCTION}
```

Each user prompt is followed by `\n\n---\n\n{chunk}`, where `{chunk}` is the source text (or a chunk of it for long documents).

---

## 2. Deduplication

**Purpose:** Identify duplicate entities via pairwise comparison, then assign all entities to thematic groups.

**Model:** `claude-haiku-4-5-20251001`, temperature `0`

### 2a. Pairwise comparison

Pre-filter: TF-IDF cosine similarity on entity names + one-liners. Only pairs above a 0.3 threshold are sent to the LLM.

**System prompt:**

```
You compare entity descriptions and return JSON only.
```

**User prompt:**

```
You are comparing two hyper-entity candidates to determine if they describe the same concept.

Entity A:
- Name: {name_a}
- One-liner: {oneliner_a}
- Mechanism: {mechanism_a}

Entity B:
- Name: {name_b}
- One-liner: {oneliner_b}
- Mechanism: {mechanism_b}

Classify the relationship as exactly one of:
- SAME: These describe the same entity/concept/system (even if named differently). They should be merged.
- OVERLAPPING: Related concepts in the same domain, but distinct enough to keep separate.
- DISTINCT: Unrelated or only superficially similar.

Return a JSON object: {"verdict": "SAME"|"OVERLAPPING"|"DISTINCT", "reason": "one sentence explanation"}
```

### 2b. Group definition

Two-step process to avoid output token overflow: first define groups, then assign entities in batches of 50.

**System prompt (both steps):**

```
You categorize entities into thematic groups and return JSON only.
```

**Step 1 -- Define groups:**

```
Below is a list of {n} hyper-entity candidates (future technologies, systems, and institutions).

Define 8-12 thematic groups that cover all these entities. Return a JSON array of group names.
Example: ["Decentralized Governance", "Biotech & Health", "Energy & Climate"]

Entities:
{entity_list}
```

`{entity_list}` is a bullet list of entity names: `- Entity Name`.

**Step 2 -- Assign entities to groups (batched, 50 per call):**

```
Assign each entity below to exactly ONE of these groups: {groups}

Return a JSON object mapping each entity name (exactly as given) to its group name.
Example: {"Entity Name": "Decentralized Governance", "Another Entity": "Biotech & Health"}

Entities:
{entity_list}
```

`{groups}` is a comma-separated string of the group names from Step 1. `{entity_list}` is a bullet list of `- Name: one_liner`.

---

## 3. Web Research

**Purpose:** Enrich each entity with real-world evidence: organizations, funding, TRL, publications, state of the art, and barriers.

**Model:** `claude-haiku-4-5-20251001`, temperature `0`, with `web_search` tool (max 3 searches per entity)

**System prompt:**

```
You are a research analyst. Search the web to find real-world evidence about proposed technologies. Return valid JSON only.
```

**User prompt:**

```
Research this proposed technology/system/institution:

Name: {name}
Description: {one_liner}
Mechanism: {mechanism}
Existing work: {exists_today}

Search the web to find:
1. ORGANIZATIONS (2-5) working on this or closely related tech -- provide name, URL, and role
2. FUNDING -- specific amounts, sources, and years if findable
3. TRL LEVEL (1-9) -- Technology Readiness Level with justification
4. KEY PUBLICATIONS/DEMOS (1-3) -- with titles, dates, and URLs
5. STATE OF THE ART -- 3-5 sentences on where things actually stand today
6. BARRIERS -- 2-3 sentences on what's blocking progress

Return your findings as a JSON object with this exact structure:
{schema}

If you cannot find information for a field, use "None found" for strings, [] for arrays, and 1 for TRL.
Return ONLY the JSON object, no other text.
```

**Output schema (`{schema}`):**

```json
{
  "organizations": [
    {"name": "Org Name", "url": "https://...", "role": "Building X"}
  ],
  "funding": "Series A $10M from Y in 2024",
  "trl": 3,
  "trl_justification": "Lab prototypes demonstrated but no field testing",
  "key_publications": [
    {"title": "Paper Title", "date": "2024", "url": "https://..."}
  ],
  "state_of_the_art": "3-5 sentences on where things stand",
  "barriers": "2-3 sentences on what's blocking progress"
}
```

---

## 4. Scoring

**Purpose:** Score each entity on d/acc values alignment, actionability, and transformative potential.

**Model:** `claude-haiku-4-5-20251001`, temperature `0`

**System prompt:**

```
You are an expert technology assessor. Score entities precisely using the provided rubrics. Return valid JSON only.
```

**User prompt:**

```
Score this hyper-entity candidate on three dimensions. Use ONLY evidence from the provided description and research data. No evidence = score 0.

## Entity
Name: {name}
One-liner: {one_liner}
Mechanism: {mechanism}
Exists today: {exists_today}
Source quote: {source_quote}

## Research data
Organizations: {organizations}
Funding: {funding}
TRL: {trl} -- {trl_justification}
Publications: {publications}
State of the art: {state_of_art}
Barriers: {barriers}

## Scoring dimensions

### A. d/acc Values (each 0-5)
- **Democratic**: Does this distribute decision-making power? (0=concentrates power, 5=radically democratizes)
- **Decentralized**: Does this reduce single points of failure/control? (0=highly centralized, 5=fully distributed)
- **Defensive**: Does this protect rather than attack? Is it defense-dominant? (0=offensive, 5=purely defensive)
- **Differential**: Does this accelerate defensive tech faster than offensive tech? (0=accelerates offense, 5=strongly differential)

### B. Actionability
- **readiness_bottleneck**: What is the SINGLE biggest barrier? One of: Physics, Engineering, Funding, Regulation, Coordination, Social Acceptance
- **what_to_do_now**: What should someone do TODAY? One of: Build, Research, Advocate, Convene, Nothing Yet
- **foresight_connection**: How prominently discussed in source material? (0=barely mentioned, 1=mentioned in passing, 2=substantively discussed, 3=central focus)

### C. Transformative potential (0-5)
- 0=incremental improvement, 1=notable advance, 2=transforms a niche, 3=transforms a field, 4=transforms multiple fields, 5=civilizational new action space

Return ONLY a JSON object with this structure:
{schema}
```

**Output schema (`{schema}`):**

```json
{
  "dacc": {
    "democratic": "<0-5>",
    "democratic_evidence": "...",
    "decentralized": "<0-5>",
    "decentralized_evidence": "...",
    "defensive": "<0-5>",
    "defensive_evidence": "...",
    "differential": "<0-5>",
    "differential_evidence": "..."
  },
  "actionability": {
    "readiness_bottleneck": "Physics|Engineering|Funding|Regulation|Coordination|Social Acceptance",
    "what_to_do_now": "Build|Research|Advocate|Convene|Nothing Yet",
    "foresight_connection": "<0-3>"
  },
  "transformative": {
    "score": "<0-5>",
    "evidence": "..."
  }
}
```

Post-processing clamps all numeric scores to their valid ranges and computes `composite = dacc.total + transformative.score` (max 25).

---

## 5. Curation

**Purpose:** Assign entities to Tier 1 (Spotlight) or Tier 2 (Watch List).

**Method:** Deterministic Python rules. No LLM calls.

### v2 consensus matching

Before tiering, each v3 entity is matched against v2 consensus entities using TF-IDF cosine similarity (char n-grams 2-4, threshold >= 0.4). Matched entities get a lower d/acc bar for Tier 1.

### Tiering rules

An entity qualifies for **Tier 1** if ALL of the following hold:

| Criterion | v2 consensus entity | New entity (no v2 match) |
|---|---|---|
| d/acc total | >= 11 | >= 13 |
| Transformative score | >= 3 | >= 3 |
| Foresight connection | >= 2 | >= 2 |
| TRL | >= 2 | >= 2 |

Everything else is **Tier 2**. Within each tier, entities are sorted by composite score descending.

---

## 6. Report Generation

**Purpose:** Generate the narrative report with executive summary, methodology, Tier 1 entity writeups, and structured tables.

**Model:** `claude-sonnet-4-6`, temperature `0.3`

**System prompt (shared across all report calls):**

```
You are an expert technology policy writer producing a professional report for the Foresight Institute. Write in clear, direct prose. Avoid AI writing patterns: no "tapestry", "landscape of", "paradigm shift", "delve into", "it's worth noting", "in conclusion". Use concrete language. Do not add meta-commentary about the report itself. Return ONLY the markdown content requested, no preamble.
```

### 6a. Executive summary and methodology

**User prompt:**

```
Write two sections for a report on hyper-entities -- future systems that don't exist yet but are already reorganizing coordination, investment, and narrative around their anticipated existence.

DATA:
- {stats['total']} candidates analyzed from 109 sources (Existential Hope podcast transcripts, world gallery submissions, AI pathways essays)
- {stats['tier1_count']} spotlight entities (Tier 1), {stats['tier2_count']} watch list (Tier 2)
- {stats['v2_matches']} entities also appeared in v2 analysis (cross-version consensus)
- Average d/acc score: {stats['avg_dacc']}/20
- Average transformative score: {stats['avg_transformative']}/5
- Average TRL: {stats['avg_trl']}
- TRL distribution: {stats['trl_distribution']}

GROUPS:
{groups_str}

ACTION TYPES:
{actions_str}

BOTTLENECKS:
{bottleneck_str}

TIER 1 ENTITIES:
{tier1_summaries}

Write:

## 1. Executive Summary (~500 words)
Cover: what hyper-entities are (coined by Michael Nielsen), key findings, the 19 spotlight vs 170 watch list, d/acc framework (Vitalik Buterin -- democratic, decentralized, defensive, differential), most common bottlenecks and recommended actions. Reference that sources come from Existential Hope (existentialhope.com), the Foresight Institute's initiative.

## 2. Methodology (~300 words)
Cover: V3 pipeline (extract from 109 sources -> deduplicate -> web research -> score on d/acc + transformative + actionability -> curate into tiers), scoring dimensions, tiering criteria (composite score threshold), source categories. Mention that scoring was done by Claude API with human curation.

Use markdown headers as shown. Be specific with numbers. Write for an audience of funders, policymakers, and technologists.
```

`{tier1_summaries}` is one line per Tier 1 entity in the format:
```
- {name} | group={group} | d/acc={dacc_total}/20 | transformative={trans_score}/5 | composite={composite} | action={action}
```

`{groups_str}`, `{actions_str}`, `{bottleneck_str}` are bullet lists of `- Label: count entities`.

### 6b. Entity writeup (one call per Tier 1 entity)

**User prompt:**

```
Write a spotlight entry (~200-300 words) for this hyper-entity. This is entity {idx + 1} of {total} in the Tier 1 section of a Foresight Institute report.

ENTITY DATA:
{detail}

FORMAT (use this exact structure):

### {entity['name']}
**{entity.get('group', '')}** | Composite: {composite}

[One-liner description]

**How it works.** [2-3 sentences on mechanism, drawn from the data above]

**Who's building toward this.** [List real organizations from the research data with their roles. Include funding and TRL.]

**d/acc alignment.** [Which dimensions score highest and why, 1-2 sentences. Reference actual scores.]

> **What can someone do RIGHT NOW?** [Based on the action type ({action}) and bottleneck ({bottleneck}), write 1-2 concrete sentences about what a funder/builder/researcher/advocate could do today.]

> "{entity.get('source_quote', '')}" -- *Source: [{source_slug}]({source_url})*

Be factual. Use the research data provided -- do not invent organizations or funding amounts.
```

`{detail}` is a structured block containing all entity fields:

```
Name: ...
Group: ...
One-liner: ...
Mechanism: ...
Exists today: ...
Source quote: "..."
Speaker: ...
Source URL: ...

Organizations: Org1 (role); Org2 (role)
Funding: ...
TRL: N -- justification
Publications: Title1 (2024); Title2 (2023)
State of the art: ...
Barriers: ...

d/acc scores: Democratic=N/5, Decentralized=N/5, Defensive=N/5, Differential=N/5 (Total=N/20)
d/acc summary: ...
Transformative: N/5 -- evidence
Bottleneck: Type -- evidence
Action: Type -- evidence
Composite score: N
v2 consensus: Yes/No
```
