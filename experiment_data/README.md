# Thesis experiment data

The CSV files in this directory are generated from benchmark suites with:

```bash
python scripts/summarize_thesis_experiments.py
```

`runs.csv` contains one row per training run, `by_scene.csv` contains per-scene
aggregates, and `overall.csv` contains experiment-level aggregates. Paper-style
VGG LPIPS is joined from a suite's common file or method-specific file.

`profile_*.csv` contains the matched three-scene profiler traces.
`fused_backend_*.csv` and `fused_backend_validation.json` contain the backend
microbenchmark and numerical checks. `external_repositories.csv` records the
separate official RapidGS and gaussian-splatting repository runs; those rows
are not mixed into the local implementation summaries.
