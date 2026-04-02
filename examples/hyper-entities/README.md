# Hyper-Entities: Extracting Future Systems from the Existential Hope Archive

Which technologies could help build the best possible future but aren't getting the attention they deserve? This pipeline scans 490,000 words of expert thinking on positive futures to find out. It identifies and scores "hyper-entities" — technologies, institutions, and coordination systems that don't fully exist yet but are already attracting funding, talent, and attention (a term coined by Michael Nielsen).

## Results

- **189 hyper-entity candidates** extracted from 109 Existential Hope sources
- **19 Tier 1 spotlight entities** selected for deep analysis
- **170 Tier 2 watch list entities** catalogued with scores
- **12 thematic groups** identified through clustering

## Explore

**[Interactive dashboard](https://foresightinstitute.github.io/existential-hope-archive/examples/hyper-entities/dashboard/index-labeled.html)** — Scatter plot visualization (d/acc alignment vs. transformative potential), filtering by group and action type, and detailed entity cards.

**Scored dataset:** `data/curated.json` contains all 189 entities with full scoring, research data, and tier assignments.

## Scoring Dimensions

Each entity is scored on three axes:

- **d/acc Values Alignment** (0-20): Democratic, Decentralized, Defensive, and Differential dimensions (0-5 each), based on Vitalik Buterin's d/acc framework
- **Transformative Potential** (0-5): From incremental improvement to civilizational new action space
- **Actionability**: Readiness bottleneck, recommended action, and foresight connection strength

See [METHODOLOGY.md](METHODOLOGY.md) for the full scoring framework with rubrics.

## Pipeline

The extraction pipeline has six stages. Full prompt text and schemas for each stage are documented in [PROMPTS.md](PROMPTS.md).

1. **Extract** — Pull hyper-entity candidates from source documents (Claude Sonnet)
2. **Deduplicate** — Merge duplicates and assign thematic groups (Claude Haiku)
3. **Research** — Enrich with web evidence: organizations, funding, TRL, publications (Claude Haiku + web search)
4. **Score** — Rate on d/acc, transformative potential, and actionability (Claude Haiku)
5. **Curate** — Assign to Tier 1 or Tier 2 using deterministic threshold rules
6. **Report** — Generate narrative writeups for Tier 1 entities (Claude Sonnet)

## Reproduce

To run this pipeline on the archive data (or your own sources), you'll need:
- An Anthropic API key with access to Claude Sonnet and Haiku models
- Python 3.10+
- The `anthropic` Python SDK

Adapt the prompts in [PROMPTS.md](PROMPTS.md) to your use case. The pipeline cost approximately $17 in API calls for the full 189-entity run.
