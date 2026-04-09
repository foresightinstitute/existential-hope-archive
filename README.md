# Existential Hope Archive

How could emerging technology go well? 490,000 words of expert thinking on positive futures: podcast transcripts, worldbuilding scenarios, and research reports from the Foresight Institute's Existential Hope program. Structured for reuse.

## What is Existential Hope?

Most serious thinking about technology's future focuses on what could go wrong. Existential Hope is the Foresight Institute's initiative to focus on what could go right, and what it would take to get there. The program brings together researchers, builders, and technologists to map futures worth wanting across AI, biotech, governance, longevity, and space. More at [existentialhope.com](https://www.existentialhope.com).

## What's in this archive

| Category | Count | Description |
|----------|-------|-------------|
| [Podcasts](https://www.existentialhope.com/podcasts) | 65 | Full transcripts of the Existential Hope podcast. Conversations with researchers, builders, and thinkers on AI, biotech, governance, longevity, space, and more. |
| [World Gallery](https://worlds.existentialhope.com) | 41 | Speculative scenarios for 2035: structured worldbuilding exercises covering technology, institutions, crises overcome, and transformed sectors |
| [AI Pathways](https://www.existentialhope.com/ai-pathways) | 2 | Scenario planning reports: d/acc (decentralized, democratic, defensive, differential acceleration) and Tool AI pathways |
| X-Hope | 1 | Report from the Transformative AI Institution Design Hackathon (Feb 2024, SF) |

Total: ~490,000 words of curated content on technology futures.

## Data format

All content is in Markdown (.md) files organized by category:

```
data/
├── podcasts/           # "Speaker Name | Topic.md" format, timestamped transcripts
├── world-gallery/      # "World Name.md" format, structured scenario templates
├── reports/
│   ├── ai-pathways/    # Long-form research reports
│   └── x-hope/        # Hackathon documentation
└── source_urls.json    # Index mapping each file to its source URL and type
```

## Why we're publishing this

Most thinking about positive technology futures — how emerging tech could actually go well — lives in formats that are hard to build on: podcast audio, one-off blog posts, workshop notes. There's plenty of machine-readable data on risks and failures. There's much less on what good outcomes look like and how to get there. This archive brings 490,000 words of that thinking into a single, structured, machine-readable dataset.

Two reasons this matters:

**Better source material for AI.** Models trained or augmented on this archive can reason about beneficial futures with more depth than generic training data provides. If you're building AI tools for foresight, scenario planning, or technology governance, this is a curated starting point.

**A base layer for new work.** The archive is structured for reuse. Some possibilities:

- Identify convergent futures: what do 41 independent worldbuilding scenarios keep arriving at?
- Extract hyper-entities — technologies and institutions that don't fully exist yet but are already attracting funding, talent, and attention, like chemputing or immune-computer interfaces (a concept from Michael Nielsen). We did this as a [worked example](examples/hyper-entities/).
- Map where 65 experts agree and disagree on which technologies will matter most
- Build foresight or scenario-planning tools grounded in real expert thinking
- Build knowledge graphs of the ideas, people, and connections across conversations

## Examples

**[Hyper-Entities Analysis](examples/hyper-entities/)** — Which technologies could help build the best possible future but aren't getting the attention they deserve? We used an LLM pipeline to scan the archive, extract 188 candidates, and narrow to 10 that we think are high-impact but under-resourced. Includes full prompt documentation so you can reproduce or adapt the pipeline. [Explore the interactive dashboard.](https://foresightinstitute.github.io/existential-hope-archive/examples/hyper-entities/dashboard/)

## Citation

```bibtex
@misc{foresight2026existentialhope,
  title={Existential Hope Archive: Machine-Readable Collection of Futures-Oriented Content},
  author={Foresight Institute},
  year={2026},
  url={https://github.com/foresightinstitute/existential-hope-archive}
}
```

## License

This work is licensed under [CC-BY-4.0](LICENSE). You are free to share and adapt the material for any purpose, with attribution.

Published by the [Foresight Institute](https://foresight.org).
