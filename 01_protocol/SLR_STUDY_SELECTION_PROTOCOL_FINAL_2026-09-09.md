# SLR Study Selection Protocol — Final Operational Record

**Project:** Artificial Intelligence in DevOps Automation  
**Review period:** 2016–2026  
**Search date:** 7 September 2026  
**Authoritative state:** 9 September 2026  
**Methodological basis:** Kitchenham & Charters + PRISMA 2020

---

## 1. Purpose

This document records the study-selection procedure that can be supported by the preserved SLR evidence.

It distinguishes between:

1. **draft inclusion/exclusion criteria** documented during protocol development;
2. the **operational selection boundary** demonstrably applied during screening;
3. the **final observed screening outcomes**; and
4. PRISMA accounting.

This distinction is necessary because the archived milestone files label the original IC/EC table as **draft awal**. The repository therefore supports the criteria as documented protocol-development material, but it does not justify retrospectively claiming a stronger pre-registration status than the evidence supports.

---

## 2. Conceptual Selection Boundary

The review focuses on:

> **AI-for-DevOps**

Eligible studies must use Artificial Intelligence, Machine Learning, Deep Learning, Generative AI, LLMs, AIOps, or related AI techniques to improve, support, analyze, optimize, or automate a DevOps-related activity.

The review excludes:

> **MLOps-only / DevOps-for-AI**

unless AI is explicitly being used to improve a DevOps activity.

Examples of in-scope activity include:

- anomaly detection;
- log analysis;
- incident prediction;
- root-cause analysis;
- CI/CD optimization;
- deployment optimization;
- automated troubleshooting;
- failure prediction;
- intelligent monitoring;
- AI-assisted operations;
- LLM-assisted DevOps automation.

Examples of out-of-scope activity include:

- ML model deployment as the primary topic;
- model versioning;
- dataset versioning;
- ML training pipelines;
- model retraining;
- model serving;
- MLOps practice without AI being used to improve DevOps.

---

## 3. Documented Draft Inclusion Criteria

The protocol-development archive records the following criteria as **draft awal**:

| ID | Documented draft inclusion criterion |
|---|---|
| IC1 | Publication was issued during 2016–2026 |
| IC2 | Study discusses DevOps or activities explicitly related to DevOps/CI/CD |
| IC3 | Study applies AI/ML/GenAI/LLM to support or automate DevOps activities |
| IC4 | Study is a peer-reviewed journal article or conference paper |
| IC5 | Article is written in English |
| IC6 | Full text is accessible |
| IC7 | Study provides information usable for answering at least one Research Question |

These criteria are retained as the documented selection framework. However, the source labels them as a draft and therefore this file does not claim that an independently time-stamped final protocol version containing this exact wording was preserved before screening.

---

## 4. Documented Draft Exclusion Criteria

The protocol-development archive records:

| ID | Documented draft exclusion criterion |
|---|---|
| EC1 | Duplicate publication |
| EC2 | Study is not relevant to Software Engineering / DevOps |
| EC3 | Study discusses AI but does not apply it to DevOps activities |
| EC4 | Study only discusses DevOps/MLOps for developing AI systems, without AI being used to improve DevOps |
| EC5 | Editorial, poster, presentation, book review, thesis, or other non-peer-reviewed material |
| EC6 | Full text is unavailable |
| EC7 | Article is not in English |
| EC8 | Secondary study such as an SLR or survey is not included as a primary study |

Secondary studies could still be used for:

- background;
- related work;
- terminology discovery;
- keyword discovery;
- backward snowballing;
- forward snowballing;
- comparison with review findings.

---

## 5. Operational Selection Procedure

The preserved workflow follows:

```text
Database search
    ↓
Raw export
    ↓
Deduplication
    ↓
Title/abstract screening
    ↓
Retrieval attempt
    ↓
Full-text eligibility screening
    ↓
Quality assessment
    ↓
Included primary studies
```

The final review numbers are:

```text
1,132 records identified
2 records removed before screening
1,130 records entering deduplication
317 duplicate occurrences removed
813 unique records screened
431 title/abstract records excluded
382 reports sought for retrieval
309 reports not retrieved
73 reports retrieved / assessed
13 full-text reports excluded
60 primary studies included
```

---

## 6. Deduplication

Primary artifact:

```text
03_screening/dedup/SLR_Master_Deduplication_2026-09-07.xlsx
```

Input:

```text
1,130 bibliographic records
```

Removed:

```text
317 duplicate occurrences
```

Output:

```text
813 unique records
```

Check:

```text
1,130 - 317 = 813
```

Duplicate removal is a pre-screening bibliographic operation and should not be confused with substantive study exclusion.

---

## 7. Title and Abstract Screening

Primary artifact:

```text
03_screening/title-abstract/SLR_Master_Maybe_Resolved_813_2026-09-08.xlsx
```

Input:

```text
813 unique records
```

Outcome:

```text
431 excluded
382 retained for retrieval
```

Check:

```text
813 - 431 = 382
```

At this stage, the conceptual AI-for-DevOps boundary was used to reject records that were clearly outside the review scope.

The preserved evidence supports the final count, but this reproduction guide does not invent per-record exclusion categories beyond those stored in the screening artifact.

---

## 8. Full-Text Retrieval

Primary artifacts:

```text
03_screening/full-text/SLR_Master_FullText_Screening_Ready_382_2026-09-08.xlsx
03_screening/prism-reconciliation/SLR_Master_PRISMA_Reconciliation_382_2026-09-08_FINAL.xlsx
```

Retrieval was attempted for:

```text
382 reports
```

Final result:

```text
309 reports not retrieved
73 reports retrieved / assessed
```

Check:

```text
382 - 309 = 73
```

### Important PRISMA distinction

The 309 unavailable reports are categorized as:

```text
Reports not retrieved
```

They are **not** counted as full-text eligibility exclusions because their full texts were not available for substantive eligibility assessment.

This distinction is required to preserve the final PRISMA accounting.

---

## 9. Full-Text Eligibility Screening

Primary artifact:

```text
03_screening/full-text/Full-Text Screening_73total.xlsx
```

Input:

```text
73 retrieved reports
```

Outcome:

```text
60 included
13 excluded
```

Check:

```text
73 - 13 = 60
```

The final observed full-text exclusion categories are:

| Code | Operational reason | Count |
|---|---|---:|
| FT3 | No AI/ML/GenAI/AIOps intervention | 2 |
| FT4 | MLOps only / DevOps-for-AI | 1 |
| FT5 | Secondary or non-primary publication | 7 |
| FT6 | Insufficient substantive evidence for RQs | 3 |
|  | **Total** | **13** |

Only FT3–FT6 are reported here because these are the exclusion categories actually observed in the final locked full-text exclusion distribution.

This file does not invent unused FT1, FT2, or FT7 definitions unless a preserved screening artifact explicitly supplies them.

---

## 10. Relationship Between Draft EC Codes and Final FT Codes

The draft exclusion framework and the final full-text exclusion codes are related conceptually but are not assumed to be a one-to-one coding system.

For example:

- draft EC3 broadly corresponds to AI without valid DevOps application;
- draft EC4 corresponds to MLOps-only / DevOps-for-AI;
- draft EC8 corresponds to secondary studies;
- draft IC7 / substantive relevance is reflected operationally by FT6.

However:

> Do not mechanically replace FT codes with EC codes in the historical screening data.

The FT codes are the authoritative final full-text exclusion labels for PRISMA reporting.

---

## 11. Included Primary Studies

Recovered included-study identity artifact:

```text
03_screening/full-text/SLR_60_Included_Uxxxx_RECOVERED_2026-09-09.xlsx
```

Final traceability mapping:

```text
05_extraction/SLR_PS001-PS060_Uxxxx_FULL_EXACT_MAPPING_FINAL_2026-09-09.xlsx
```

Final state:

```text
60 included studies
60 Uxxxx identifiers
60 PS001–PS060 identifiers
60/60 one-to-one mapping
```

The included primary-study corpus is therefore fixed at 60 for the current manuscript state.

---

## 12. Quality Assessment Position in Selection

Quality assessment was conducted for all 60 included primary studies.

Final result:

```text
QA assessed = 60
QA PASS     = 60
QA FAIL     = 0
Threshold   = >= 3.0 / 5
```

Quality assessment did not reduce the final study count because all 60 studies passed the threshold.

QA PASS does not imply equal evidence strength.

---

## 13. Selection Integrity Equations

A valid reconstruction must satisfy:

```text
1,130 - 317 = 813
813 - 431 = 382
382 - 309 = 73
73 - 13 = 60
```

Full-text exclusion total:

```text
FT3 2
+ FT4 1
+ FT5 7
+ FT6 3
= 13
```

---

## 14. Selection Evidence Locations

```text
03_screening/
├── dedup/
│   └── SLR_Master_Deduplication_2026-09-07.xlsx
├── title-abstract/
│   └── SLR_Master_Maybe_Resolved_813_2026-09-08.xlsx
├── full-text/
│   ├── SLR_Master_FullText_Screening_Ready_382_2026-09-08.xlsx
│   ├── Full-Text Screening_73total.xlsx
│   └── SLR_60_Included_Uxxxx_RECOVERED_2026-09-09.xlsx
└── prism-reconciliation/
    └── SLR_Master_PRISMA_Reconciliation_382_2026-09-08_FINAL.xlsx
```

PRISMA support:

```text
07_prisma/
├── PRISMA-2020-F_AI_DevOps_AUTHORITATIVE.svg
└── SLR_PRISMA_RECONCILIATION_WORKSHEET_2026-09-09.md
```

---

## 15. Reproducibility Limitations

The repository strongly supports:

- final selection counts;
- deduplication outcome;
- title/abstract screening outcome;
- retrieval accounting;
- final full-text exclusion distribution;
- final included corpus;
- one-to-one PS↔U study identity.

The repository does not support claiming that the archived IC1–IC7 / EC1–EC8 wording was preserved as a separately frozen, pre-registered final protocol before screening, because the surviving source labels it as **draft awal**.

Therefore publication-ready wording should distinguish:

> documented protocol criteria

from:

> final observed operational screening outcomes.

This is a provenance safeguard rather than a weakness in the final selection accounting.

---

## 16. Status

**Study selection operational record: FINAL for the currently preserved evidence.**

Do not change the locked counts or FT3–FT6 distribution without record-level evidence and a controlled correction across the screening dataset, PRISMA artifacts, context master, and manuscript.
