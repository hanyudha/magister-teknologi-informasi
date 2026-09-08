# magister-teknologi-informasi

Catatan, dataset kerja, dokumentasi, dan progress perkuliahan **Magister Teknologi Informasi**.

Repository ini saat ini juga digunakan untuk proyek **Systematic Literature Review (SLR)** pada bidang Software Engineering dengan fokus **Artificial Intelligence for DevOps Automation**.

---

## SLR — Artificial Intelligence for DevOps Automation

### Working Title

> **Artificial Intelligence in DevOps Automation: A Systematic Literature Review of Applications, Benefits, Challenges, and Research Trends from 2016 to 2026**

Versi Bahasa Indonesia:

> **Artificial Intelligence dalam Otomasi DevOps: Systematic Literature Review terhadap Aplikasi, Manfaat, Tantangan, dan Tren Penelitian Tahun 2016–2026**

### Scope

- Domain: **Software Engineering**
- Area: **DevOps**
- Boundary: **AI for DevOps**, bukan DevOps-for-AI / MLOps-only
- AI scope: AI, Machine Learning, Deep Learning, AIOps, Generative AI, Large Language Models, AI Agents
- Publication period: **2016–2026**
- Search date: **7 September 2026**
- Citation style: **IEEE**
- Synthesis: **Descriptive Quantitative + Qualitative Thematic**
- Statistical meta-analysis: **tidak digunakan**

### Methodology

- **Kitchenham & Charters** — guideline utama SLR Software Engineering
- **PICOC** — scope, Research Questions, dan search strategy
- **PRISMA 2020** — pelaporan study selection
- **Quality Assessment** — threshold `>= 3.0 / 5`

Primary databases:

1. ScienceDirect
2. IEEE Xplore
3. ACM Digital Library

Scopus Preview tidak digunakan sebagai database primer.

---

## Research Objective

> Mengidentifikasi dan menganalisis secara sistematis penerapan Artificial Intelligence dalam mendukung otomasi aktivitas DevOps selama periode 2016–2026, dengan fokus pada area penerapan, teknologi dan metode AI yang digunakan, manfaat yang diperoleh, tantangan yang dihadapi, serta perkembangan dan peluang penelitian selanjutnya.

---

## Research Questions

**RQ1 — Research Trend**

> Bagaimana tren perkembangan penelitian mengenai penerapan Artificial Intelligence dalam otomasi DevOps selama periode 2016–2026?

**RQ2 — Area of Application**

> Pada aktivitas atau tahapan DevOps apa saja teknologi Artificial Intelligence diterapkan?

**RQ3 — AI Technologies**

> Teknik, metode, dan teknologi Artificial Intelligence apa yang digunakan untuk mendukung otomasi DevOps?

**RQ4 — Benefits and Impact**

> Apa manfaat dan dampak yang dilaporkan dari penerapan Artificial Intelligence pada proses DevOps?

**RQ5 — Challenges and Research Opportunities**

> Apa tantangan, keterbatasan, dan peluang penelitian selanjutnya dalam penerapan Artificial Intelligence untuk otomasi DevOps?

---

## Current Progress

**Last updated: 8 September 2026**

| Phase | Tahap | Status |
|---|---|---|
| 1 | Topic Definition | ✅ Selesai |
| 2 | SLR Research Protocol | ✅ Selesai / Locked |
| 3 | Pilot Search | ✅ Selesai |
| 4 | Full Literature Search | ✅ Selesai |
| 5 | Deduplication | ✅ Selesai |
| 6 | Title & Abstract Screening | ✅ Selesai |
| 7 | Full-text Screening | ✅ Selesai untuk corpus yang diproses |
| 8 | Quality Assessment | ✅ 60/60 PASS |
| 9 | PRISMA Documentation | ⏳ Next — Final Reconciliation |
| 10 | Data Extraction | ✅ 60/60 |
| 11 | Data Synthesis | ✅ RQ1–RQ5 |
| 12 | Research Gap Identification | ✅ G1–G8 |
| 13 | Future Research Agenda | ✅ FR1–FR5 |
| 14 | SLR Writing | ⬜ Belum |

