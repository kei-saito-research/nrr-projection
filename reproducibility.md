# Reproducibility (NRR-Projection)

## Scope

This repository currently provides the manuscript package for the Projection theory line.
The manuscript is theory-first and does not add new Projection-specific experiments in this version.
The manuscript discusses historical Boundary evidence as an external source surface for the Section 5 empirical-contact reinterpretation, but this repository's current package is limited to the Projection manuscript line and stable verification wrappers.

## Stable review-package commands

- Build the current manuscript to temp output:
  - `bash scripts/build_current_manuscript.sh`
  - output: `/tmp/nrr-projection_current_build/nrr-projection_manuscript_v26.pdf`
- Verify the active review surface:
  - `bash scripts/verify_active_review_surface.sh`
- Verify the current review-package checksum manifest:
  - `bash scripts/verify_current_package.sh`

## Current review package

- Main TeX: `manuscript/current/nrr-projection_manuscript_v26.tex`
- Current PDF snapshot: `manuscript/current/nrr-projection_manuscript_v26.pdf`
- Active review checksum manifest: `manuscript/checksums_active_review_surface_sha256.txt`
- Current package checksum manifest: `manuscript/checksums_current_package_sha256.txt`
- `manuscript/current/` is latest-only and contains only the active manuscript `.tex` / `.pdf` pair.

## Checksum policy

- `manuscript/checksums_active_review_surface_sha256.txt` covers the active review
  surface and is limited to the committed current `.tex` / `.pdf` pair in
  `manuscript/current/`.
- `manuscript/checksums_current_package_sha256.txt` covers the repository files
  needed to verify the current Projection manuscript line and stable scripts.
- Older manuscript versions are not retained in `manuscript/current/`; version history
  is tracked through git history.

## Build

Compile from repository root:

```bash
bash scripts/build_current_manuscript.sh
```

Default temp output:
- `/tmp/nrr-projection_current_build/nrr-projection_manuscript_v26.pdf`

## Current manuscript package details

- Main TeX: `manuscript/current/nrr-projection_manuscript_v26.tex`
- PDF snapshot: `manuscript/current/nrr-projection_manuscript_v26.pdf`
- Active review checksum manifest: `manuscript/checksums_active_review_surface_sha256.txt`
- Current package checksum manifest: `manuscript/checksums_current_package_sha256.txt`

## Artifact map

| Artifact | Command | Output |
|---|---|---|
| Current manuscript build | `bash scripts/build_current_manuscript.sh` | `/tmp/nrr-projection_current_build/nrr-projection_manuscript_v26.pdf` |
| Active review surface verification | `bash scripts/verify_active_review_surface.sh` | stdout verification for `manuscript/checksums_active_review_surface_sha256.txt` plus latest-only checks on `manuscript/current/` |
| Current package checksum verification | `bash scripts/verify_current_package.sh` | stdout verification for `manuscript/checksums_current_package_sha256.txt` |
| Current manuscript source snapshot | N/A (tracked artifact) | `manuscript/current/nrr-projection_manuscript_v26.tex` |

Verify the tracked package:

```bash
bash scripts/verify_current_package.sh
```

## Notes

- The `NRR-Patterns` discussion in the manuscript is a post hoc reinterpretation of existing reported results, not a new Projection experiment.
- The historical Boundary evidence cited in Section 5 is external to this repository's current package.
- Any future Projection-specific empirical test should be added under a separately fixed protocol.
