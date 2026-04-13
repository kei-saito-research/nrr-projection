# Reproducibility (NRR-Projection)

## Scope

This repository provides the current manuscript package for the Projection theory line. The current package contains the manuscript snapshot and stable verification wrappers. It does not bundle Projection-specific experiment assets in this version.

## Primary package commands

- Build the current manuscript to temp output:
  - `bash scripts/build_current_manuscript.sh`
  - output: `/tmp/nrr-projection_current_build/nrr-projection_manuscript_v28.pdf`
- Verify the current manuscript files:
  - `bash scripts/verify_active_review_surface.sh`
- Verify the current package checksum manifest:
  - `bash scripts/verify_current_package.sh`

## Current snapshot

- Main TeX: `manuscript/current/nrr-projection_manuscript_v28.tex`
- Current PDF snapshot: `manuscript/current/nrr-projection_manuscript_v28.pdf`
- Current manuscript checksum manifest: `manuscript/checksums_active_review_surface_sha256.txt`
- Current package checksum manifest: `manuscript/checksums_current_package_sha256.txt`

## Checksum policy

- `manuscript/checksums_active_review_surface_sha256.txt` covers the committed current
  manuscript `.tex` / `.pdf` pair in `manuscript/current/`.
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
- `/tmp/nrr-projection_current_build/nrr-projection_manuscript_v28.pdf`

## Current manuscript package details

- Main TeX: `manuscript/current/nrr-projection_manuscript_v28.tex`
- PDF snapshot: `manuscript/current/nrr-projection_manuscript_v28.pdf`
- Current manuscript checksum manifest: `manuscript/checksums_active_review_surface_sha256.txt`
- Current package checksum manifest: `manuscript/checksums_current_package_sha256.txt`

## Artifact map

| Artifact | Command | Output |
|---|---|---|
| Current manuscript build | `bash scripts/build_current_manuscript.sh` | `/tmp/nrr-projection_current_build/nrr-projection_manuscript_v28.pdf` |
| Current manuscript verification | `bash scripts/verify_active_review_surface.sh` | stdout verification for `manuscript/checksums_active_review_surface_sha256.txt` plus latest-only checks on `manuscript/current/` |
| Current package checksum verification | `bash scripts/verify_current_package.sh` | stdout verification for `manuscript/checksums_current_package_sha256.txt` |
| Current manuscript source snapshot | N/A (tracked artifact) | `manuscript/current/nrr-projection_manuscript_v28.tex` |

Verify the tracked package:

```bash
bash scripts/verify_current_package.sh
```

## Notes

- This repository is a manuscript-centered package for the Projection line.
- Any future Projection-specific empirical test should be added as a separate, clearly documented artifact set.
