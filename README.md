# magister-teknologi-informasi

Catatan, dataset kerja, dokumentasi, dan artefak reproduksi untuk proyek
**Systematic Literature Review (SLR)** bidang Software Engineering
dengan fokus **Artificial Intelligence for DevOps Automation**.

## Final working title

> **Artificial Intelligence in DevOps Automation: A Systematic
> Literature Review of Applications, Benefits, Challenges, and Research
> Trends from 2016 to 2026**

## Scope & methodology

-   Domain: Software Engineering
-   Boundary: **AI-for-DevOps**, excluding MLOps-only / DevOps-for-AI
-   Period: 2016--2026
-   Search date: 7 September 2026
-   Databases: ScienceDirect, IEEE Xplore, ACM Digital Library
-   Methodological basis: Kitchenham & Charters + PICOC + PRISMA 2020
-   Citation style: IEEE
-   Synthesis: descriptive quantitative + qualitative thematic
-   Statistical meta-analysis: no

## Current status --- 9 September 2026

  Phase                             Status
  --------------------------------- ----------------------------------
  Search strategy / protocol        ✅ Final operational record
  Deduplication                     ✅ Complete
  Title/abstract screening          ✅ Complete
  Full-text retrieval / screening   ✅ Complete / reconciled
  Quality Assessment                ✅ 60/60 PASS
  Data Extraction                   ✅ 60/60, 26 fields
  PS↔U Mapping                      ✅ 60/60
  RQ1--RQ5 synthesis                ✅ Locked
  PRISMA                            ✅ Locked
  Bibliographic verification        ✅ 60/60
  Manuscript Sections 1--7          ✅ Locked
  IEEE references                   ✅ \[1\]--\[66\]
  Appendix A--E                     ✅ Complete
  Supplementary Dataset Master      ✅ Complete
  Repository synchronization        🔄 Final release synchronization
  Visual publication-ready DOCX     ✅ Final / QA PASS
  Visual publication-ready PDF      ✅ Final / QA PASS
  Submission-template formatting    ⏳ Optional / venue-specific

## Locked PRISMA accounting

``` text
Records identified                              1,132
  ScienceDirect                                   185
  IEEE Xplore                                     765
  ACM Digital Library                             180
Other/container records removed                     2
Records entering deduplication                  1,130
Duplicate occurrences removed                     317
Records screened                                  813
Title/abstract excluded                           431
Reports sought for retrieval                      382
Reports not retrieved                             309
Reports retrieved / assessed                       73
Full-text excluded                                 13
Studies included                                   60
```

Full-text exclusions:

``` text
FT3 = 2
FT4 = 1
FT5 = 7
FT6 = 3
Total = 13
```

## Locked synthesis anchors

### RQ1

``` text
2016=0
2017=0
2018=0
2019=3
2020=7
2021=4
2022=7
2023=7
2024=12
2025=8
2026=12
Total=60
```

PS045 is final = **2026**.

Trajectory: **Predictive AI → Diagnostic AIOps → Generative AI → Agentic
AI**.

### RQ2

Monitor/Observability 35; Operate 31; Incident/RCA/Remediation 17; Test
16; Build/CI 10; Deploy/Release 9; Develop/Code/IaC 3; AIOps Model
Governance 3; Human/Cross-cutting 1.

RQ2 is multi-label; counts are not expected to sum to 60.

### RQ3

Classical ML 27; Deep Learning 8; Unsupervised/Anomaly AI 6;
Optimization & RL 3; NLP/Representation 4; GenAI/LLM 7;
Agentic/Multi-Agent 5.

RQ3 final distribution uses one normalized primary AI category per
study.

### RQ4

Benefit themes B1--B7 are qualitative synthesis themes. **Do not report
corpus-wide B1--B7 prevalence** without complete record-level recoding.

Core interpretation: **technical capability is developing faster than
demonstrated production benefit**.

### RQ5

Research gaps: G1 Production-scale validation; G2 Cross-system
generalization; G3 Concept drift & long-term maintenance; G4
Explainability/trust/reliability; G5 Autonomous-remediation safety; G6
LLM/agent cost & latency; G7 Human--AI collaboration/adoption; G8
Unified ML + DevOps operational evaluation.

