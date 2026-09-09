# Reproducing the SLR — Artificial Intelligence for DevOps Automation

**Project:** Artificial Intelligence in DevOps Automation  
**Review period:** 2016–2026  
**Search date:** 7 September 2026  
**Databases:** ScienceDirect, IEEE Xplore, ACM Digital Library  
**Methodological basis:** Kitchenham & Charters, PICOC, PRISMA 2020  
**Citation style:** IEEE  
**Current authoritative state:** 9 September 2026
**Repository synchronization:** Appendix A–E and Supplementary Dataset Master included

---

## 1. Purpose

This document explains how the main results of this Systematic Literature Review (SLR) can be reconstructed from the repository artifacts.

The intended evidence lineage is:

```text
Raw database exports
        ↓
Deduplication
        ↓
813 unique records
        ↓
Title/abstract screening
        ↓
382 reports sought for retrieval
        ↓
Full-text retrieval
        ↓
73 reports retrieved and assessed
        ↓
Full-text eligibility screening
        ↓
60 included primary studies
        ↓
Quality assessment
        ↓
26-field data extraction
        ↓
PS001–PS060 ↔ Uxxxx traceability
        ↓
RQ1–RQ5 synthesis
        ↓
PRISMA + bibliographic verification
        ↓
Publication-ready manuscript
```

This file is a **reproduction guide**, not a replacement for the SLR protocol, extraction dataset, screening workbooks, or manuscript.

---

## 2. Authoritative Project State

Before reproducing or modifying any analysis, read:

```text
00_context/SLR_CONTEXT_MASTER_2026-09-09.md
```

This is the primary source of truth for the current project state.

The following values are locked unless a new evidence-backed correction is intentionally introduced.

### 2.1 Final PRISMA accounting

| Stage | Count |
|---|---:|
| Records identified | 1,132 |
| ScienceDirect | 185 |
| IEEE Xplore | 765 |
| ACM Digital Library | 180 |
| Other/container records removed before screening | 2 |
| Bibliographic records entering deduplication | 1,130 |
| Duplicate occurrences removed | 317 |
| Unique records screened | 813 |
| Title/abstract records excluded | 431 |
| Reports sought for retrieval | 382 |
| Reports not retrieved | 309 |
| Reports retrieved / assessed | 73 |
| Full-text reports excluded | 13 |
| Studies included | 60 |

Full-text exclusion distribution:

| Code | Reason | Count |
|---|---|---:|
| FT3 | No AI/ML/GenAI/AIOps intervention | 2 |
| FT4 | MLOps only / DevOps-for-AI | 1 |
| FT5 | Secondary or non-primary publication | 7 |
| FT6 | Insufficient substantive evidence for RQs | 3 |
|  | **Total** | **13** |

### 2.2 Final RQ1 publication-year distribution

```text
2016 = 0
2017 = 0
2018 = 0
2019 = 3
2020 = 7
2021 = 4
2022 = 7
2023 = 7
2024 = 12
2025 = 8
2026 = 12
Total = 60
```

### 2.3 PS045 correction

The final resolution is:

```text
PS045 ↔ U0041
Title: ARM: Autonomous Remediation and Management With LLM Agents for Intent-Driven Control
Venue: IEEE Internet of Things Journal
Bibliographic year: 2026
DOI: 10.1109/JIOT.2025.3648858
```

The DOI / early-access timing in 2025 does **not** replace the final bibliographic issue year of 2026.

Do not restore the obsolete distribution `2025=9 / 2026=11`.

---

## 3. Repository Areas Used for Reproduction

Current repository layout relevant to the SLR:

```text
00_context/
01_protocol/
02_search/
    raw/
        sciencedirect/
        ieee/
        acm/
    log/
    derived/
03_screening/
    dedup/
    title-abstract/
    full-text/
    prism-reconciliation/
05_extraction/
06_synthesis/
    rq1/
    rq2/
    rq3/
    rq4/
    rq5/
07_prisma/
08_manuscript/
    final/
09_references/
```

