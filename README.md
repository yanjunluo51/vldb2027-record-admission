# Record Admission and Evaluation Targets Shape Query Scores in LLM Extraction Pipelines

Supplemental material and reproducibility artifact for the VLDB 2027 Experiment, Analysis & Benchmark submission of the same title.

## Download

The complete artifact is attached to the release **v1.1** of this repository:

https://github.com/yanjunluo51/vldb2027-record-admission/releases/tag/v1.1

- File: `record-admission-artifact-v1.1.zip` (about 371 MB)
- SHA-256: `cb88ef6fa895ebead2c033f0366f72fc2a9302f9a8a4908eeda445deb5b5eb9f`

## Contents of the archive

- `paper/`: the paper, its LaTeX sources and the supplement (`paper/supplement/main.pdf`).
- `reproducibility/`: all saved model outputs, references, analysis code and frozen protocols for the news, literary, relation-extraction and DocETL experiments.
- `bc5cdr/`: the frozen protocol, the 2,480 saved requests and the offline analysis of the BC5CDR audit.
- `reporting/`: the reporting template and a filled BC5CDR example.

Replay needs no new inference, GPU or paid API. After extraction, run `python3 verify_manifest.py`, then follow `README.md` inside the archive.

## Licenses

The archive combines components under different terms. See `LICENSE.md` and `LICENSES_AND_SCOPE.md`.

Version v1.0 contains the same artifact with the paper before its final layout revision.
