# EEG Router — BIBM paper and follow-up code

Authors: Ziquan Wang and Zixuan Luo (equal contribution).

Download **[eeg-router-bibm-source.zip](eeg-router-bibm-source.zip)** for the complete organized source snapshot: **387 files**, including original training/inference support, H1 temporal sharing, H3 detector-source classification, H4 router/oracle evaluation, related router/MoE development, and reviewer-driven follow-up analyses.

The ZIP preserves directory structure:

```text
eeg-router-bibm/
  README.md
  src/bfa/          # preprocessing, detectors, training, evaluation
  scripts/         # original named entry points and follow-up code
  configs/
  protocols/
  tests/
  paper/           # BIBM manuscript and figure source
  archive/         # differing historical/current copies
  docs/            # experiment index, provenance, checksums, known issues
```

After extracting, start with `README.md`, `docs/EXPERIMENTS.md`, and `docs/STATUS.md`.

## Status

The original paper protocol is `v3-groupkfold-confirmatory-v1` (five patient-held-out folds, three seeds). The learned-router negative result is preserved.

The reviewer supplement `257_run_bibm_router_review_diagnostics.py` is unfinished development code. The latest verified artifact is a one-run smoke with zero bootstrap replicates. The full supplementary analysis is not represented as complete.

All packaged Python files pass syntax parsing; five evaluation unit/smoke tests passed. Full training and data-dependent reproduction were not rerun for this upload. Historical paths and external inputs are documented inside the archive.

The archive excludes EEG/patient datasets, predictions, model weights, credentials and private correspondence. Standalone HMM, artifact-ontology and TTT projects are outside this router repository. No new license grant is applied.

Snapshot: 2026-09-30. Archive SHA-256:
`2bcaeab0069c93523d07340e68babb6faf8a43acf73ec95de711d522159b9f65`

This initial upload is a complete source archive; files are organized within the ZIP rather than individually browsable on GitHub.