Future agenda: FR1 Production-Validated AI-for-DevOps; FR2 Adaptive and
Generalizable AIOps; FR3 Trustworthy and Explainable LLM-AIOps; FR4 Safe
and Cost-Efficient Agentic DevOps; FR5 Human-Centered Autonomous DevOps.

## Repository navigation

``` text
magister-teknologi-informasi/
├── README.md
├── REPRODUCE.md
├── 00_context/
├── 01_protocol/
├── 02_search/
│   ├── raw/
│   ├── logs/
│   └── derived/
├── 03_screening/
│   ├── dedup/
│   ├── title-abstract/
│   ├── full-text/
│   └── prism-reconciliation/
├── 04_quality/
├── 05_extraction/
├── 06_synthesis/
│   ├── rq1/
│   ├── rq2/
│   ├── rq3/
│   ├── rq4/
│   └── rq5/
├── 07_prisma/
├── 08_manuscript/
│   └── final/
├── 09_references/
├── 10_supplementary/
│   ├── appendices/
│   └── datasets/
├── release/
│   └── 2026-09-09/
└── 99_archive/
```

## Current authoritative artifacts

### Context

``` text
00_context/SLR_CONTEXT_MASTER_2026-09-09.md
00_context/SLR_SESSION_HANDOFF_2026-09-09.md
00_context/SLR_EVIDENCE_SYNTHESIS_LEDGER_2026-09-09.md
00_context/REPOSITORY_MANIFEST_SLR_2026-09-09.md
00_context/FINAL_VISUAL_QA_REPORT_2026-09-09.md
```

### Protocol / QA

``` text
01_protocol/SLR_SEARCH_STRATEGY_FINAL_2026-09-09.md
01_protocol/SLR_STUDY_SELECTION_PROTOCOL_FINAL_2026-09-09.md
01_protocol/SLR_DATA_EXTRACTION_AND_CODING_FRAMEWORK_FINAL_2026-09-09.md
04_quality/QA_CRITERIA_AND_SCORING_FINAL_2026-09-09.md
```

### Extraction / traceability

``` text
05_extraction/SLR_Data_Extraction_60_Studies_26Fields_FINAL_2026-09-09.xlsx
05_extraction/SLR_PS001-PS060_Uxxxx_FULL_EXACT_MAPPING_FINAL_2026-09-09.xlsx
```

### PRISMA

``` text
07_prisma/PRISMA-2020-F_AI_DevOps_AUTHORITATIVE.svg
07_prisma/SLR_PRISMA_RECONCILIATION_WORKSHEET_2026-09-09.md
03_screening/prism-reconciliation/SLR_Master_PRISMA_Reconciliation_382_2026-09-08_FINAL.xlsx
```

### Manuscript --- authoritative publication artifacts

``` text
08_manuscript/final/SLR_AI_DevOps_VISUAL_PUBLICATION_READY_FINAL_2026-09-09.docx
08_manuscript/final/SLR_AI_DevOps_VISUAL_PUBLICATION_READY_FINAL_2026-09-09.pdf
```

The visual publication-ready DOCX is the **authoritative editable
manuscript**, and the corresponding PDF is the **authoritative
publication rendering** for the current evidence state.

### Manuscript --- pre-visual baseline / rollback

``` text
08_manuscript/final/SLR_AI_DevOps_PUBLICATION_READY_FINAL_2026-09-09.docx
```

This file is retained as the pre-visual publication baseline for
provenance and rollback. It must not override the visual
publication-ready manuscript above.

### References

``` text
09_references/SLR_Primary_Study_Reference_Ledger_EXTERNAL_VERIFICATION_COMPLETE_2026-09-09.xlsx
09_references/SLR_Final_PS_to_IEEE_Mapping_7-66_2026-09-09.xlsx
09_references/SLR_Final_Citation_Integrity_Audit_2026-09-09.xlsx
```

### Appendices

``` text
10_supplementary/appendices/APPENDIX_A_SEARCH_STRATEGY_2026-09-09.md
10_supplementary/appendices/APPENDIX_B_STUDY_SELECTION_PROTOCOL_2026-09-09.md
10_supplementary/appendices/APPENDIX_C_QUALITY_ASSESSMENT_2026-09-09.md
10_supplementary/appendices/APPENDIX_D_INCLUDED_PRIMARY_STUDIES_2026-09-09.md
10_supplementary/appendices/APPENDIX_E_DATA_EXTRACTION_AND_CODING_FRAMEWORK_2026-09-09.md
```