---

## Search & Study Selection

```text
Database search results identified                  1,132
Non-article/container records removed                   2
Bibliographic article records imported              1,130
Duplicate occurrences removed                         317
Unique records screened                               813
Title/abstract excluded                               431
Title/abstract Include / reports sought               382

Unique full-text studies processed                     73
Include                                                60
Exclude                                                13
Pending                                                 0
Duplicate PDFs encountered                              3
```

Full-text exclusion distribution:

```text
FT3 = 2
FT4 = 1
FT5 = 7
FT6 = 3
Total = 13
```

### PRISMA Caveat

Accounting antara `382 reports sought for retrieval` dan `73 unique full-text studies processed` **belum direkonsiliasi secara final**.

Jangan menganggap:

```text
382 - 73 = 309
```

sebagai `reports not retrieved` tanpa audit trail.

---

## Quality Assessment

```text
QA candidates = 60
QA assessed   = 60
QA PASS       = 60
QA FAIL       = 0
Progress      = 100%
```

QA tetap digunakan sebagai stratifikasi kekuatan evidence; PASS tidak berarti seluruh paper mempunyai kekuatan evidence yang sama.

---

## Data Extraction

Data Extraction selesai untuk seluruh **60 primary studies**.

Final schema = **26 fields**:

1. Paper ID
2. Authors
3. Year
4. Title
5. Source Database
6. Venue
7. Publication Type
8. Research Type
9. DevOps Stage
10. DevOps Activity
11. AI Category
12. AI Method/Model
13. Dataset/System
14. Research Objective
15. Evaluation Method
16. Metrics
17. Main Findings
18. Benefits
19. Challenges
20. Limitations
21. Future Work
22. RQ Mapping
23. QA Score
24. Industrial Context
25. Evidence Type
26. Evidence Strength

Evidence Strength:

- Production
- Industrial Empirical
- Controlled Experimental
- Benchmark
- Simulation
- Conceptual

---

## Main Synthesis Findings

### RQ1 — Research Trend

Provisional distribution:

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
2025 = 9
2026 = 11
Total = 60
```

Main trajectory:

```text
Predictive AI
      ↓
Diagnostic AIOps
      ↓
Generative AI
      ↓
