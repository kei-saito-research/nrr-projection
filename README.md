# NRR-Projection

Local workspace for the `NRR-Projection` theory line.
This line is positioned as a companion paper to `NRR-Phi` and a bridge paper connecting the Phi state ontology to the comparison-and-boundary surfaces now consolidated in `NRR-Patterns`, with downstream carry-forward into Energy and Guarantee while remaining a theory-first bridge line rather than an operational-control or assurance paper.

## Structure

- `manuscript/current/`: latest-only manuscript source and compiled PDF
- `manuscript/archive/`: prior manuscript versions kept for history

## Current Manuscript

- `manuscript/current/nrr-projection_manuscript_v27.tex`
- `manuscript/current/nrr-projection_manuscript_v27.pdf`
- `manuscript/checksums_active_review_surface_sha256.txt`
- `manuscript/checksums_current_package_sha256.txt`
- `manuscript/current/` keeps only the active `.tex` / `.pdf` pair.

## Reproducibility

- Build command: `bash scripts/build_current_manuscript.sh`
- Active review surface verification: `bash scripts/verify_active_review_surface.sh`
- Current package verification: `bash scripts/verify_current_package.sh`
- This repository does not bundle Projection-specific experiment assets.
- The manuscript's package-first reinterpretation cites historical Boundary evidence as an external source surface, but the current Projection repository package is limited to the manuscript and stable verification wrappers.

## Notes

- This workspace is organized as a standalone git-managed line so Projection can be versioned independently from the parent workspace.
- The parent workspace `.gitignore` ignores `nrr-*`, so this folder is intentionally managed as its own repository.
- Reviewpack zip bundles are handoff artifacts and may be produced outside the committed git tree.

Stable review-package entrypoints:
- `bash scripts/build_current_manuscript.sh`
- `bash scripts/verify_active_review_surface.sh`
- `bash scripts/verify_current_package.sh`
