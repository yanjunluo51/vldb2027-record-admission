# Component notices and distribution scope

This is the reproducibility artifact for the conference paper. The authors decided on 22 November 2026 to publish this complete package, including all saved hosted-model outputs, in a public archival repository together with the initial submission. Component licenses, attribution and noncommercial restrictions apply separately. Packaging does not create new rights over third-party data, models or dependencies.

| Component | Retained source/notice | Scope of this check |
|---|---|---|
| Code written for the study | `reproducibility/private_staging/original/vldbj_repo/LICENSE` | Existing MIT statement explicitly covers study code and excludes third-party data/models/dependencies; no blanket MIT label is applied to the mixed artifact. |
| German news and study-derived records | Original `DATA_LICENSES.md`, `public_workload_replay/sources/german_news/LICENSE` and source README | Retained CC BY-NC-SA 4.0 attribution; data and references were not changed. |
| LitBank | Added unchanged upstream README under `workbench/source_notices`; original `DATA_LICENSES.md`; source-note explanation below | Both differing upstream wordings are retained; neither is silently replaced. |
| REDEWIEDERGABE | Added unchanged fixed-commit README under `workbench/source_notices`; original data terms and conversion code | Official README states CC BY-NC-SA 4.0; the fixed source tree and README blob were verified. |
| Re-DocRED and DocRED ontology | `relation_extension/source/LICENSE`, `DocRED_LICENSE`, and `RELEASE_NOTICES_ADDENDUM.md` | Separate original MIT notices retained. The ontology addendum supplies the verified source route; the unresolved historical commit is not treated as verified. |
| DocETL / SemBench | Workbench `THIRD_PARTY_NOTICES.md` and original upstream MIT/Apache notices | Preserve fixed-commit code and metric provenance; these licenses do not grant rights to every external dataset mentioned by those projects. |
| German specialist implementation | Original `german_specialist/upstream/LICENSE` | Upstream MIT notice retained unchanged. |
| VLDB template | Original template headers and README | No template changes or new license assertions. |
| Descriptive pilot coordinates | `workbench/pilot_descriptive_evidence/README.md` | Pseudonymous old comparison only. No raw student workbooks, names, source text or free comments. The later adjudicated scenarios are in `workbench/results/e62_adjudicated_reference/`. |

Paths in the table are relative to `reproducibility/private_staging/` where abbreviated. Original frozen records stay byte-identical. This review did not establish the historical download event, authorship of annotations, or blanket legal clearance for all uses.

## LitBank: retain both source statements

The fixed repository README at commit `3e50db0ffc033d7ccbb94f4d88f6b99210328ed8` states CC BY 4.0:
https://github.com/dbamman/litbank/blob/3e50db0ffc033d7ccbb94f4d88f6b99210328ed8/README.md .

The quotation-data paper (Sims and Bamman, 2020, Section 3.2) uses the phrase “Creative Commons ShareAlike 4.0”:
https://aclanthology.org/2020.emnlp-main.47/ .

The study's existing DATA_LICENSES.md assigns CC BY-SA 4.0 to its LitBank-derived files and describes this as satisfying both notices. Treat that as the study's stated handling of derived contributions, not proof that the two upstream descriptions are identical or that this review recovered an otherwise undocumented grant. Preserve original attribution, both source descriptions and the indication of changes (coordinate conversion, speaker projection and predictions). Do not place the whole mixed-data bundle under a single license.

License texts: https://creativecommons.org/licenses/by/4.0/legalcode.en and https://creativecommons.org/licenses/by-sa/4.0/legalcode.en .

## REDEWIEDERGABE

Fixed source: https://github.com/redewiedergabe/corpus/tree/45abfcf5f9c2a3d9a903f5c68f8f5b36bbce5563 . The unchanged README is included, rather than replacing its attribution with a local paraphrase. The original TSV files are not newly added. Existing reconstructed units and saved analyses remain as previously preserved.

## What is outside this candidate

No literature full-text review cache, raw student returns, cloud billing records or API credentials are added. BC5CDR now includes 2,480 actual saved requests and their offline analysis. Its original corpus public-domain notice is retained under `bc5cdr/protocol/independent_audit/sources/`. Model weights are not redistributed. Training qualification, development choice and test records retain the frozen boundaries. Older absolute paths in preserved failure logs are historical provenance. Run `configure_paths.py` after moving the folder; the offline CPU workflow has already been checked without the external original disk.

Only the CPU commands in README.md form the supported replay path. Historical acquisition scripts are retained for provenance; they are not invoked by that path, do not establish current model access, and should not be confused with a newly executed generation experiment.

## Derived annotation stress inputs

`reproducibility/supplement_inputs/scenario_inputs.json` contains public source text with its existing data license, pseudonymous document IDs, span coordinates and discourse types. S2/S3 are the two original student returns. The adjudicated scenarios of 22 November 2026 are in `workbench/results/e62_adjudicated_reference/`. Raw student spreadsheets, names, free-text replies and coordinator reports are excluded. The descriptive overlap snapshot contains only hashes, lengths, coordinates and types. Its arithmetic is reproducible but does not verify authorship, semantic correctness or independence. Do not send reference-containing materials to participants whose blinded judgments remain pending.

The directory name `private_staging` is retained solely for compatibility with the existing replay scripts. It is not an instruction to publish the private parent workbench. Only this separately screened distribution candidate is in scope. Historical frozen text may describe earlier preparation states. Current status is in the root README and verification receipts.

## Output distribution

The authors decided on 22 November 2026 to publish this complete package, including all saved hosted-model outputs, in a public archival repository together with the initial submission. `OUTPUT_TERMS_REVIEW.md` records the primary-source checks of the provider terms and this decision.
