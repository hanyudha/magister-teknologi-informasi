# Appendix E — Data Extraction and Coding Framework

Data extraction was conducted for all **60 included primary studies** using a structured **26-field schema**. The framework was designed to preserve study identity, characterize the DevOps and AI dimensions of each study, capture study-level evidence, and maintain traceability from primary studies to RQ1–RQ5.

The complete record-level dataset is maintained as supplementary material; this appendix documents the extraction and coding framework rather than reproducing the full 60 × 26 evidence matrix.

## E.1 Data Extraction Fields

The final extraction schema consists of the following fields:

| No. | Field | Function |
|---:|---|---|
| 1 | Paper ID | Stable primary-study identifier (`PS001–PS060`) |
| 2 | Authors | Study authors |
| 3 | Year | Final bibliographic publication year |
| 4 | Title | Study title |
| 5 | Source Database | ScienceDirect, IEEE Xplore, or ACM Digital Library |
| 6 | Venue | Journal or conference venue |
| 7 | Publication Type | Primary publication type |
| 8 | Research Type | Study/evaluation design |
| 9 | DevOps Stage | DevOps lifecycle stage(s) addressed |
| 10 | DevOps Activity | Specific DevOps activity |
| 11 | AI Category | Normalized AI methodological family |
| 12 | AI Method / Model | Specific algorithm, model, or architecture |
| 13 | Dataset / System | Dataset, software system, logs, platform, or environment |
| 14 | Research Objective | Main study objective |
| 15 | Evaluation Method | Validation/evaluation procedure |
| 16 | Metrics | Evaluation metrics or outcome measures |
| 17 | Main Findings | Main evidence-supported findings |
| 18 | Benefits | Reported benefits or impacts |
| 19 | Challenges | Reported technical, operational, or organizational challenges |
| 20 | Limitations | Study limitations or threats |
| 21 | Future Work | Future research directions |
| 22 | RQ Mapping | Research Question(s) informed by the study |
| 23 | QA Score | Final QA status / score representation |
| 24 | Industrial Context | Application and validation context |
| 25 | Evidence Type | Descriptive evidence/evaluation type |
| 26 | Evidence Strength | Normalized evidence-strength category |

## E.2 Study Identity and Traceability

Each extraction record is keyed by `Paper ID` (`PS001–PS060`) and is mapped one-to-one to its screening identifier (`Uxxxx`). This allows evidence used in the manuscript to be traced back through screening and bibliographic records.

```text
60 PS identifiers
60 U identifiers
PS↔U mapping = 60/60 one-to-one
```

## E.3 DevOps Coding

DevOps-stage coding is **multi-label**, because a single AI intervention may span several lifecycle stages.

The final RQ2 taxonomy is:

```text
Monitor / Observability
Operate / Operations
Incident / RCA / Remediation
Test
Build / CI
Deploy / Release
Develop / Code / IaC
AIOps Model Governance
Human / Cross-cutting
```

For example, a study addressing monitoring, operational analytics, and incident diagnosis may be coded:

```text
Monitor; Operate; Incident/RCA
```

Consequently, RQ2 category frequencies are not mutually exclusive and are not expected to sum to 60.

`DevOps Activity` retains finer-grained descriptions such as anomaly detection, root-cause analysis, build prediction, test-case prioritization, deployment optimization, or automated remediation.

## E.4 AI Taxonomy

The final RQ3 taxonomy consists of seven primary categories:

| AI Category | Final primary-study count |
|---|---:|
| Classical ML | 27 |
| Deep Learning | 8 |
| Unsupervised / Anomaly AI | 6 |
| Optimization & RL | 3 |
| NLP / Representation | 4 |
| GenAI / LLM | 7 |
| Agentic / Multi-Agent | 5 |
| **Total** | **60** |

Individual studies can combine multiple methods. The detailed `AI Method / Model` field preserves hybrid approaches, while the RQ3 quantitative synthesis assigns one normalized **primary AI category** per study.

AIOps is treated as an **application paradigm**, not as an algorithm class.

## E.5 Evidence Strength

Study evidence is normalized into six evidence-strength categories:

```text
Production
Industrial Empirical
Controlled Experimental
Benchmark
Simulation
Conceptual
```

Evidence strength is distinct from QA status. A study may pass the minimum QA threshold while providing conceptual, simulation, benchmark, or production-level evidence.

This distinction supports interpretation of the recurring benchmark-to-production gap identified in the review.

## E.6 Benefit Coding

Study-level benefit evidence is preserved in the `Benefits` field and synthesized using seven themes:

```text
B1 — Speed & Efficiency
B2 — Accuracy & Detection Quality
B3 — Reliability & Availability
B4 — Cost & Resource Optimization
B5 — Automation & Toil Reduction
B6 — Security Improvement
B7 — Human Decision Support & Productivity
```

The current repository does not preserve a complete record-level B1–B7 binary coding matrix for all 60 studies. Therefore, corpus-wide B1–B7 prevalence is not reported unless a new complete recoding is performed.

## E.7 Challenge and Future-Research Coding

The `Challenges`, `Limitations`, and `Future Work` fields provide the study-level evidence used to derive the final RQ5 research-gap taxonomy:

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

These were further synthesized into five future-research directions:

```text
FR1 — Production-Validated AI-for-DevOps
FR2 — Adaptive and Generalizable AIOps
FR3 — Trustworthy and Explainable LLM-AIOps
FR4 — Safe and Cost-Efficient Agentic DevOps
FR5 — Human-Centered Autonomous DevOps
```

The G1–G8 and FR1–FR5 labels are synthesis constructs derived from cross-study evidence; they are not claimed to be terminology used verbatim by every primary study.

## E.8 Field-to-RQ Mapping

| Main extraction component | Primary use |
|---|---|
| Year and descriptive publication data | RQ1 |
| DevOps Stage / Activity | RQ2 |
| AI Category / Method | RQ3 |
| Metrics, Main Findings, Benefits | RQ4 |
| Challenges, Limitations, Future Work | RQ5 |
| Dataset/System, Evaluation Method, Industrial Context, Evidence Type/Strength | Cross-cutting evidence interpretation |
| RQ Mapping | Study-to-RQ traceability |

## E.9 Extraction Reproducibility

The complete extraction dataset is stored in:

```text
05_extraction/
SLR_Data_Extraction_60_Studies_26Fields_FINAL_2026-09-09.xlsx
```

The study identity mapping is stored in:

```text
05_extraction/
SLR_PS001-PS060_Uxxxx_FULL_EXACT_MAPPING_FINAL_2026-09-09.xlsx
```

Known recovery limitations are retained explicitly. In particular, exact historical numeric QA scores are unrecovered, and the current extraction records `PASS — exact score unrecovered`. Missing historical values are not reconstructed through inference.

The extraction layer is therefore reproducible for the currently preserved 60-study evidence base while preserving the provenance limitations of recovered artifacts.