### Supplementary datasets

``` text
10_supplementary/datasets/SLR_INCLUDED_PRIMARY_STUDIES_60_FINAL_2026-09-09.xlsx
10_supplementary/datasets/SLR_SUPPLEMENTARY_DATASET_MASTER_2026-09-09.xlsx
```

## Visual publication QA

The visual-publication pass is presentation-only and does not alter the
locked analytical substance.

Current QA record:

``` text
00_context/FINAL_VISUAL_QA_REPORT_2026-09-09.md
```

The final visual QA covers the rendered manuscript, figure/table
presentation, page layout, accessibility checks, and preservation of the
locked SLR content. The visual-publication version remains governed by
the same PRISMA accounting, study identities, RQ synthesis, QA rules,
references, and conclusions documented in the authoritative evidence
artifacts.

## Source-of-truth rules

1.  `README.md` is the current navigation/overview.
2.  `00_context/SLR_CONTEXT_MASTER_2026-09-09.md` is the dense
    authoritative project state.
3.  `00_context/SLR_SESSION_HANDOFF_2026-09-09.md` is the compact
    recovery context for a new session.
4.  `REPRODUCE.md` describes the evidence lineage and reproduction
    workflow.
5.  Raw RIS exports under `02_search/raw/` are immutable.
6.  Record-level screening/extraction workbooks remain the source of
    truth for study-level decisions.
7.  The supplementary master is an audit/convenience package; it does
    not replace raw or stage-specific source artifacts.
8.  `08_manuscript/final/SLR_AI_DevOps_VISUAL_PUBLICATION_READY_FINAL_2026-09-09.docx`
    is the authoritative editable manuscript.
9.  `08_manuscript/final/SLR_AI_DevOps_VISUAL_PUBLICATION_READY_FINAL_2026-09-09.pdf`
    is the authoritative publication rendering.
10. `08_manuscript/final/SLR_AI_DevOps_PUBLICATION_READY_FINAL_2026-09-09.docx`
    is retained only as the pre-visual baseline / rollback artifact.
11. `00_context/FINAL_VISUAL_QA_REPORT_2026-09-09.md` records the final
    visual QA state.
12. Files under `99_archive/` are historical and must not override
    current authoritative artifacts.
13. Do not restore obsolete PS045 uncertainty or RQ1 counts
    `2025=9 / 2026=11`.
14. Do not invent unrecovered exact numeric QA scores.
15. Visual/layout revisions must not be interpreted as changes to the
    locked analytical SLR unless an explicit substantive revision is
    documented.

## Reproduction

Start with:

``` text
REPRODUCE.md
```

Minimal new-session recovery package:

``` text
README.md
REPRODUCE.md
00_context/SLR_CONTEXT_MASTER_2026-09-09.md
00_context/SLR_SESSION_HANDOFF_2026-09-09.md
```

For verification of the final publication rendering, also supply:

``` text
00_context/FINAL_VISUAL_QA_REPORT_2026-09-09.md
08_manuscript/final/SLR_AI_DevOps_VISUAL_PUBLICATION_READY_FINAL_2026-09-09.docx
08_manuscript/final/SLR_AI_DevOps_VISUAL_PUBLICATION_READY_FINAL_2026-09-09.pdf
```

For record-level correction, also supply the corresponding source
workbook.

## Remaining work

The analytical SLR, manuscript body, Appendices A--E, supplementary
master dataset, visual publication-ready manuscript, publication PDF,
and final visual QA are complete for the current evidence state.

Remaining work is release/submission administration only:

-   synchronize `REPRODUCE.md` with the visual-final authoritative
    artifacts;
-   update/finalize the repository manifest;
-   assemble or refresh `release/2026-09-09/`;
-   regenerate release checksums;
-   optionally create a Git release/tag;
-   apply university/journal template-specific formatting only if
    required by the target venue;
-   prepare any additional submission-specific files required by the
    target venue.

No further analytical or substantive SLR revision is required unless the
evidence state or submission requirements change.
