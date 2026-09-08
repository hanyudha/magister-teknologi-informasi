# magister-teknologi-informasi

Catatan, dataset kerja, dokumentasi, dan progress perkuliahan **Magister
Teknologi Informasi**.

Repository ini memuat proyek **Systematic Literature Review (SLR)**
bidang Software Engineering dengan fokus **Artificial Intelligence for
DevOps Automation**.

## SLR --- Artificial Intelligence for DevOps Automation

### Working title

> **Artificial Intelligence in DevOps Automation: A Systematic
> Literature Review of Applications, Benefits, Challenges, and Research
> Trends from 2016 to 2026**

Versi Indonesia: \> **Artificial Intelligence dalam Otomasi DevOps:
Systematic Literature Review terhadap Aplikasi, Manfaat, Tantangan, dan
Tren Penelitian Tahun 2016--2026**

### Scope & methodology

-   Domain: Software Engineering
-   Area: DevOps
-   Boundary: **AI for DevOps**, bukan MLOps-only / DevOps-for-AI
-   AI scope: AI, ML, Deep Learning, AIOps, GenAI, LLM, AI Agents
-   Period: 2016--2026
-   Search date: 7 September 2026
-   Databases: ScienceDirect, IEEE Xplore, ACM Digital Library
-   Kitchenham & Charters: main SLR guideline
-   PICOC: scope/RQs/search
-   PRISMA 2020: selection reporting
-   IEEE citation style
-   Synthesis: descriptive quantitative + qualitative thematic
-   No statistical meta-analysis

## Research Questions

1.  **RQ1:** Bagaimana tren perkembangan penelitian AI dalam otomasi
    DevOps 2016--2026?
2.  **RQ2:** Pada aktivitas/tahapan DevOps apa AI diterapkan?
3.  **RQ3:** Teknik, metode, dan teknologi AI apa yang digunakan?
4.  **RQ4:** Apa manfaat dan dampak yang dilaporkan?
5.  **RQ5:** Apa tantangan, keterbatasan, dan peluang penelitian
    selanjutnya?

## Current progress --- 8 September 2026

  Phase                           Status
  ------------------------------- --------------------------
  Topic Definition                ✅ Complete
  Research Protocol               ✅ Complete / Locked
  Pilot + Full Search             ✅ Complete
  Deduplication                   ✅ Complete
  Title/Abstract Screening        ✅ Complete
  Full-text Retrieval/Screening   ✅ Complete / reconciled
  Quality Assessment              ✅ 60/60 PASS
  PRISMA Reconciliation           ✅ Complete
  Data Extraction                 ✅ 60/60
  RQ1--RQ5 Synthesis              ✅ Complete
  Research Gaps G1--G8            ✅ Locked
  Future Agenda FR1--FR5          ✅ Locked
  RQ1--RQ5 Final Tables/Charts    ✅ Complete
  PRISMA Final Flow Diagram       ⏳ Next
  Threats to Validity             ⬜ Pending
  Manuscript                      ⬜ Pending
  IEEE Reference Validation       ⬜ Pending
  Appendices                      ⬜ Pending
  Final DOCX                      ⬜ Pending

## Final PRISMA counts

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

Retrieval was attempted via Zotero for **all 382 reports**; **73 full
texts were obtained**. Therefore 309 are validly classified as
`Reports not retrieved`.

Full-text exclusions: FT3=2; FT4=1; FT5=7; FT6=3.

Authoritative workbook:
`SLR_Master_PRISMA_Reconciliation_382_2026-09-08_FINAL.xlsx`

## QA & extraction

-   QA: 60/60 PASS; threshold \>=3.0/5.
-   Data Extraction: 60/60 complete.
-   Final extraction schema: 26 fields.
-   Evidence Strength: Production; Industrial Empirical; Controlled
    Experimental; Benchmark; Simulation; Conceptual.

## RQ1

Provisional publication distribution: 2016=0; 2017=0; 2018=0; 2019=3;
2020=7; 2021=4; 2022=7; 2023=7; 2024=12; 2025=9; 2026=11.

PS045 is still unresolved (2025 vs 2026); provisional chart uses 2025.

Trajectory: **Predictive AI → Diagnostic AIOps → Generative AI → Agentic
AI**

## RQ2

Multi-label stages: Monitor 35; Operate 31; Incident/RCA 17; Test 16;
Build 10; Deploy 9; Develop/IaC 3; Model Governance 3; Human 1.

Main pattern: **Monitor → Operate → Incident/RCA**

## RQ3

Taxonomy: Classical ML; Deep Learning; Unsupervised/Anomaly AI;
Optimization/RL; NLP/Representation; GenAI/LLM; Agentic/Multi-Agent.

