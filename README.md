# MMALS v1.1 - Full Status and External Continual-Learning Update

This repository packages the June 12, 2026 status article for Mycelium-Inspired Mutualistic Adaptive Learning Systems (MMALS).

<p align="center">
  <a href="./paper/main.pdf">
    <img src="https://img.shields.io/badge/Open-Article-0B5FFF?style=for-the-badge&logo=adobeacrobatreader&logoColor=white" alt="Open PDF">
  </a>
  <a href=".//docs/MMALS_Section4_Experiments_v4.docx">
    <img src="https://img.shields.io/badge/Open-Section4-0B5FFF?style=for-the-badge&logo=adobeacrobatreader&logoColor=white" alt="Open DOCX">
  </a>
</p>

## Scope

The paper consolidates:

- MNIST-family functional-memory and geometry diagnostics;
- the five-seed RC2O-v2.2c SplitCIFAR10 robust external bridge;
- the five-seed SplitCIFAR100 robust diagnostic;
- the five-seed CORe50 robust diagnostic;
- the two-seed CORe50 v2.3 context-retention rescue ablation.

The strongest current external claim is the SplitCIFAR10 bridge over frozen supervised visual features. SplitCIFAR100 and CORe50 remain diagnostic. The v2.3 CORe50 rescue improves class coverage, forgetting and host diversity but fails the oldest-context gate.

## Repository structure

- `paper/`: LaTeX source, compiled PDF, figures and generated tables.
- `data/`: compact machine-readable evidence used by the article.
- `notebooks/`: key executable notebooks for SplitCIFAR10, CORe50 robust and CORe50 v2.3.
- `docs/`: claim boundary, reproducibility and release notes.

## Build

```bash
cd paper
pdflatex -interaction=nonstopmode main.tex
pdflatex -interaction=nonstopmode main.tex
```

## Scientific status

This is a research status package, not a state-of-the-art claim. It does not establish end-to-end raw-pixel continual representation learning, positive backward transfer, or universal benchmark generality.
