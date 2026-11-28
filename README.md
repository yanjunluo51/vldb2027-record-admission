# Record Admission and Evaluation Targets Shape Query Scores in LLM Extraction Pipelines

Supplemental material and reproducibility artifact for the VLDB 2027 Experiment, Analysis & Benchmark submission of the same title.

## Download

The complete artifact is attached to the release **v1.70** of this repository:

https://github.com/yanjunluo51/vldb2027-record-admission/releases/tag/v1.70

- File: `record-admission-artifact-v1.70.zip` (about 371 MB)
- SHA-256: `692b25717414ec66b38eabf92763d6c5d510349ecc163c915d091b3ee9d15919`

## Quick start

Run these commands in the extracted archive. They repeat the steps in `README.md` inside the archive, which explains each step.

```sh
python3 verify_manifest.py
python3 -m venv reproducibility/clean_env
reproducibility/clean_env/bin/python -m pip install -r reproducibility/requirements-cpu.txt
reproducibility/clean_env/bin/python -m pip check
reproducibility/clean_env/bin/python -B reproducibility/configure_paths.py
reproducibility/clean_env/bin/python reproduce.py --bc5cdr-only
reproducibility/clean_env/bin/python reproduce.py --review-followup-only
reproducibility/clean_env/bin/python reproduce.py --all
```

Dependency installation uses the network. The replay uses saved data and needs no new inference, GPU, model weights or paid API. PDF checks need `pdflatex` with the packages loaded by the paper sources, and Poppler.

## Contents of the archive

- `paper/`: the paper, its LaTeX sources and the supplement (`paper/supplement/main.pdf`).
- `reproducibility/`: all saved model outputs, references, analysis code and frozen protocols for the news, literary, relation-extraction and DocETL experiments.
- `bc5cdr/`: the frozen protocol, the 2,480 saved requests and the offline analysis of the BC5CDR audit.
- `reporting/`: the reporting template and a filled BC5CDR example.

## Licenses

The archive combines components under different terms. See `LICENSE.md` and `LICENSES_AND_SCOPE.md`.

Earlier releases contain the same artifact with earlier wording of the paper.
