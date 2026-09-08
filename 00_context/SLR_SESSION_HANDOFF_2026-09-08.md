# SLR AI-for-DevOps --- Session Handoff

**Updated: 8 September 2026 --- Final state before session migration**

## Purpose

Use this file as the first context file in a new ChatGPT session. It
records the current authoritative project state and supersedes older
handoff notes where they conflict.

## Locked scope

-   Domain: Software Engineering
-   Topic: **Artificial Intelligence for DevOps Automation**
-   Period: **2016--2026**
-   Search date: **7 September 2026**
-   Boundary: **AI for DevOps**, not DevOps-for-AI / MLOps-only
-   AI scope: AI, ML, Deep Learning, AIOps, Generative AI, LLM, AI
    Agents
-   Databases: ScienceDirect, IEEE Xplore, ACM Digital Library
-   Methodology: Kitchenham & Charters + PICOC + PRISMA 2020
-   Citation: IEEE
-   Synthesis: descriptive quantitative + qualitative thematic; no
    statistical meta-analysis

## Locked Research Questions

-   **RQ1:** research trends, 2016--2026
-   **RQ2:** DevOps stages/activities where AI is applied
-   **RQ3:** AI techniques/methods/technologies used
-   **RQ4:** benefits and impacts
-   **RQ5:** challenges, limitations, and future research opportunities

## Final selection / PRISMA accounting

The previous uncertainty has been resolved by user confirmation:
**full-text retrieval was attempted via Zotero for all 382 reports, and
only 73 full texts were obtained.**

``` text
Database search results identified                 1,132
ScienceDirect                                        185
IEEE Xplore                                          765
ACM Digital Library                                  180
Other/container records removed before screening       2
Bibliographic records entering deduplication        1,130
Duplicate occurrences removed                        317
Unique records screened                              813
Title/abstract records excluded                      431
Reports sought for retrieval                         382
Reports not retrieved                                309
Reports retrieved                                     73
Reports assessed for eligibility                      73
Full-text reports excluded                            13
Studies included                                      60
```

Full-text exclusions: - FT3 --- No AI/ML/GenAI/AIOps intervention: 2 -
FT4 --- MLOps only / DevOps-for-AI: 1 - FT5 --- Secondary or non-primary
publication: 7 - FT6 --- Insufficient substantive evidence for RQs: 3

**Do not revert to the old warning that 309 is unknown.** The 309 are
validly classified as reports not retrieved because the user explicitly
confirmed retrieval was attempted for all 382 via Zotero and only 73
were obtained.

Authoritative PRISMA workbook:
`SLR_Master_PRISMA_Reconciliation_382_2026-09-08_FINAL.xlsx`

## QA and extraction

-   QA: 60/60 assessed, 60 PASS, 0 FAIL.
-   Threshold: \>=3.0/5.
-   QA remains evidence-strength stratification; PASS does not imply
    equal evidence quality.
-   Data Extraction: **60/60 complete**.
-   Final schema: **26 fields**, including `Evidence Strength`.
-   Evidence Strength: Production; Industrial Empirical; Controlled
    Experimental; Benchmark; Simulation; Conceptual.

## RQ1 --- final synthesis

Provisional year distribution:
`2016=0, 2017=0, 2018=0, 2019=3, 2020=7, 2021=4, 2022=7, 2023=7, 2024=12, 2025=9, 2026=11`.

PS045 remains bibliographically unresolved (2025 vs 2026); provisional
RQ1 uses 2025. If confirmed 2026, then 2025=8 and 2026=12.

Trajectory: **Predictive AI → Diagnostic AIOps → Generative AI → Agentic
AI**

RQ1 final table/chart has been prepared for reporting.

## RQ2 --- final synthesis

Multi-label stage mapping: - Monitor / Observability: 35 (58.3%) -
Operate / Operations: 31 (51.7%) - Incident / RCA / Remediation: 17
(28.3%) - Test / Continuous Testing: 16 (26.7%) - Build / CI: 10
(16.7%) - Deploy / Release / Delivery: 9 (15.0%) - Develop / Code / IaC:
3 (5.0%) - AIOps Model Governance: 3 (5.0%) - Human / Cross-cutting: 1
(1.7%)

Main finding: **shift-right concentration** toward Monitor → Operate →
Incident/RCA.

RQ2 final table/chart has been prepared for reporting.

## RQ3 --- final synthesis

Taxonomy: 1. Classical Machine Learning 2. Deep Learning 3. Unsupervised
/ Anomaly AI 4. Optimization & Reinforcement Learning 5. NLP /
Representation Learning 6. Generative AI / LLM 7. Agentic / Multi-Agent
AI

AIOps is an application paradigm/context, not an algorithm.

Primary-category distribution used for the mutually exclusive RQ3
chart: - Classical ML: 27 (45.0%) - Deep Learning: 8 (13.3%) -
Generative AI / LLM: 7 (11.7%) - Unsupervised / Anomaly AI: 6 (10.0%) -
Agentic / Multi-Agent AI: 5 (8.3%) - NLP / Representation Learning: 4
(6.7%) - Optimization & Reinforcement Learning: 3 (5.0%) - Total: 60

Evolution: **Model → Pipeline → Reasoning System → Agentic System**