> Current snapshot includes `04_quality/`, `10_supplementary/`, and `99_archive/`.

---

# 4. Reproduction Workflow

## Step 0 — Establish the authoritative context

Read:

```text
00_context/SLR_CONTEXT_MASTER_2026-09-09.md
```

Also consult the current session handoff and evidence ledger when present.

Do **not** treat older milestone files as authoritative if they conflict with the context master.

Expected final checkpoints:

```text
Included studies = 60
QA PASS = 60/60
PS↔U mapping = 60/60
Primary-study DOI coverage = 60/60
External bibliographic verification = 60/60
```

---

## Step 1 — Reconstruct the database search inputs

Raw database exports are preserved under:

```text
02_search/raw/sciencedirect/
02_search/raw/ieee/
02_search/raw/acm/
```

### ScienceDirect exports

Seven query/export groups are preserved, including:

```text
SD-01_DevOps_AI_2016-2026_2026-09-07.ris
SD-02_CICD_AI_2016-2026_2026-09-07.ris
SD-03_ContinuousIntegration_AI_2016-2026_2026-09-07.ris
SD-04_ContinuousDelivery_AI_2016-2026_2026-09-07.ris
SD-05_ContinuousDeployment_AI_2016-2026_2026-09-07.ris
SD-06_SoftwareDelivery_AI_2016-2026_2026-09-07.ris
SD-07_AIOps_2016-2026_2026-09-07.ris
```

### IEEE Xplore exports

IEEE exports are split into batches where required by export limits.

Examples:

```text
IE-01_batch01_001-100_DevOps_AI_2016-2026_2026-09-07.ris
IE-01_batch02_101-179_DevOps_AI_2016-2026_2026-09-07.ris

IE-03_batch01_001-100_Continuous_Integration_2016-2026_2026-09-07.ris
IE-03_batch02_101-159_Continuous_Integration_2016-2026_2026-09-07.ris

IE-07_batch01_001-100_AIOps_2016-2026_2026-09-07.ris
IE-07_batch02_101-184_AIOps_2016-2026_2026-09-07.ris
```

Two current filenames contain a duplicated extension:

```text
IE-02_batch01_001-100_CICD_AI_2016-2026_2026-09-07.ris.ris
IE-02_batch02_101-129_CICD_AI_2016-2026_2026-09-07.ris.ris
```

These should be normalized to `.ris` when repository cleanup is performed. This is a filename hygiene issue only; do not alter the record contents during renaming.

### ACM Digital Library exports

Seven query/export groups are preserved:

```text
ACM-01_DevOps_AI_2016-2026_2026-09-07.ris
...
ACM-07_AIOps_2016-2026_2026-09-07.ris
```

### Search logs

Operational search notes are stored under:

```text
02_search/logs/
```

Current files:

```text
Search Log ACM (Chatgpt).txt
Search Log IEEE Xplore (Chatgpt).txt
Search Log ScienceDirect (Chatgpt).txt
```

Use these logs to recover database-specific execution details where available.

### Expected identification total

The final manuscript-level accounting is:

```text
ScienceDirect = 185
IEEE Xplore = 765
ACM Digital Library = 180
Database records = 1,130
Other/container records removed before screening = 2
Displayed records identified = 1,132
```

Do not infer record counts from filename ranges alone. Validate against the deduplication workbook and final PRISMA reconciliation.

---

## Step 2 — Reproduce deduplication

Primary artifact:

```text
03_screening/dedup/SLR_Master_Deduplication_2026-09-07.xlsx
```

Target reconciliation:

```text
Records entering deduplication = 1,130
Duplicate occurrences removed = 317
Unique records = 813
```

Check:

```text
1,130 - 317 = 813
```

The 813 unique records form the authoritative input to title/abstract screening.

If reconstructing deduplication programmatically, preserve the original workbook before applying any normalization or duplicate-detection changes. Different DOI/title normalization rules may otherwise create a different duplicate count.

---

## Step 3 — Reproduce title/abstract screening

Primary artifact:

