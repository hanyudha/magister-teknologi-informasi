# SLR Data Extraction and Coding Framework — Final Operational Record

**Project:** Artificial Intelligence in DevOps Automation  
**Review period:** 2016–2026  
**Authoritative state:** 9 September 2026  
**Included primary studies:** 60  
**Extraction schema:** 26 fields

---

## 1. Purpose

This document records the final data-extraction structure and coding framework used to transform the 60 included primary studies into the evidence base for RQ1–RQ5.

The extraction model combines:

1. bibliographic identity;
2. study-design and context descriptors;
3. DevOps-stage and activity coding;
4. AI taxonomy coding;
5. evidence extraction;
6. quality/evidence-strength descriptors; and
7. Research Question mapping.

The canonical extraction workbook is:

```text
05_extraction/
SLR_Data_Extraction_60_Studies_26Fields_FINAL_2026-09-09.xlsx
```

The final schema contains **26 fields** distributed across two logical views:

```text
Bibliographic / coding fields = 16
Evidence fields               = 12
Shared identity fields        = 2
Unique fields                 = 26
```

The shared identity fields are `Paper ID` and `Title`.

---

# 2. Final 26-Field Extraction Schema

## 2.1 Bibliographic and Coding Fields

| Field | Purpose |
|---|---|
| Paper ID | Stable manuscript-level identifier (`PS001–PS060`) |
| Authors | Study authors |
| Year | Final bibliographic publication year |
| Title | Primary-study title |
| Source Database | Database from which the record was retained |
| Venue | Journal, conference, or publication venue |
| Publication Type | Journal article, conference paper, or other eligible primary publication |
| Research Type | High-level design or study type |
| DevOps Stage | DevOps lifecycle stage(s) addressed by the study |
| DevOps Activity | More specific operational activity addressed |
| AI Category | AI family or primary methodological class |
| AI Method / Model | Specific algorithm, architecture, or AI technique |
| QA Score | Final quality-assessment status / score representation |
| Industrial Context | Production, organizational, industrial, or other application context |
| Evidence Type | Description of the type of empirical or conceptual evidence |
| Evidence Strength | Normalized strength-of-evidence category |

## 2.2 Evidence Fields

| Field | Purpose |
|---|---|
| Paper ID | Links evidence back to the canonical study identity |
| Title | Human-readable cross-check of study identity |
| Dataset / System | Dataset, software system, platform, logs, repository, or operational environment used |
| Research Objective | Main research objective relevant to the review |
| Evaluation Method | Evaluation or validation procedure used |
| Metrics | Quantitative or qualitative evaluation measures |
| Main Findings | Primary findings supported by the study |
| Benefits | Reported or evidenced benefits relevant to AI-for-DevOps |
| Challenges | Operational, methodological, technical, or organizational challenges |
| Limitations | Explicit or evidence-supported study limitations |
| Future Work | Research directions stated or supported by the study |
| RQ Mapping | Research Question(s) informed by the extracted evidence |

---

# 3. Extraction Unit and Identity Control

The unit of analysis is the **included primary study**, represented by:

```text
PS001–PS060
```

Each `PSxxx` identifier is mapped one-to-one to the corresponding screening identifier:

```text
Uxxxx
```

Canonical mapping artifact:

```text
05_extraction/
SLR_PS001-PS060_Uxxxx_FULL_EXACT_MAPPING_FINAL_2026-09-09.xlsx
```

The final integrity condition is:

```text
60 PS identifiers
60 included U identifiers
60/60 one-to-one mapping
```

The `Paper ID` should be used as the stable join key across extraction, QA, synthesis, reference, and supplementary artifacts.

---

# 4. DevOps Stage Coding

DevOps-stage coding is **multi-label**.

A study can contribute to more than one lifecycle stage when its intervention spans multiple activities.

The final normalized RQ2 stage/activity taxonomy is:

| Code / Label | Operational interpretation |
|---|---|
| Monitor / Observability | Monitoring, telemetry, logs, metrics, anomaly detection, observability |
| Operate / Operations | Operational management, runtime optimization, maintenance, service operation |
| Incident / RCA / Remediation | Incident detection, diagnosis, root-cause analysis, troubleshooting, remediation |
| Test | Testing, test prioritization, defect/failure-oriented test activities |
| Build / CI | Build processes, continuous integration, build prediction, CI job analysis |
| Deploy / Release | Deployment, release, rollout, delivery optimization |
| Develop / Code / IaC | Coding, code assistance, infrastructure-as-code, development support |
| AIOps Model Governance | Management, evaluation, adaptation, or governance of operational AI models |
| Human / Cross-cutting | Human-centered, organizational, or cross-stage DevOps activities |

### Coding rule

Use all relevant labels supported by the paper.

Example:

```text
Monitor; Operate; Incident/RCA
```

is valid if the study spans monitoring, operations, and incident diagnosis.

Consequently:

> RQ2 category counts are not mutually exclusive and must not be expected to sum to 60.

---

# 5. DevOps Activity Coding

`DevOps Activity` provides a finer-grained description than `DevOps Stage`.

Examples observed in the extraction include:

- KPI anomaly detection;
- real-time log anomaly detection;
- operational analytics;
- root-cause isolation;
- intermittent-job failure diagnosis;
- ML-based test-case prioritization;
- build outcome prediction;
- deployment optimization;
- automated remediation;
- AI-enabled security detection and response.

The activity field is descriptive rather than constrained to a single global controlled vocabulary.

When aggregating RQ2, these detailed activities are normalized into the final DevOps-stage taxonomy.

---

# 6. AI Category Coding

The final RQ3 taxonomy contains seven primary methodological classes:

| AI Category | Operational interpretation |
|---|---|
| Classical ML | Traditional supervised or statistical machine-learning approaches |
| Deep Learning | Neural-network methods beyond conventional ML, including LSTM/autoencoder-type architectures |
| Unsupervised / Anomaly AI | Unsupervised learning, clustering, anomaly-detection-oriented approaches |
| Optimization & RL | Optimization algorithms and reinforcement-learning approaches |
| NLP / Representation | NLP, text representation, embeddings, and representation-learning approaches primarily used for textual/software artifacts |
| Generative AI / LLM | Generative models and Large Language Model-based methods |
| Agentic / Multi-Agent | Autonomous or semi-autonomous AI agents and multi-agent systems |

### Primary-category rule for RQ3

Individual extraction records can describe hybrid methods.

For example:

```text
Optimization & RL / Classical ML
```

may appear when a study combines Random Forest prediction with an optimization algorithm.

However, the final RQ3 quantitative distribution uses **one normalized primary AI category per study**, so that:

```text
27 + 8 + 6 + 3 + 4 + 7 + 5 = 60
```

Final distribution:

```text
Classical ML              = 27
Deep Learning             = 8
Unsupervised / Anomaly AI = 6
Optimization & RL         = 3
NLP / Representation      = 4
GenAI / LLM               = 7
Agentic / Multi-Agent     = 5
Total                     = 60
```

### AIOps rule

AIOps is treated as:

> an application paradigm / operational context,

not as an algorithm category.

A paper can therefore be an AIOps study while its AI category is Classical ML, Deep Learning, GenAI/LLM, Agentic AI, or another methodological class.

---

# 7. AI Method / Model Field

`AI Method / Model` records the study-specific implementation rather than the normalized taxonomy.

Examples include:

- Random Forest;
- LSTM;
- LSTM Encoder–Decoder + Attention;
- autoencoders;
- clustering;
- learning-to-rank;
- NSGA-II;
- reinforcement learning;
- CodeBERT/BGE encoders;
- Large Language Models;
- multi-agent architectures.

This field should preserve technical specificity even when the study is normalized into a broader RQ3 category.

---

# 8. Industrial Context Coding

`Industrial Context` records the environment in which evidence was generated.

Examples include:

- production cloud systems;
- organizational O&M datasets;
- proprietary industrial logs;
- open-source CI projects;
- controlled cloud-native testbeds;
- public benchmark datasets;
- simulated operational environments.

This field supports interpretation of external validity and the benchmark-to-production gap.

It should not be collapsed automatically into a binary industrial/non-industrial flag if the original context contains more informative detail.

---

# 9. Evidence Type and Evidence Strength

`Evidence Type` retains descriptive information about how a study was evaluated.

Examples include:

```text
Production AIOps case study
Industrial failure-log evaluation
Multi-project benchmark
Controlled security/testbed evaluation
Multi-source controlled empirical evaluation
```

`Evidence Strength` normalizes this into one of six categories:

| Evidence Strength | Operational meaning |
|---|---|
| Production | Evidence from actual production operation or deployment |
| Industrial Empirical | Empirical evidence using industrial systems/data without necessarily demonstrating full production deployment |
| Controlled Experimental | Controlled experimental evaluation or testbed study |
| Benchmark | Evaluation primarily against benchmark datasets/projects or comparative benchmarks |
| Simulation | Evidence primarily produced through simulation |
| Conceptual | Framework, architecture, proof-of-concept, or conceptual evidence without strong empirical deployment validation |

### Interpretation rule

Evidence Strength describes the **strength and context of empirical support**, not methodological quality.

Therefore:

```text
QA PASS ≠ Production evidence
```

and:

```text
Conceptual evidence can pass QA
```

if it satisfies the minimum quality criteria.

---

# 10. Benefit Coding for RQ4

The final qualitative benefit taxonomy contains seven themes:

| Code | Benefit Theme |
|---|---|
| B1 | Speed & Efficiency |
| B2 | Accuracy & Detection Quality |
| B3 | Reliability & Availability |
| B4 | Cost & Resource Optimization |
| B5 | Automation & Toil Reduction |
| B6 | Security Improvement |
| B7 | Human Decision Support & Productivity |

The `Benefits` field retains paper-level evidence in narrative form.

The B1–B7 taxonomy is used for thematic synthesis.

### Important restriction

The current repository does not contain a complete reproducible record-level B1–B7 recoding matrix for all 60 studies.

Therefore:

> Do not report corpus-wide B1–B7 frequencies unless a new complete record-level recoding is performed and stored.

---

# 11. Challenge, Limitation, and Future-Work Coding for RQ5

Paper-level evidence is preserved separately in:

```text
Challenges
Limitations
Future Work
```

These fields were synthesized into cross-study research gaps:

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

and future-research directions:

```text
FR1 — Production-Validated AI-for-DevOps
FR2 — Adaptive and Generalizable AIOps
FR3 — Trustworthy and Explainable LLM-AIOps
FR4 — Safe and Cost-Efficient Agentic DevOps
FR5 — Human-Centered Autonomous DevOps
```

The gap/future-research taxonomy is an analytical synthesis derived from study-level evidence, not a claim that every primary paper used these exact labels.

---

# 12. RQ Mapping

The `RQ Mapping` field records which Research Questions are supported by the extracted study.

The final Research Questions are:

```text
RQ1 — Research trends, 2016–2026
RQ2 — DevOps stages/activities where AI is applied
RQ3 — AI techniques/methods/technologies used
RQ4 — Benefits and impacts
RQ5 — Challenges, limitations, and future research opportunities
```

Many included studies contribute to multiple or all RQs.

RQ mapping is therefore multi-label.

Example:

```text
RQ1–RQ5
```

means that the study provides extractable evidence relevant to all five RQs.

---

# 13. Field-to-RQ Relationship

| Extraction Field | Main RQ Use |
|---|---|
| Year | RQ1 |
| Publication Type | RQ1 / descriptive context |
| Research Type | RQ1 / evidence interpretation |
| DevOps Stage | RQ2 |
| DevOps Activity | RQ2 |
| AI Category | RQ3 |
| AI Method / Model | RQ3 |
| Dataset / System | RQ2–RQ5 context |
| Research Objective | Cross-RQ interpretation |
| Evaluation Method | RQ4–RQ5 evidence interpretation |
| Metrics | RQ4 |
| Main Findings | RQ2–RQ5 |
| Benefits | RQ4 |
| Challenges | RQ5 |
| Limitations | RQ5 |
| Future Work | RQ5 |
| Industrial Context | RQ4–RQ5 / external validity |
| Evidence Type | RQ4–RQ5 |
| Evidence Strength | RQ4–RQ5 |
| RQ Mapping | RQ1–RQ5 traceability |

Bibliographic fields such as Paper ID, Authors, Title, Source Database, Venue, and Publication Type primarily support study identity, auditability, and descriptive reporting.

---

# 14. Extraction Integrity Rules

A valid final extraction must satisfy:

```text
Included studies = 60
Paper IDs         = PS001–PS060
Unique PS IDs     = 60
Extraction fields = 26
```

The extraction must remain traceable to:

```text
PSxxx ↔ Uxxxx
```

and to the externally verified bibliography.

Controlled corrections should be applied when an extracted bibliographic value conflicts with a later externally verified ledger.

---

# 15. Known Recovery Constraints

The extraction master was recovered and reconciled after earlier data-loss/incompleteness issues.

Known constraints include:

1. PS009/PS047 required identity reconciliation because a recovered extraction version duplicated a title.
2. PS045 required controlled bibliographic-year correction to 2026.
3. Exact per-study numeric QA scores are unrecovered; canonical extraction records `PASS — exact score unrecovered`.
4. Not every thematic synthesis dimension has a complete record-level binary coding matrix; notably, corpus-wide B1–B7 prevalence is not reproducible from the current artifacts.

These constraints must be retained in supplementary documentation rather than silently repaired through inference.

---

# 16. Reproducibility Statement

The repository supports reproduction of:

- the 26-field extraction structure;
- the 60-study study-level evidence table;
- final PS identity;
- DevOps-stage synthesis;
- AI taxonomy synthesis;
- evidence-strength categorization;
- RQ1–RQ5 evidence lineage.

It does not justify reconstructing missing historical values that are not present in preserved evidence.

---

# 17. Status

**Data Extraction and Coding Framework: FINAL for the currently preserved evidence.**

Future changes must be treated as controlled corrections and propagated to the affected extraction dataset, synthesis artifact, context master, supplementary material, and manuscript where applicable.