Mutually exclusive primary-category chart: - Classical ML 27 (45.0%) -
Deep Learning 8 (13.3%) - GenAI/LLM 7 (11.7%) - Unsupervised/Anomaly AI
6 (10.0%) - Agentic/Multi-Agent 5 (8.3%) - NLP/Representation 4 (6.7%) -
Optimization/RL 3 (5.0%)

AIOps is context/paradigm, not an algorithm.

## RQ4

Benefit themes: B1 Speed & Efficiency; B2 Accuracy & Detection Quality;
B3 Reliability & Availability; B4 Cost & Resource Optimization; B5
Automation & Toil Reduction; B6 Security Improvement; B7 Human Decision
Support & Productivity.

Do not invent corpus-wide B1--B7 frequencies. Final RQ4 chart uses **16
representative evidence anchors** only.

Key interpretation: **technical capability is developing faster than
demonstrated production benefit**.

## RQ5

Challenge themes: data quality; imbalance; leakage; drift;
generalization; benchmark-production gap; explainability/trust;
hallucination; cost/latency; integration; remediation safety; human
oversight; privacy/security; evaluation inconsistency.

Research gaps: - G1 Production-scale validation - G2 Generalization - G3
Drift/lifecycle - G4 Explainability/trust/reliability - G5 Remediation
safety - G6 LLM/agent cost & latency - G7 Human--AI
collaboration/adoption - G8 Integrated ML + DevOps operational
evaluation

Highest priority: **G1, G5, G8**.

Future agenda: FR1 Production-Validated; FR2 Adaptive/Generalizable; FR3
Trustworthy/Explainable LLM-AIOps; FR4 Safe/Cost-Efficient Agentic
DevOps; FR5 Human-Centered Autonomous DevOps.

Target trajectory: **Predictive → Diagnostic → Generative → Agentic →
Trustworthy Autonomous DevOps**

## Reporting artifacts

Current reporting artifacts include:

``` text
RQ3_Final_AI_Taxonomy_and_Methods_DevOps_2016-2026.xlsx
RQ4_Final_Benefits_Impacts_Evidence_Anchors_AI_DevOps_2016-2026.xlsx
RQ5_Final_Challenges_Gaps_Future_Research_AI_DevOps_2016-2026.xlsx
SLR_Master_PRISMA_Reconciliation_382_2026-09-08_FINAL.xlsx
```

RQ1 and RQ2 final tables/charts were also completed in the working
session and should be stored under `06_synthesis/` or
`08_manuscript/tables|figures/`.

## Repository structure

``` text
magister-teknologi-informasi/
├── README.md
├── 00_context/
│   ├── SLR_Milestone_AI_DevOps_2016-2026.md
│   ├── SLR_SESSION_HANDOFF_2026-09-08.md
│   └── SLR_CONTEXT_MASTER_2026-09-08.md
├── 01_protocol/
├── 02_search/
├── 03_screening/
├── 04_quality/
├── 05_extraction/
├── 06_synthesis/
├── 07_prisma/
├── 08_manuscript/
│   ├── figures/
│   ├── tables/
│   └── draft/
└── 09_archive/
```

## Source-of-truth rules

1.  `README.md` = overview/current status/navigation.
2.  `SLR_Milestone_AI_DevOps_2016-2026.md` = full history +
    authoritative current-state section.
3.  `SLR_SESSION_HANDOFF_2026-09-08.md` = compact new-session context.
4.  `SLR_CONTEXT_MASTER_2026-09-08.md` = dense machine-readable/manual
    handoff context.
5.  Evidence Ledger = synthesis findings and claim guardrails.
6.  Final PRISMA workbook = authoritative retrieval/full-text audit.
7.  Record-level screening/extraction workbooks remain source of truth
    for paper-level decisions.
8.  Raw exports are immutable.
9.  Unknown remains Unknown until evidence resolves it.

## Bibliographic caveats

-   PS019 = 2025
-   PS029 = 2024
-   PS043 = 2021
-   PS044 = 2023
-   PS045 = unresolved 2025 vs 2026; provisional RQ1 uses 2025

## Critical warning

Do **not** reuse the earlier generated PRISMA image. It contained wrong
database counts and wrong FT-code descriptions.

## Next step

**Create the authoritative corrected PRISMA 2020 final flow diagram**,
then finalize **Threats to Validity**, then start the manuscript.

## New-session prompt

> Baca `SLR_SESSION_HANDOFF_2026-09-08.md` dan
> `SLR_CONTEXT_MASTER_2026-09-08.md` sebagai authoritative state. PRISMA
> reconciliation sudah final: 382 sought, 309 not retrieved, 73
> retrieved/assessed, 13 excluded, 60 included. RQ1--RQ5 tables/charts
> sudah final. Jangan gunakan PRISMA image lama yang salah. Lanjutkan
> satu step: buat authoritative PRISMA 2020 final flow diagram, lalu
> Threats to Validity.