```text
03_screening/title-abstract/SLR_Master_Maybe_Resolved_813_2026-09-08.xlsx
```

Input:

```text
813 unique records
```

Final result:

```text
Title/abstract excluded = 431
Reports sought for retrieval = 382
```

Check:

```text
813 - 431 = 382
```

The 382 records are the retrieval cohort.

The review boundary is:

> Include AI-for-DevOps studies. Exclude MLOps-only / DevOps-for-AI studies unless AI is explicitly used to improve a DevOps activity.

Do not silently reclassify records using a broader AI/software-engineering definition.

---

## Step 4 — Reproduce full-text retrieval

Primary artifacts:

```text
03_screening/full-text/SLR_Master_FullText_Screening_Ready_382_2026-09-08.xlsx
03_screening/prism-reconciliation/SLR_Master_PRISMA_Reconciliation_382_2026-09-08_FINAL.xlsx
```

Retrieval was attempted for all:

```text
382 reports
```

Final retrieval result:

```text
Retrieved / assessed = 73
Not retrieved = 309
```

Check:

```text
382 - 309 = 73
```

The 309 records must remain classified as:

```text
Reports not retrieved
```

They must **not** be recoded as full-text exclusions because eligibility assessment was not completed on unavailable full texts.

---

## Step 5 — Reproduce full-text eligibility screening

Primary artifact:

```text
03_screening/full-text/Full-Text Screening_73total.xlsx
```

Recovered included-study identity artifact:

```text
03_screening/full-text/SLR_60_Included_Uxxxx_RECOVERED_2026-09-09.xlsx
```

Input:

```text
73 retrieved reports
```

Outcome:

```text
Included = 60
Excluded = 13
```

Check:

```text
73 - 13 = 60
```

Final exclusion distribution:

```text
FT3 = 2
FT4 = 1
FT5 = 7
FT6 = 3
Total = 13
```

Cross-check the same counts against:

```text
07_prisma/SLR_PRISMA_RECONCILIATION_WORKSHEET_2026-09-08.md
```

and:

```text
03_screening/prism-reconciliation/SLR_Master_PRISMA_Reconciliation_382_2026-09-08_FINAL.xlsx
```

---

## Step 6 — Reconstruct the 60-study identity set

Primary study identity is based on two identifier systems:

```text
Uxxxx = unique record identifier from the screening/retrieval workflow
PS001–PS060 = manuscript/extraction primary-study identifier
```

Final mapping artifact:

```text
05_extraction/SLR_PS001-PS060_Uxxxx_FULL_EXACT_MAPPING_FINAL_2026-09-09.xlsx
```

Required integrity condition:

```text
60 PS IDs
60 included U IDs
one-to-one mapping
no duplicate PS
no duplicate U
```

Expected:

```text
PS001–PS060 ↔ Uxxxx = 60/60
```

### Recovery exception

The recovered extraction master previously duplicated:

```text
Commit Artifact Preserving Build Prediction
```

into PS009 and PS047.

The final resolution is:

```text
PS047 → U0459
PS009 → U0669
```

PS009 resolves to:

```text
Predicting build outcomes in continuous integration using textual analysis of source code commits
```

Do not regenerate the mapping by relying only on duplicated recovered titles.

---

## Step 7 — Reproduce quality assessment

Final QA status:

```text
60/60 assessed
60 PASS
0 FAIL
Threshold = >= 3.0 / 5
```

QA dimensions:

```text
QA1 — Research objective is clear
QA2 — DevOps + AI relevance is clear
QA3 — Method/evaluation is adequate
QA4 — Results are evidence-supported
QA5 — Limitations/threats/implications are reported
```

Scoring model:

```text
Yes     = 1.0
Partial = 0.5
No      = 0.0
PASS    = total score >= 3.0
```

Important interpretation:

> QA PASS is an inclusion-quality threshold. It does not mean all included studies have equal evidence strength.

The dedicated QA protocol artifact is stored at:

```text
04_quality/QA_CRITERIA_AND_SCORING_FINAL_2026-09-09.md
```

