# SLR CONTEXT MASTER — AI-for-DevOps

**Updated: 9 September 2026**

## Project identity

- Field: Software Engineering
- Topic: Artificial Intelligence for DevOps Automation
- Period: 2016–2026
- Search date: 7 September 2026
- Databases: ScienceDirect, IEEE Xplore, ACM Digital Library
- Guideline: Kitchenham & Charters
- PICOC: scope/search
- PRISMA 2020: selection reporting
- Citation: IEEE
- Synthesis: descriptive quantitative + qualitative thematic
- Statistical meta-analysis: no

## Final title

**Artificial Intelligence in DevOps Automation: A Systematic Literature Review of Applications, Benefits, Challenges, and Research Trends from 2016 to 2026**

## Scope boundary

AI-for-DevOps only. Exclude MLOps-only / DevOps-for-AI unless AI is explicitly used to improve a DevOps activity.

## RQs

RQ1 trends; RQ2 DevOps stages/activities; RQ3 AI methods/technologies; RQ4 benefits/impacts; RQ5 challenges/limitations/future opportunities.

## PRISMA final

```text
Identified=1,132
ScienceDirect=185
IEEE Xplore=765
ACM DL=180
Removed before screening=2
Entering deduplication=1,130
Duplicate occurrences removed=317
Unique screened=813
Title/abstract excluded=431
Reports sought=382
Reports not retrieved=309
Reports retrieved/assessed=73
Full-text excluded=13
Included=60
Pending=0
```

FT exclusions: FT3=2; FT4=1; FT5=7; FT6=3.

## QA

QA1 objective clear; QA2 DevOps+AI clear; QA3 method/evaluation adequate; QA4 results evidence-supported; QA5 limitations/threats/implications.
Threshold >=3.0/5.
60/60 PASS.
QA PASS != equal evidence strength.

## Extraction

26 fields:
Paper ID | Authors | Year | Title | Source Database | Venue | Publication Type | Research Type | DevOps Stage | DevOps Activity | AI Category | AI Method/Model | Dataset/System | Research Objective | Evaluation Method | Metrics | Main Findings | Benefits | Challenges | Limitations | Future Work | RQ Mapping | QA Score | Industrial Context | Evidence Type | Evidence Strength

Evidence Strength:
Production | Industrial Empirical | Controlled Experimental | Benchmark | Simulation | Conceptual

## Study identity

- 60 included U IDs recovered.
- PS001–PS060 ↔ Uxxxx = 60/60 one-to-one.
- DOI coverage = 60/60.
- External bibliographic verification = 60/60.
- Background refs = [1]–[6].
- Primary refs = [7]–[66].
- Citation integrity = PASS.

Recovery exception:
recovered extraction master duplicated the PS047 title into PS009. PS047→U0459 is independently verified; PS009 uniquely reconciles to U0669.

## PS045 final

PS045→U0041
Year=2026
DOI=10.1109/JIOT.2025.3648858
Venue=IEEE Internet of Things Journal

Final RQ1:
2016=0; 2017=0; 2018=0; 2019=3; 2020=7; 2021=4; 2022=7; 2023=7; 2024=12; 2025=8; 2026=12.

## RQ1
Predictive AI → Diagnostic AIOps → Generative AI → Agentic AI

## RQ2
Monitor/Observability 35; Operate 31; Incident/RCA/Remediation 17; Test 16; Build/CI 10; Deploy/Release 9; Develop/Code/IaC 3; AIOps Model Governance 3; Human/Cross-cutting 1.

Interpretation: Monitor → Operate → Incident/RCA.
Automation lens: Assist → Predict → Diagnose → Recommend → Act.

## RQ3
Classical ML 27; Deep Learning 8; GenAI/LLM 7; Unsupervised/Anomaly 6; Agentic/Multi-Agent 5; NLP/Representation 4; Optimization/RL 3.
AIOps = application paradigm.
Evolution: Model → Pipeline → Reasoning System → Agentic System.

## RQ4
B1 Speed & Efficiency
B2 Accuracy & Detection Quality
B3 Reliability & Availability
B4 Cost & Resource Optimization
B5 Automation & Toil Reduction
B6 Security Improvement
B7 Human Decision Support & Productivity

No reproducible corpus-wide B1–B7 prevalence.
Core interpretation: technical capability is developing faster than demonstrated production benefit.

## RQ5
Challenges: data quality; imbalance; leakage/unrealistic evaluation; drift; generalization; benchmark-production gap; explainability/trust; LLM hallucination/reliability; cost/latency/resources; integration; remediation safety; human oversight; security/privacy; metric inconsistency.

Gaps:
G1 Production-scale validation
G2 Cross-system generalization
G3 Concept drift & long-term maintenance
G4 Explainability/trust/reliability
G5 Autonomous-remediation safety
G6 LLM/agent cost & latency
G7 Human-AI collaboration/adoption
G8 Unified ML+DevOps operational evaluation

Priority: highest G1,G5,G8; high G2,G3,G4; emerging/high G6,G7.

FR1 Production-Validated AI-for-DevOps
FR2 Adaptive and Generalizable AIOps
FR3 Trustworthy and Explainable LLM-AIOps
FR4 Safe and Cost-Efficient Agentic DevOps
FR5 Human-Centered Autonomous DevOps

Long-term trajectory:
Predictive → Diagnostic → Generative → Agentic → Trustworthy Autonomous DevOps

## Claims to avoid

Do not claim:
- AI replaces DevOps/SRE engineers.
- Agentic systems are broadly production-ready.
- Higher F1/AUC automatically means lower MTTR.
- Benchmark evidence equals production impact.
- Corpus-wide B1–B7 or challenge frequencies exist without record-level recoding.
- PS045 is unresolved.
- RQ1 2025=9 and 2026=11.
- the two removed pre-screening records had specific publication types.

## Manuscript

Locked: Abstract+Keywords; Sections 1–7; PRISMA; citations [1]–[66]; References; PS045=2026.

Current publication-ready manuscript:
`SLR_AI_DevOps_PUBLICATION_READY_FINAL_2026-09-09.docx`

## Next work

1. Appendices / Supplementary Material
2. Optional template-specific formatting
3. Optional final PDF
4. Repository finalization / submission package
