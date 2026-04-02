# NRR-Projection

Local workspace for the `NRR-Projection` theory line.
This line is positioned as a companion paper to `NRR-Phi` and a bridge paper connecting the Phi state ontology to the comparison-and-boundary surfaces now consolidated in integrated `paper7`, with downstream carry-forward into Energy and Guarantee while remaining a theory-first bridge line rather than an operational-control or assurance paper.

## Structure

- `manuscript/current/`: latest manuscript source and compiled PDF
- `manuscript/archive/`: prior manuscript versions kept for history
- `artifacts/reviewpacks/`: zip bundles used for review handoff

## Current Manuscript

- `manuscript/current/nrr-projection_manuscript_v24.tex`
- `manuscript/current/nrr-projection_manuscript_v24.pdf`
- `manuscript/current/checksums_sha256.txt`

## Reproducibility

- Build command: `bash scripts/build_current_manuscript.sh`
- Current checksum manifest: `bash scripts/verify_current_package.sh`
- Current narrow review surfaces bundle the manuscript package plus the inherited
  Boundary CSV support surface used to audit Section 5:
  `nrr-boundary/stats/combo_rep3_all/mst_sign_flip_boundaries.csv` and
  `nrr-boundary/stats/combo_rep3_all/mst_tau_trace_provider_balanced.csv`
- No new Projection-specific experiment assets are introduced for this theory paper;
  the bundled CSVs are historical support inputs for the package-first reinterpretation.

## Notes

- This workspace is organized as a standalone git-managed line so Projection can be versioned independently from the parent workspace.
- The parent workspace `.gitignore` ignores `nrr-*`, so this folder is intentionally managed as its own repository.
- Reviewpack zip bundles are handoff artifacts and may be produced outside the committed git tree.

Stable review-package entrypoints:
- `bash scripts/build_current_manuscript.sh`
- `bash scripts/verify_current_package.sh`