Agentic AI
```

### RQ2 — DevOps Application Areas

Multi-label stage mapping:

```text
Monitor / Observability       35
Operate / Operations          31
Incident / RCA / Remediation  17
Test                          16
Build / CI                    10
Deploy / Release               9
Develop / Code / IaC           3
AIOps Model Governance         3
Human / Cross-cutting          1
```

Dominant pattern:

```text
Monitor → Operate → Incident / RCA
```

### RQ3 — AI Technology Taxonomy

1. Classical Machine Learning
2. Deep Learning
3. Unsupervised / Anomaly AI
4. Optimization & Reinforcement Learning
5. NLP / Representation Learning
6. Generative AI / Large Language Models
7. Agentic / Multi-Agent AI

> **AIOps diperlakukan sebagai application paradigm/context, bukan algoritma.**

Evolution:

```text
Model → Pipeline → Reasoning System → Agentic System
```

### RQ4 — Benefits

Locked benefit themes:

- B1 — Speed & Efficiency
- B2 — Accuracy & Detection Quality
- B3 — Reliability & Availability
- B4 — Cost & Resource Optimization
- B5 — Automation & Toil Reduction
- B6 — Security Improvement
- B7 — Human Decision Support & Productivity

Benchmark performance tidak otomatis dianggap production impact.

### RQ5 — Challenges

Main themes:

- data quality dan scarcity of labels
- class imbalance
- temporal leakage
- concept drift / model decay
- limited generalization
- benchmark-to-production gap
- explainability dan trust
- LLM hallucination / reliability
- inference cost dan latency
- DevOps toolchain integration
- autonomous-remediation safety
- human oversight
- privacy dan security
- non-standard evaluation metrics

---

## Research Gap Matrix

| ID | Research Gap |
|---|---|
| G1 | Kurangnya production-scale validation |
| G2 | Generalization antar-sistem dan organisasi masih terbatas |
| G3 | Concept drift dan long-term model maintenance belum cukup diteliti |
| G4 | Explainability, trust, dan reliability belum matang |
| G5 | Safety mechanisms untuk autonomous remediation belum matang |
| G6 | Cost, latency, dan resource consumption LLM/multi-agent kurang dievaluasi |
| G7 | Human–AI collaboration dan organizational adoption masih kurang diteliti |
| G8 | Belum ada evaluation framework konsisten yang menggabungkan ML metrics dengan DevOps operational outcomes |

Central gap:

> **Masih terdapat kesenjangan antara kemampuan eksperimental AI-for-DevOps dan trustworthy production-scale autonomy.**

---

## Future Research Agenda

- **FR1 — Production-Validated AI-for-DevOps**
- **FR2 — Adaptive and Generalizable AIOps**
- **FR3 — Trustworthy and Explainable LLM-AIOps**
- **FR4 — Safe and Cost-Efficient Agentic DevOps**
- **FR5 — Human-Centered Autonomous DevOps**

Roadmap:

```text
NEAR TERM
Production validation
+ standardized evaluation
+ time/drift-aware evaluation
+ cross-system benchmarking
+ LLM grounding

        ↓

MID TERM
Adaptive AIOps
+ explainability
+ cost-aware LLM/agents
+ human-AI collaboration
+ privacy-preserving AIOps

        ↓

LONG TERM
Safe autonomous remediation
+ closed-loop Agentic AIOps
+ continuous operational learning
+ trustworthy autonomous DevOps
```

Target trajectory:

```text
Predictive
→ Diagnostic
→ Generative
→ Agentic
→ Trustworthy Autonomous DevOps
```

---

## Repository Structure

```text
magister-teknologi-informasi/
├── README.md
│
├── 00_context/
│   ├── SLR_Milestone_AI_DevOps_2016-2026.md
│   └── SLR_SESSION_HANDOFF_2026-09-08.md
│
├── 01_protocol/
│   └── research-protocol.md
│
├── 02_search/
│   ├── search-log.md
│   └── raw-exports/
│
├── 03_screening/
│   ├── deduplication/
│   ├── title-abstract/
│   └── full-text/
│
├── 04_quality/
│   └── qa-log.md
│
├── 05_extraction/
│   ├── extraction-master.xlsx
│   └── extraction-schema.md
│
├── 06_synthesis/
│   └── SLR_EVIDENCE_SYNTHESIS_LEDGER_2026-09-08.md
│
├── 07_prisma/
│   └── SLR_PRISMA_RECONCILIATION_WORKSHEET_2026-09-08.md
│
├── 08_manuscript/
│   ├── figures/
│   ├── tables/
│   └── draft/
│
└── 09_archive/
```

Struktur tersebut adalah target. Folder/file yang belum diperlukan tidak harus dibuat sekaligus.

---

## Source-of-Truth Rules

1. **`README.md`**  
   Overview repository, current project status, dan navigasi.

2. **`SLR_Milestone_AI_DevOps_2016-2026.md`**  
   Riwayat proyek, keputusan metodologis, dan milestone lengkap.

3. **`SLR_SESSION_HANDOFF_*.md`**  
   Context ringkas untuk pindah sesi ChatGPT.

4. **`SLR_EVIDENCE_SYNTHESIS_LEDGER_*.md`**  
   Synthesis findings, evidence anchors, dan guardrail untuk penulisan.

5. **`SLR_PRISMA_RECONCILIATION_WORKSHEET_*.md`**  
   Audit retrieval dan angka final PRISMA.

6. **Screening / extraction workbooks**  
   Source of truth untuk keputusan pada level paper.

7. **Raw database exports**  
   Jangan ditimpa; simpan sebagai immutable audit trail.

8. **Unknown values**  
   Tetap `Unknown` sampai tersedia evidence yang cukup.

---

## Important Working Files

```text
SLR_Master_Deduplication_2026-09-07.xlsx
SLR_Master_Maybe_Resolved_813_2026-09-08.xlsx
SLR_Master_FullText_Screening_Ready_382_2026-09-08.xlsx
SLR_Include_382_for_Zotero_FullText_Retrieval.ris
SLR_Milestone_AI_DevOps_2016-2026.md
SLR_SESSION_HANDOFF_2026-09-08.md
SLR_EVIDENCE_SYNTHESIS_LEDGER_2026-09-08.md
SLR_PRISMA_RECONCILIATION_WORKSHEET_2026-09-08.md
```

---

## Bibliographic Caveats

- PS019 → **2025**
- PS029 → **2024**
- PS043 → **2021**
- PS044 → **2023**
- PS045 → **belum final**; perlu rekonsiliasi metadata 2025 vs filename 2026

Jangan menggunakan filename sebagai satu-satunya dasar metadata bibliografis.

---

## Current Next Step

### PRISMA Final Reconciliation

Target:

```text
Reports sought for retrieval        382
Reports not retrieved                 ?
Reports retrieved                     ?
Reports assessed for eligibility      ?
Full-text excluded                    ?
Studies included                     60
```

Rules:

- jangan mengarang missing counts;
- bedakan `reports` dan `studies`;
- bedakan retrieval failure dan full-text exclusion;
- seluruh angka final harus mempunyai audit trail.

Roadmap sesudahnya:

```text
PRISMA Final Reconciliation
        ↓
