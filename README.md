# Cross-Over Trigger Function via Persona Reference Attention and Drift-Resistant Anchoring via Named-Subject Persona Reference Attention (PRACT)

A prompt engineering methodology for preventing persona drift and triggering cross-section attention in Large Language Models through minimal named-subject design.

## Overview

The **Persona Reference Attention Cross-Trigger (PRACT)** is a prompt engineering methodology that addresses **persona drift** and **attention decay** in long-form LLM sessions through a minimal-design approach using a named subject.

The methodology rests on the observed phenomenon that the act of naming a persona and repeatedly using that name as the grammatical subject within responses generates persistent attention to the persona's defining text, dynamically regenerating reference at each turn of response generation.

Building on this observation, PRACT further formalizes a *cross-over trigger function*: by inscribing the names of other sections within the persona's character description, each use of the named subject generates cross-over attention to those sections, dramatically improving the execution rate of rules contained therein.

PRACT addresses **attention decay** as formalized by Benderahmane et al. (2024), and builds on the research on identity token propagation by Poonia and Jain (2025) and the practical knowledge of semantic anchors by stunspot (2026).

### Key Characteristics

- **Minimal design**: A single-sentence construction enforcing the persona's name as the subject in every response
- **Persona reference attention**: Dynamic self-referential attention to the persona definition is generated at each occurrence of the named subject
- **Cross-over trigger function**: Section names inscribed within the persona definition produce cross-over attention to those sections, improving rule execution rates
- **Drift prevention**: Long-form session stability verified for approximately 70 turns under Gemini's low-performance fast mode
- **Standalone operation**: Functions independently without combination with other prompt engineering methodologies
- **Cross-model functionality**: Confirmed effects on Anthropic Claude and Google Gemini

## Citation

```
@misc{masahiko_o_2026_pract,
  author       = {Masahiko.O},
  title        = {Cross-Over Trigger Function via Persona Reference Attention and Drift-Resistant Anchoring via Named-Subject Persona Reference Attention (PRACT)},
  year         = {2026},
  doi          = {10.5281/zenodo.20024118},
  url          = {https://doi.org/10.5281/zenodo.20024118},
  note         = {Preprint v1.1, originally presented 2026-05-02}
}
```

- **Author**: Masahiko.O
- **DOI (v1.1)**: [10.5281/zenodo.20024118](https://doi.org/10.5281/zenodo.20024118)
- **Concept DOI (all versions)**: [10.5281/zenodo.19975248](https://doi.org/10.5281/zenodo.19975248)
- **License**: Creative Commons Attribution 4.0 International (CC-BY-4.0)

## Full Paper

- **[paper.md](https://github.com/Masahiko-O/Persona-Reference-Attention-Cross-Over-Trigger/blob/main/paper.md)** — Full paper in Markdown format (v1.1)
- **[paper.pdf](https://github.com/Masahiko-O/Persona-Reference-Attention-Cross-Over-Trigger/blob/main/paper.pdf)** — PDF version (v1.1)

Original preprint on Zenodo (v1.1):

- https://doi.org/10.5281/zenodo.20024118

## Related Protocols

This is part of a four-protocol research series on natural-language LLM intervention by Masahiko.O:

- **[GIP](https://github.com/Masahiko-O/Governance-Interlock-Protocol)** — Instruction adherence through pre-generative self-attestation
- **[CMDP](https://github.com/Masahiko-O/Convergence-Multi-Layer-Distribution-Prompting)** — Probability distribution redistribution for creative output
- **PRACT** (this repository) — Persona drift prevention via named-subject attention
- **[CAP](https://github.com/Masahiko-O/Contradiction-Avoidance-Protocol)** — Internal state articulation through metaphorical translation

## Author

**Masahiko.O** — Independent AI researcher

- GitHub: [@Masahiko-O](https://github.com/Masahiko-O)

## License

This work is licensed under [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/). You are free to share and adapt the material with proper attribution.
