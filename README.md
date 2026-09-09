# magister-teknologi-informasi

Catatan, dataset kerja, dokumentasi, dan progress perkuliahan **Magister Teknologi Informasi**.

Repository ini memuat proyek **Systematic Literature Review (SLR)** bidang Software Engineering dengan fokus **Artificial Intelligence for DevOps Automation**.

## Final working title

> **Artificial Intelligence in DevOps Automation: A Systematic Literature Review of Applications, Benefits, Challenges, and Research Trends from 2016 to 2026**

## Scope & methodology

- Domain: Software Engineering
- Area: DevOps
- Boundary: **AI-for-DevOps**, bukan MLOps-only / DevOps-for-AI
- Period: 2016–2026
- Search date: 7 September 2026
- Databases: ScienceDirect, IEEE Xplore, ACM Digital Library
- Kitchenham & Charters + PICOC + PRISMA 2020
- IEEE citation style
- Descriptive quantitative + qualitative thematic synthesis
- No statistical meta-analysis

## Current progress — 9 September 2026

| Phase | Status |
|---|---|
| Topic / Protocol / Search | ✅ Complete |
| Deduplication | ✅ Complete |
| Title/Abstract Screening | ✅ Complete |
| Full-text Retrieval/Screening | ✅ Complete / Reconciled |
| Quality Assessment | ✅ 60/60 PASS |
| PRISMA Reconciliation | ✅ Complete |
| PRISMA Final SVG | ✅ Locked |
| Data Extraction | ✅ 60/60 |
| PS↔U Mapping | ✅ 60/60 |
| RQ1–RQ5 | ✅ Complete / Locked |
| Research Gaps G1–G8 | ✅ Locked |
| Future Agenda FR1–FR5 | ✅ Locked |
| Threats to Validity | ✅ Locked |
| Manuscript Sections 1–7 | ✅ Locked |
| Abstract + Keywords | ✅ Locked |
| IEEE References | ✅ [1]–[66] |
| Publication-ready Cleanup | ✅ Complete |
| Appendices / Supplementary | ⏳ Next |
| Final submission package | ⬜ Pending |

## Final PRISMA counts

```text
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

## RQ1 final

```text
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
```

PS045 is final = **2026**.

Trajectory:
**Predictive AI → Diagnostic AIOps → Generative AI → Agentic AI**

## RQ2

Monitor 35; Operate 31; Incident/RCA 17; Test 16; Build 10; Deploy 9; Develop/IaC 3; Model Governance 3; Human 1.

## RQ3

Classical ML 27; Deep Learning 8; GenAI/LLM 7; Unsupervised/Anomaly 6; Agentic/Multi-Agent 5; NLP/Representation 4; Optimization/RL 3.

## RQ4

Benefit themes B1–B7 are qualitative synthesis themes. Do not invent corpus-wide prevalence.

Core interpretation:
**technical capability is developing faster than demonstrated production benefit**.

## RQ5

G1 Production-scale validation; G2 Generalization; G3 Drift/lifecycle; G4 Explainability/trust/reliability; G5 Remediation safety; G6 LLM/agent cost & latency; G7 Human–AI collaboration/adoption; G8 Integrated ML + DevOps operational evaluation.

Future agenda:
FR1 Production-Validated; FR2 Adaptive/Generalizable; FR3 Trustworthy/Explainable LLM-AIOps; FR4 Safe/Cost-Efficient Agentic DevOps; FR5 Human-Centered Autonomous DevOps.

Target trajectory:
**Predictive → Diagnostic → Generative → Agentic → Trustworthy Autonomous DevOps**

## Study identity and references

- 60 included `Uxxxx` records recovered
- `PS001–PS060 ↔ Uxxxx`: 60/60
- DOI coverage: 60/60
- external verification: 60/60
- background references: [1]–[6]
- primary references: [7]–[66]
- citation-integrity audit: PASS

## Main current artifacts

```text
SLR_SESSION_HANDOFF_2026-09-09.md
SLR_CONTEXT_MASTER_2026-09-09.md
SLR_Milestone_AI_DevOps_2016-2026.md
SLR_EVIDENCE_SYNTHESIS_LEDGER_2026-09-09.md
SLR_PRISMA_RECONCILIATION_WORKSHEET_2026-09-09.md
PRISMA_2020_AI_DevOps_AUTHORITATIVE.svg
SLR_AI_DevOps_PUBLICATION_READY_FINAL_2026-09-09.docx
SLR_PS001-PS060_Uxxxx_FULL_EXACT_MAPPING_FINAL_2026-09-09.xlsx
SLR_Primary_Study_Reference_Ledger_EXTERNAL_VERIFICATION_COMPLETE_2026-09-09.xlsx
SLR_Final_PS_to_IEEE_Mapping_7-66_2026-09-09.xlsx
SLR_Final_Citation_Integrity_Audit_2026-09-09.xlsx
```

## Recommended repository structure

```text
magister-teknologi-informasi/
├── README.md
├── 00_context/
├── 01_protocol/
├── 02_search/
│   ├── raw/
│   ├── logs/
│   └── derived/
├── 03_screening/
├── 04_quality/
├── 05_extraction/
├── 06_synthesis/
├── 07_prisma/
├── 08_manuscript/
│   ├── figures/
│   ├── tables/
│   ├── draft/
│   └── final/
├── 09_references/
├── 10_supplementary/
└── 99_archive/
```

## Source-of-truth rules

1. `README.md` = current overview/navigation.
2. `SLR_SESSION_HANDOFF_2026-09-09.md` = compact new-session context.
3. `SLR_CONTEXT_MASTER_2026-09-09.md` = dense authoritative state.
4. `SLR_Milestone_AI_DevOps_2016-2026.md` = full historical audit trail.
5. Evidence ledger = claim guardrails and synthesis interpretation.
6. PRISMA worksheet + authoritative SVG = selection/reporting source of truth.
7. Record-level screening/extraction workbooks = source of truth for study-level decisions.
8. Raw search exports are immutable.
9. Archive superseded files instead of deleting them.

## Next step

**Appendices / Supplementary Material**, then final submission package.