PRISMA 2020 Final Flow
        ↓
Final Tables & Charts
        ↓
Threats to Validity
        ↓
SLR Manuscript
        ↓
IEEE Reference Validation
        ↓
Appendices
        ↓
Final DOCX
```

---

## Definition of Done

- [x] Topic dan scope
- [x] Research Objective
- [x] RQ1–RQ5
- [x] PICOC
- [x] Research Protocol
- [x] Search Strategy
- [x] Search execution
- [x] Search date
- [x] Deduplication
- [x] Title/Abstract Screening
- [x] Full-text decisions untuk corpus diproses
- [x] QA 60/60
- [x] Data Extraction 60/60
- [x] Data Synthesis RQ1–RQ5
- [x] Research Gap G1–G8
- [x] Future Research Agenda FR1–FR5
- [ ] PRISMA Final Reconciliation
- [ ] PRISMA 2020 Final Flow
- [ ] Final Tables/Charts
- [ ] Threats to Validity
- [ ] SLR Manuscript
- [ ] IEEE Reference Validation
- [ ] Appendices
- [ ] Final DOCX

---

## Session Continuation

Untuk pindah ke sesi ChatGPT baru, gunakan:

```text
SLR_SESSION_HANDOFF_2026-09-08.md
```

Prompt singkat:

> Lanjutkan proyek SLR berdasarkan current project state. Keputusan yang sudah locked jangan diubah tanpa alasan metodologis. Current state: QA 60/60 PASS, Data Extraction 60/60 selesai, RQ1–RQ5 synthesis selesai, Research Gap G1–G8 dan Future Research Agenda FR1–FR5 sudah locked. Tahap berikutnya adalah PRISMA Final Reconciliation. Audit hubungan 382 reports sought dengan retrieval/full-text status aktual. Jangan menganggap selisih 309 otomatis sebagai reports not retrieved.

---

_Last updated: 8 September 2026_