Exact paper-level numeric QA scores remain unrecovered; the canonical extraction preserves PASS status only.

---

## Step 8 — Reproduce data extraction

Canonical extraction artifact:

```text
05_extraction/SLR_Data_Extraction_60_Studies_26Fields_FINAL_2026-09-09.xlsx
```

The final extraction schema contains **26 fields**:

```text
Paper ID
Authors
Year
Title
Source Database
Venue
Publication Type
Research Type
DevOps Stage
DevOps Activity
AI Category
AI Method/Model
Dataset/System
Research Objective
Evaluation Method
Metrics
Main Findings
Benefits
Challenges
Limitations
Future Work
RQ Mapping
QA Score
Industrial Context
Evidence Type
Evidence Strength
```

Evidence-strength categories:

```text
Production
Industrial Empirical
Controlled Experimental
Benchmark
Simulation
Conceptual
```

Recommended repository cleanup:

```text
05_extraction/SLR_Data_Extraction_60_Studies_26Fields_FINAL_2026-09-09.xlsx
```

should remain preserved, while a normalized authoritative export should be created, for example:

```text
05_extraction/SLR_Data_Extraction_60_Studies_26Fields_FINAL_2026-09-09.xlsx
```

Do not destroy or overwrite the recovered source workbook when producing the normalized final copy.

---

# 5. Reproducing the Research Questions

## RQ1 — Research trends, 2016–2026

Primary synthesis artifact:

```text
06_synthesis/rq1/RQ1_Final_Publication_Trend_AI_DevOps_2016-2026.xlsx
```

Required final distribution:

| Year | Studies |
|---|---:|
| 2016 | 0 |
| 2017 | 0 |
| 2018 | 0 |
| 2019 | 3 |
| 2020 | 7 |
| 2021 | 4 |
| 2022 | 7 |
| 2023 | 7 |
| 2024 | 12 |
| 2025 | 8 |
| 2026 | 12 |
| **Total** | **60** |

Interpretive trajectory:

```text
Predictive AI
→ Diagnostic AIOps
→ Generative AI
→ Agentic AI
```

PS045 must be counted under 2026.

---

## RQ2 — DevOps stages and application areas

Primary synthesis artifact:

```text
06_synthesis/rq2/RQ2_Final_DevOps_Stages_and_Application_Areas_AI_DevOps_2016-2026.xlsx
```

Final counts:

| DevOps stage/activity | Studies | Share |
|---|---:|---:|
| Monitor / Observability | 35 | 58.3% |
| Operate / Operations | 31 | 51.7% |
| Incident / RCA / Remediation | 17 | 28.3% |
| Test | 16 | 26.7% |
| Build / CI | 10 | 16.7% |
| Deploy / Release | 9 | 15.0% |
| Develop / Code / IaC | 3 | 5.0% |
| AIOps Model Governance | 3 | 5.0% |
| Human / Cross-cutting | 1 | 1.7% |

These categories are multi-label. Their counts are therefore **not expected to sum to 60**.

Core interpretation:

```text
Monitor → Operate → Incident/RCA
```

Automation lens:

```text
Assist → Predict → Diagnose → Recommend → Act
```

---

## RQ3 — AI techniques, methods, and technologies

Primary synthesis artifact:

```text
06_synthesis/rq3/RQ3_Final_AI_Taxonomy_and_Methods_DevOps_2016-2026.xlsx
```

Final primary-category distribution:

| AI category | Count |
|---|---:|
| Classical ML | 27 |
| Deep Learning | 8 |
| Unsupervised / Anomaly AI | 6 |
| Optimization & RL | 3 |
| NLP / Representation | 4 |
| GenAI / LLM | 7 |
| Agentic / Multi-Agent | 5 |
| **Total** | **60** |

Interpretive progression:

```text
Model
→ Pipeline
→ Reasoning System
→ Agentic System
```

Important taxonomy rule:

> AIOps is treated as an application paradigm, not as an algorithm class.

---

## RQ4 — Benefits and impacts

Primary synthesis artifact:

