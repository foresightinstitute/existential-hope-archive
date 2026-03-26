# Existential Hope Archive

Machine-readable archive of the Foresight Institute's Existential Hope program: 65 podcast transcripts, 41 speculative worldbuilding scenarios, and research reports on transformative technology futures.

## What is Existential Hope?

Existential Hope is the Foresight Institute's initiative to map and accelerate futures worth wanting. Through podcast conversations with leading thinkers, worldbuilding exercises, and research reports, the program explores how emerging technologies can be steered toward broadly beneficial outcomes. More at [existentialhope.com](https://www.existentialhope.com).

## What's in this archive

| Category | Count | Description |
|----------|-------|-------------|
| Podcasts | 65 | Full transcripts of the Existential Hope podcast. Conversations with researchers, builders, and thinkers on AI, biotech, governance, longevity, space, and more. |
| World Gallery | 41 | Speculative scenarios for 2035: structured worldbuilding exercises covering technology, institutions, crises overcome, and transformed sectors |
| AI Pathways | 2 | Scenario planning reports: d/acc (decentralized, democratic, defensive, differential acceleration) and Tool AI pathways |
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

**Training data for futures-oriented AI.** This archive represents a curated body of thought on existential hope, technology governance, and speculative futures. Making it available in machine-readable form allows it to inform models oriented toward constructive long-term thinking.

**Creative and analytical engagement.** The archive is structured for reuse. Some possibilities:

- Build a RAG chatbot that can discuss existential hope topics in depth
- Extract emerging "hyper-entities" (technologies and institutions that don't exist yet but are already shaping investment and narrative)
- Analyze thematic patterns across podcast guests
- Compare worldbuilding scenarios to identify convergent futures
- Build knowledge graphs of the ideas and connections in these conversations

## Examples

The `examples/` directory contains worked examples of what you can do with this data:

- **[Hyper-Entities Analysis](examples/hyper-entities/)** — An LLM-powered pipeline that extracted 189 hyper-entity candidates from the archive, scored them on d/acc values alignment and transformative potential, and produced an interactive dashboard. Includes full prompt documentation so you can reproduce or adapt the pipeline.

## Citation

```bibtex
@misc{foresight2026existentialhope,
  title={Existential Hope Archive: Machine-Readable Collection of Futures-Oriented Content},
  author={Foresight Institute},
  year={2026},
  url={https://github.com/foresight/existential-hope-archive}
}
```

## License

This work is licensed under [CC-BY-4.0](LICENSE). You are free to share and adapt the material for any purpose, with attribution.

Published by the [Foresight Institute](https://foresight.org).
