# Reproducibility (NRR-Projection)

## Scope

This repository currently provides the manuscript package for the Projection theory line.
The manuscript is theory-first and does not add new Projection-specific experiments in this version.

## Build

Compile from repository root:

```bash
bash scripts/build_current_manuscript.sh
```

Default temp output:
- `/tmp/nrr-projection_current_build/nrr-projection_manuscript_v20.pdf`

## Current manuscript package

- Main TeX: `manuscript/current/nrr-projection_manuscript_v20.tex`
- PDF snapshot: `manuscript/current/nrr-projection_manuscript_v20.pdf`
- Checksums: `manuscript/current/checksums_sha256.txt`

Verify the tracked package:

```bash
bash scripts/verify_current_package.sh
```

## Notes

- The Boundary discussion in the manuscript is a post hoc reinterpretation of existing reported results, not a new Projection experiment.
- Any future Projection-specific empirical test should be added under a separately fixed protocol.
