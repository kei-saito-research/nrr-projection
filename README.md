# NRR-Projection

NRR-Projection hosts the manuscript snapshot for the Projection theory line in the Non-Resolution Reasoning (NRR) research program. This repository is a manuscript-centered package: it provides the current paper source, compiled PDF, and stable verification scripts for the Projection line.

NRR is not an anti-LLM framework.
NRR does not replace standard LLM use.
NRR optimizes when to commit and when to defer, under explicit conditions.

## Key Artifacts

- Current manuscript source:
  - `manuscript/current/nrr-projection_manuscript_v28.tex`
- Current manuscript PDF:
  - `manuscript/current/nrr-projection_manuscript_v28.pdf`
- Reproducibility guide:
  - `reproducibility.md`

## Structure

- `manuscript/current/`: current manuscript source and PDF
- `manuscript/archive/`: earlier manuscript versions
- `scripts/`: build and verification entrypoints

## Reproducibility

See `reproducibility.md` for supported commands and the current artifact map.

Primary package entrypoints:
- `bash scripts/build_current_manuscript.sh`
- `bash scripts/verify_active_review_surface.sh`
- `bash scripts/verify_current_package.sh`

This repository does not bundle Projection-specific experiment assets in the current package.
