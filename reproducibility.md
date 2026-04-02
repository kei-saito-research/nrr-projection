# Reproducibility (NRR-Projection)

## Scope

This repository currently provides the manuscript package for the Projection theory line.
The manuscript is theory-first and does not add new Projection-specific experiments in this version.
For current narrow review surfaces, the package also bundles the inherited
Boundary CSV support surface used to audit the Section 5 empirical-contact table:
`nrr-boundary/stats/combo_rep3_all/mst_sign_flip_boundaries.csv` and
`nrr-boundary/stats/combo_rep3_all/mst_tau_trace_provider_balanced.csv`.

## Stable review-package commands

- Build the current manuscript to temp output:
  - `bash scripts/build_current_manuscript.sh`
  - output: `/tmp/nrr-projection_current_build/nrr-projection_manuscript_v24.pdf`
- Verify the current review-package checksum manifest:
  - `bash scripts/verify_current_package.sh`

## Current review package

- Main TeX: `manuscript/current/nrr-projection_manuscript_v24.tex`
- Current PDF snapshot: `manuscript/current/nrr-projection_manuscript_v24.pdf`
- Checksum manifest: `manuscript/current/checksums_sha256.txt`
- Bundled support CSVs for Section 5 audit:
  - `nrr-boundary/stats/combo_rep3_all/mst_sign_flip_boundaries.csv`
  - `nrr-boundary/stats/combo_rep3_all/mst_tau_trace_provider_balanced.csv`

## Checksum policy

- `manuscript/current/checksums_sha256.txt` covers the tracked files that define the
  current review package for the latest manuscript line in `manuscript/current/`.
- Coverage includes the current main `.tex` file and the committed current `.pdf`.
- Coverage excludes `checksums_sha256.txt` itself, older manuscript versions that may
  remain in `manuscript/current/` for local working continuity, and repo-specific
  artifacts outside `manuscript/current/` unless a separate manifest is provided.

## Build

Compile from repository root:

```bash
bash scripts/build_current_manuscript.sh
```

Default temp output:
- `/tmp/nrr-projection_current_build/nrr-projection_manuscript_v24.pdf`

## Current manuscript package details

- Main TeX: `manuscript/current/nrr-projection_manuscript_v24.tex`
- PDF snapshot: `manuscript/current/nrr-projection_manuscript_v24.pdf`
- Checksums: `manuscript/current/checksums_sha256.txt`

## Artifact map

| Artifact | Command | Output |
|---|---|---|
| Current manuscript build | `bash scripts/build_current_manuscript.sh` | `/tmp/nrr-projection_current_build/nrr-projection_manuscript_v24.pdf` |
| Current package checksum verification | `bash scripts/verify_current_package.sh` | stdout verification for `manuscript/current/checksums_sha256.txt` |
| Current manuscript source snapshot | N/A (tracked artifact) | `manuscript/current/nrr-projection_manuscript_v24.tex` |
| Bundled Section 5 support surface | N/A (bundled review-surface artifact) | `nrr-boundary/stats/combo_rep3_all/mst_sign_flip_boundaries.csv`, `nrr-boundary/stats/combo_rep3_all/mst_tau_trace_provider_balanced.csv` |

Verify the tracked package:

```bash
bash scripts/verify_current_package.sh
```

## Notes

- The integrated `paper7` package discussion in the manuscript is a post hoc reinterpretation of existing reported results, not a new Projection experiment.
- The bundled Boundary CSVs are supporting audit inputs for that reinterpretation, not new Projection-native experiments.
- Any future Projection-specific empirical test should be added under a separately fixed protocol.