```text
06_synthesis/rq4/RQ4_Final_Benefits_Impacts_Evidence_Anchors_AI_DevOps_2016-2026.xlsx
```

Benefit taxonomy:

```text
B1 — Speed & Efficiency
B2 — Accuracy & Detection Quality
B3 — Reliability & Availability
B4 — Cost & Resource Optimization
B5 — Automation & Toil Reduction
B6 — Security Improvement
B7 — Human Decision Support & Productivity
```

Core interpretation:

> Technical capability is developing faster than demonstrated production benefit, especially for LLM and agentic approaches.

### Important restriction

Do **not** report corpus-wide B1–B7 prevalence unless a complete record-level recoding is explicitly performed and stored as a reproducible derived dataset.

The current locked manuscript does not claim reproducible corpus-wide B1–B7 frequencies.

---

## RQ5 — Challenges, gaps, and future research

Primary synthesis artifact:

```text
06_synthesis/rq5/RQ5_Final_Challenges_Gaps_Future_Research_AI_DevOps_2016-2026.xlsx
```

Final gap taxonomy:

```text
G1 — Production-scale validation
G2 — Cross-system generalization
G3 — Concept drift & long-term maintenance
G4 — Explainability / trust / reliability
G5 — Autonomous-remediation safety
G6 — LLM / agent cost & latency
G7 — Human–AI collaboration & adoption
G8 — Unified ML + DevOps operational evaluation
```

Future research agenda:

```text
FR1 — Production-Validated AI-for-DevOps
FR2 — Adaptive and Generalizable AIOps
FR3 — Trustworthy and Explainable LLM-AIOps
FR4 — Safe and Cost-Efficient Agentic DevOps
FR5 — Human-Centered Autonomous DevOps
```

Long-term trajectory:

```text
Predictive
→ Diagnostic
→ Generative
→ Agentic
→ Trustworthy Autonomous DevOps
```

---

# 6. Reproduce the PRISMA Figure

Authoritative figure:

```text
07_prisma/PRISMA-2020-F_AI_DevOps_AUTHORITATIVE.svg
```

Supporting reconciliation artifact:

```text
07_prisma/SLR_PRISMA_RECONCILIATION_WORKSHEET_2026-09-08.md
```

Primary reconciliation workbook:

```text
03_screening/prism-reconciliation/SLR_Master_PRISMA_Reconciliation_382_2026-09-08_FINAL.xlsx
```

Before accepting any regenerated PRISMA figure, confirm all of the following:

```text
1,132 identified
1,130 entering deduplication
317 duplicate occurrences removed
813 screened
431 title/abstract exclusions
382 sought
309 not retrieved
73 assessed
13 full-text exclusions
60 included
```

Consistency equations:

```text
1,130 - 317 = 813
813 - 431 = 382
382 - 309 = 73
73 - 13 = 60
```

The SVG in `07_prisma/` is the authoritative publication figure unless a deliberate corrected replacement is created.

---

# 7. Reproduce Bibliographic Traceability

Primary reference artifacts:

```text
09_references/SLR_Final_Citation_Integrity_Audit_2026-09-09.xlsx
09_references/SLR_Final_PS_to_IEEE_Mapping_7-66_2026-09-09.xlsx
09_references/SLR_Primary_Study_Reference_Ledger_EXTERNAL_VERIFICATION_COMPLETE_2026-09-09.xlsx
```

Expected final state:

```text
Background references = [1]–[6]
Primary-study references = [7]–[66]
Primary-study DOI coverage = 60/60
External bibliographic verification = 60/60
Citation integrity = PASS
```

The `PS001–PS060` identifiers should remain traceability identifiers and must not replace IEEE citations in narrative manuscript text.

---

# 8. Reproduce the Final Manuscript State

Final manuscript artifacts:

```text
08_manuscript/final/SLR_AI_DevOps_Consolidated_FINAL_CITATIONS_2026-09-09.docx
08_manuscript/final/SLR_AI_DevOps_PUBLICATION_READY_FINAL_2026-09-09.docx
```

