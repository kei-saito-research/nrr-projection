# Scripts

This directory contains the stable manuscript/reproducibility wrappers for the
Projection theory repository surface.

## Stable entrypoints

- `build_current_manuscript.sh`
  - builds the current manuscript to a temp output directory
- `verify_active_review_surface.sh`
  - verifies that `manuscript/current/` contains only the current `.tex` / `.pdf` pair and checks `manuscript/checksums_active_review_surface_sha256.txt`
- `verify_current_package.sh`
  - verifies the active review surface first and then checks `manuscript/checksums_current_package_sha256.txt`

Projection is a theory-first manuscript repository surface. The stable public
interface for the current package remains the three entrypoints above.