Artifact: `RQ3_Final_AI_Taxonomy_and_Methods_DevOps_2016-2026.xlsx`

## RQ4 --- final synthesis

Benefit themes: - B1 Speed & Efficiency - B2 Accuracy & Detection
Quality - B3 Reliability & Availability - B4 Cost & Resource
Optimization - B5 Automation & Toil Reduction - B6 Security
Improvement - B7 Human Decision Support & Productivity

Important guardrail: the locked source does **not** contain reproducible
corpus-wide B1--B7 frequencies across all 60 studies. Do not invent
prevalence. The RQ4 chart therefore represents coverage among **16
representative evidence anchors**, not all 60 studies.

Strong evidence anchors include PS056 Facebook PTS, PS057 Alibaba
failure prediction, PS060 GPT-4 RCA, PS012 DeCaf, PS042 LLM log
prioritization, and PS049 multi-agent RCA.

Core interpretation: **technical capability is developing faster than
demonstrated production benefit**, especially for LLM and agentic AIOps.

Artifact:
`RQ4_Final_Benefits_Impacts_Evidence_Anchors_AI_DevOps_2016-2026.xlsx`

## RQ5 --- final synthesis

Fourteen challenge themes: 1. Data Quality & Availability 2. Class
Imbalance 3. Data Leakage & Unrealistic Evaluation 4. Concept Drift &
Model Decay 5. Limited Generalizability 6. Benchmark-to-Production Gap
7. Explainability & Trust 8. LLM Hallucination & Reliability 9. Cost,
Latency & Resource Consumption 10. Integration Complexity 11. Safety of
Autonomous Remediation 12. Human-in-the-Loop 13. Security & Privacy 14.
Evaluation Metric Inconsistency

Do not invent corpus-wide challenge frequencies; they were synthesized
qualitatively.

Locked gaps: - G1 Production-scale validation - G2 Cross-system
generalization - G3 Concept drift & long-term maintenance - G4
Explainability, trust & reliability - G5 Autonomous-remediation safety -
G6 LLM/agent cost & latency - G7 Human--AI collaboration & adoption - G8
Unified ML + DevOps operational evaluation framework

Priority: - Highest: G1, G5, G8 - High: G2, G3, G4 - Emerging/high: G6,
G7

Future agenda: - FR1 Production-Validated AI-for-DevOps - FR2 Adaptive
and Generalizable AIOps - FR3 Trustworthy and Explainable LLM-AIOps -
FR4 Safe and Cost-Efficient Agentic DevOps - FR5 Human-Centered
Autonomous DevOps

Long-term trajectory: **Predictive → Diagnostic → Generative → Agentic →
Trustworthy Autonomous DevOps**

Artifact:
`RQ5_Final_Challenges_Gaps_Future_Research_AI_DevOps_2016-2026.xlsx`

## Metadata caveats

-   PS019 = 2025
-   PS029 = 2024
-   PS043 = 2021
-   PS044 = 2023
-   PS045 = unresolved 2025 vs 2026; provisional RQ1 uses 2025
-   Exact QA numeric scores PS001--PS020 still need reconciliation only
    if a final QA-score distribution is required.

## PRISMA diagram warning

An earlier image-generation attempt produced incorrect database counts
and incorrect FT-code labels. **Do not use it.**

Correct flow text:

``` text
Records identified from databases (n=1,132)
- ScienceDirect (n=185)
- IEEE Xplore (n=765)
- ACM Digital Library (n=180)

Other/container records removed before screening (n=2)
Bibliographic records entering deduplication (n=1,130)
Duplicate occurrences removed (n=317)
Records screened (n=813)
Records excluded (n=431)
Reports sought for retrieval (n=382)
Reports not retrieved (n=309)
Reports assessed for eligibility (n=73)
Reports excluded (n=13):
  FT3 n=2
  FT4 n=1
  FT5 n=7
  FT6 n=3
Studies included in review (n=60)
```

Do not invent what the two container records were.

## Current phase

Completed: - Protocol/search/deduplication/screening - PRISMA
reconciliation - QA - Data Extraction - RQ1--RQ5 synthesis - G1--G8 -
FR1--FR5 - RQ1--RQ5 final reporting tables/charts

Still pending: 1. **Correct authoritative PRISMA 2020 flow diagram** 2.
**Threats to Validity finalization** 3. SLR manuscript 4. IEEE reference
validation 5. Appendices 6. Final DOCX

## Recommended next action

Continue **one step at a time**.

> **NEXT: create/finalize the authoritative PRISMA 2020 flow diagram
> using the locked counts above. After that, finalize Threats to
> Validity.**

## Continuation prompt

> Gunakan `SLR_SESSION_HANDOFF_2026-09-08.md` dan
> `SLR_CONTEXT_MASTER_2026-09-08.md` sebagai authoritative current
> project state. Jangan mengubah keputusan locked tanpa alasan
> metodologis. PRISMA retrieval accounting sudah final: 382 sought, 73
> retrieved/assessed, 309 not retrieved, 13 excluded, 60 included.
> RQ1--RQ5 tables/charts sudah difinalisasi. Jangan gunakan PRISMA image
> lama yang salah. Next step adalah membuat authoritative PRISMA 2020
> final flow diagram, lalu Threats to Validity.
