# Scripts

This directory contains the stable build and verification entrypoints for the
Projection manuscript package.

## Entrypoints

- `build_current_manuscript.sh`
  - builds the current manuscript to a temp output directory
- `verify_active_review_surface.sh`
  - verifies that `manuscript/current/` contains only the current `.tex` / `.pdf` pair and checks `manuscript/checksums_active_review_surface_sha256.txt`
- `verify_current_package.sh`
  - verifies the current manuscript files first and then checks `manuscript/checksums_current_package_sha256.txt`