The publication-ready manuscript is the current preferred final manuscript:

```text
SLR_AI_DevOps_PUBLICATION_READY_FINAL_2026-09-09.docx
```

Locked manuscript components:

```text
Abstract + Keywords
Section 1 — Introduction
Section 2 — Background
Section 3 — Research Methodology
Section 4 — Results
Section 5 — Discussion
Section 6 — Threats to Validity
Section 7 — Conclusion
PRISMA figure
IEEE citations [1]–[66]
References
PS045 year = 2026
```

Do not reopen these sections merely because an older intermediate file contains conflicting values.

A manuscript correction should only be made when backed by:

1. identifiable record-level evidence;
2. an updated authoritative dataset or reconciliation artifact;
3. a documented change in the context master;
4. downstream consistency checks.

---

# 9. Reproduction Integrity Checklist

A successful reproduction should satisfy all checks below.

## Search and screening

- [ ] Raw RIS exports are preserved unchanged.
- [ ] Database record total reconciles to 1,130.
- [ ] Deduplication yields 813 unique records.
- [ ] Title/abstract screening yields 382 retrieval candidates.
- [ ] Retrieval accounting yields 73 retrieved and 309 not retrieved.
- [ ] Full-text screening yields 60 included and 13 excluded.
- [ ] FT3 + FT4 + FT5 + FT6 = 13.

## Study identity

- [ ] Included U IDs = 60.
- [ ] PS IDs = PS001–PS060.
- [ ] PS↔U mapping is one-to-one.
- [ ] PS009 resolves to U0669.
- [ ] PS047 resolves to U0459.
- [ ] PS045 resolves to U0041.
- [ ] PS045 bibliographic year = 2026.

## QA and extraction

- [ ] QA assessed = 60/60.
- [ ] QA PASS = 60.
- [ ] QA FAIL = 0.
- [ ] Extraction includes 60 studies.
- [ ] Extraction schema contains 26 fields.

## RQ synthesis

- [ ] RQ1 sums to 60.
- [ ] RQ1 uses 2025=8 and 2026=12.
- [ ] RQ2 is treated as multi-label.
- [ ] RQ3 primary categories sum to 60.
- [ ] RQ4 does not claim unsupported corpus-wide prevalence.
- [ ] RQ5 uses evidence-backed gaps and future agenda.

## Bibliography

- [ ] 60 primary studies map to IEEE references [7]–[66].
- [ ] DOI coverage = 60/60.
- [ ] External verification = 60/60.
- [ ] Citation integrity audit passes.

## Manuscript

- [ ] Final PRISMA numbers match the data lineage.
- [ ] Section 4 RQ1 values match the final RQ1 workbook.
- [ ] No obsolete PS045 uncertainty remains.
- [ ] No obsolete `2025=9 / 2026=11` counts remain.

---

# 10. Known Historical / Recovery Hazards

The repository contains or may contain historical artifacts created before final reconciliation.

Examples of obsolete states include:

```text
PS045 unresolved or provisional = 2025
2025 = 9
2026 = 11
PRISMA retrieval reconciliation pending
manuscript not yet final
```

These were valid interim states but are **not current results**.

Recommended repository policy:

```text
00_context/      → current authoritative project state
99_archive/      → superseded milestones, intermediate recovery artifacts,
                   and obsolete versions retained for provenance
```

Historical files should never override:

```text
00_context/SLR_CONTEXT_MASTER_2026-09-09.md
```

unless a newer context master explicitly supersedes it.

---

# 11. Recommended File Classification

Use the following semantics when adding or renaming files.

| Class | Meaning |
|---|---|
| `raw` | Original export/data; no analytical modification |
| `derived` | Produced from one or more source artifacts |
| `recovered` | Reconstructed after missing/incomplete earlier state |
| `final` | Validated analytical artifact |
| `authoritative` | Current canonical source for a specific result |
| `superseded` | Historical artifact replaced by a newer authoritative version |

Do not overwrite raw or recovered source artifacts to make them look final. Create a new validated final copy instead.

