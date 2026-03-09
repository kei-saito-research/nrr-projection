# NRR-Projection

Local workspace for the `NRR-Projection` theory line.
This line is positioned as a companion paper to `NRR-Phi` and a bridge paper connecting the Phi state ontology to the empirical boundary patterns reported in `NRR-Boundary`.

## Structure

- `manuscript/current/`: latest manuscript source and compiled PDF
- `manuscript/archive/`: prior manuscript versions kept for history
- `artifacts/reviewpacks/`: zip bundles used for review handoff

## Current Manuscript

- `manuscript/current/nrr-projection_manuscript_v20.tex`
- `manuscript/current/nrr-projection_manuscript_v20.pdf`
- `manuscript/current/checksums_sha256.txt`

## Reproducibility

- Build command: `tectonic -X compile manuscript/current/nrr-projection_manuscript_v20.tex`
- Current checksum manifest: `manuscript/current/checksums_sha256.txt`
- This repository currently tracks the manuscript package only; no new Projection-specific experiment assets are required for the theory paper.

## Notes

- This workspace is organized as a standalone git-managed line so Projection can be versioned independently from the parent workspace.
- The parent workspace `.gitignore` ignores `nrr-*`, so this folder is intentionally managed as its own repository.
- Reviewpack zip bundles are handoff artifacts and may be produced outside the committed git tree.
