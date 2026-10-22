# The Reliability Stack

A cross-layer taxonomy for engineering reliable AI systems.

**Preprint, October 2026. arXiv identifier pending.**

[Read the paper (PDF)](paper.pdf)

## What this is

The Reliability Stack organizes the decisions that determine whether an AI system is reliable into six layers: task and risk specification (L0), learning objective (L1), representation (L2), inference architecture (L3), output contract (L4), and assurance and control (L5).

The paper's claim is that reliability is inherited across those layers. A choice at one layer creates failure modes that a lower layer can relocate but not remove. From that view it derives a selection procedure: two axes, answer-space openness and cost of error, return a candidate operating mode plus the evidence a team needs before deploying it.

The synthesis is typed by evidence. Eighteen claim families carry one of six classes (theory, independent empirical, author-reported, vendor-reported, verified synthesis, watch), applied to individual numbers rather than whole papers. Seven case studies test the taxonomy, including one honest null.

This repository contains the manuscript and its LaTeX source. It is not a code library.

## Contents

- `paper.pdf`: the compiled manuscript (65 pages)
- `latex/paper/`: LaTeX source, section files, TikZ figures, bibliography
- `CITATION.cff`: citation metadata
- `LICENSE`: CC BY 4.0

## Build

Requires [Tectonic](https://tectonic-typesetting.github.io/) or a LaTeX distribution with the packages listed in `latex/paper/main.tex`.

```bash
cd latex/paper
tectonic main.tex
```

The build writes `latex/paper/main.pdf`. The repository copy at `paper.pdf` is the released version.

## Cite

GitHub's "Cite this repository" button reads `CITATION.cff`. For BibTeX:

```bibtex
@misc{cura2026reliabilitystack,
  author       = {Cura, Oğuz Emre},
  title        = {The Reliability Stack: A Cross-Layer Taxonomy for Engineering Reliable AI Systems},
  year         = {2026},
  howpublished = {\url{https://github.com/oguzcura/reliability-stack}},
  note         = {Preprint; arXiv identifier pending}
}
```

Replace the note with the arXiv identifier when it is announced.

## License

The manuscript and figures are licensed under CC BY 4.0. See `LICENSE`.

## Contact

Oğuz Emre Cura, Independent Researcher  
oguzemrecura@gmail.com  
https://github.com/oguzcura