---

# 12. Current Protocol and Supplementary Artifacts

The current repository includes the finalized supporting protocol artifacts:

```text
01_protocol/SLR_SEARCH_STRATEGY_FINAL_2026-09-09.md
01_protocol/SLR_STUDY_SELECTION_PROTOCOL_FINAL_2026-09-09.md
01_protocol/SLR_DATA_EXTRACTION_AND_CODING_FRAMEWORK_FINAL_2026-09-09.md
04_quality/QA_CRITERIA_AND_SCORING_FINAL_2026-09-09.md
```

Appendix artifacts:

```text
10_supplementary/appendices/APPENDIX_A_SEARCH_STRATEGY_2026-09-09.md
10_supplementary/appendices/APPENDIX_B_STUDY_SELECTION_PROTOCOL_2026-09-09.md
10_supplementary/appendices/APPENDIX_C_QUALITY_ASSESSMENT_2026-09-09.md
10_supplementary/appendices/APPENDIX_D_INCLUDED_PRIMARY_STUDIES_2026-09-09.md
10_supplementary/appendices/APPENDIX_E_DATA_EXTRACTION_AND_CODING_FRAMEWORK_2026-09-09.md
```

Canonical supplementary datasets:

```text
10_supplementary/datasets/SLR_INCLUDED_PRIMARY_STUDIES_60_FINAL_2026-09-09.xlsx
10_supplementary/datasets/SLR_SUPPLEMENTARY_DATASET_MASTER_2026-09-09.xlsx
```

The master supplementary workbook consolidates the audit views for primary studies, QA, 26-field extraction, PS↔U mapping, RQ1–RQ5, and PRISMA. It does not replace the original raw or stage-specific source artifacts.

---

# 13. Minimal Recovery Procedure for a New Session

If work must continue in a new ChatGPT session or after local recovery, provide at minimum:

```text
00_context/SLR_CONTEXT_MASTER_2026-09-09.md
00_context/SLR_SESSION_HANDOFF_2026-09-09.md
README.md
REPRODUCE.md
```

For evidence-sensitive modifications, also provide the artifact relevant to the requested layer.

Examples:

```text
PRISMA correction
→ PRISMA reconciliation workbook + worksheet

RQ1 correction
→ extraction master + PS↔U mapping + RQ1 workbook

Bibliographic correction
→ PS↔IEEE mapping + reference ledger + citation audit

Manuscript correction
→ publication-ready DOCX + authoritative supporting dataset
```

Do not rely on context summaries alone for record-level corrections.

---

# 14. Reproducibility Boundary

This repository is designed to preserve the analytical trail and allow the review decisions, counts, coding, synthesis, and manuscript results to be audited or reconstructed.

Some full-text primary-study PDFs may be retained only in a private/local Zotero or research archive because publisher copyright or redistribution terms may prevent committing them to a public repository.

Reproduction should therefore distinguish between:

```text
Bibliographic/search reproducibility
Screening-decision reproducibility
Extraction/coding reproducibility
Synthesis reproducibility
Full-text redistribution
```

The first four can be supported by repository artifacts. The fifth depends on the licensing and access conditions of each publication.

---

# 15. Final Reproduction Target

The reproduction is considered successful when the repository independently supports the following final chain:

```text
1,132 identified
    ↓
1,130 bibliographic records entering deduplication
    ↓
813 unique records
    ↓
382 reports sought
    ↓
73 reports retrieved and assessed
    ↓
60 included primary studies
    ↓
60/60 QA PASS
    ↓
60-study, 26-field extraction
    ↓
60/60 PS↔U mapping
    ↓
RQ1–RQ5 final synthesis
    ↓
60/60 DOI and bibliographic verification
    ↓
PRISMA authoritative figure
    ↓
SLR_AI_DevOps_PUBLICATION_READY_FINAL_2026-09-09.docx
```

Any future modification that changes this chain should be treated as a **controlled correction** and documented across the affected source dataset, derived artifact, context master, and manuscript.

---

**End of reproduction guide.**
