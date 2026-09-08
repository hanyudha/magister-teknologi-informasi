# SLR AI-for-DevOps --- Evidence & Synthesis Ledger

**Updated: 8 September 2026 --- post RQ1--RQ5 finalization**

## Evidence rules

-   Corpus: PS001--PS060.
-   QA: all PASS, but evidence strength differs.
-   Benchmark/controlled metrics ≠ production impact.
-   No statistical meta-analysis across heterogeneous metrics.
-   Paper-derived fields: Main Findings, Benefits, Challenges,
    Limitations, Future Work.
-   SLR coding fields: DevOps Stage, AI Category, Research Type, RQ
    Mapping, Evidence Strength.
-   Evidence Strength uses the strongest evidence actually supported:
    Production; Industrial Empirical; Controlled Experimental;
    Benchmark; Simulation; Conceptual.

## RQ1 --- Trends

Provisional distribution: 2016=0; 2017=0; 2018=0; 2019=3; 2020=7;
2021=4; 2022=7; 2023=7; 2024=12; 2025=9; 2026=11.

PS045 provisional=2025; if resolved as 2026, 2025=8 and 2026=12.

Trajectory: **Predictive AI → Diagnostic AIOps → Generative AI → Agentic
AI**

Interpretation: - 2019--2021: classical ML / early DL,
prediction/classification. - 2022--2023: broader AIOps, anomaly
detection, monitoring, incident intelligence, forecasting. - 2024--2026:
GenAI/LLM, semantic reasoning, RCA generation, decision support. -
2025--2026: agentic AIOps, tool use, planning, autonomous remediation. -
New technologies accumulate rather than fully replace classical ML. -
Some older classical-ML studies have stronger production evidence than
newer agentic studies.

## RQ2 --- DevOps application areas

Multi-label: - Monitor / Observability: 35 (58.3%) - Operate /
Operations: 31 (51.7%) - Incident / RCA / Remediation: 17 (28.3%) -
Test: 16 (26.7%) - Build / CI: 10 (16.7%) - Deploy / Release: 9
(15.0%) - Develop / Code / IaC: 3 (5.0%) - AIOps Model Governance: 3
(5.0%) - Human / Cross-cutting: 1 (1.7%)

Primary application areas: - Incident Management, Diagnosis, RCA &
Remediation: 16 (26.7%) - Monitoring & Anomaly Detection: 13 (21.7%) -
Testing & Test Prioritization: 10 (16.7%) - Resource / Performance /
Deployment Optimization: 6 (10.0%) - Security / DevSecOps: 5 (8.3%) -
Build / CI Prediction: 4 (6.7%) - AIOps Model Governance /
Interpretation: 3 (5.0%) - Cross-cutting DevOps Automation: 2 (3.3%) -
Human / Organizational Impact: 1 (1.7%)

Main finding: **shift-right concentration** toward Monitor → Operate →
Incident/RCA.

Automation maturity: Assist → Predict → Diagnose → Recommend → Act.

## RQ3 --- AI taxonomy

Final taxonomy: 1. Classical Machine Learning 2. Deep Learning 3.
Unsupervised / Anomaly AI 4. Optimization & Reinforcement Learning 5.
NLP / Representation Learning 6. Generative AI / LLM 7. Agentic /
Multi-Agent AI

AIOps = application paradigm/context, not algorithm.

Primary-category chart distribution, mutually exclusive: - Classical ML:
27 (45.0%) - Deep Learning: 8 (13.3%) - Generative AI / LLM: 7 (11.7%) -
Unsupervised / Anomaly AI: 6 (10.0%) - Agentic / Multi-Agent AI: 5
(8.3%) - NLP / Representation Learning: 4 (6.7%) - Optimization & RL: 3
(5.0%)

Evolution: **Model → Pipeline → Reasoning System → Agentic System**

## RQ4 --- Benefits and impacts

Benefit themes: - B1 Speed & Efficiency - B2 Accuracy & Detection
Quality - B3 Reliability & Availability - B4 Cost & Resource
Optimization - B5 Automation & Toil Reduction - B6 Security
Improvement - B7 Human Decision Support & Productivity

**Frequency guardrail:** corpus-wide B1--B7 frequencies are not
reproducibly available in the locked source. Do not invent them. The
final RQ4 chart uses 16 representative evidence anchors only.

Representative evidence anchors: - PS056 Facebook Predictive Test
Selection --- \~2× testing infrastructure cost reduction; \>95%
individual failures; \>99.9% faulty changes --- **Production**. - PS057
Alibaba node failure prediction --- AUC \~0.92; daily DevOps use ---
**Production**. - PS060 GPT-4 RCA --- \>100k production incidents;
\~24.8% improvement vs fine-tuned GPT-3; human correctness +43.5%;
readability +8.7% --- **Industrial Empirical**. - PS012 DeCaf Microsoft
--- 4× more valid issues; precision 0.72 vs 0.66 --- **Production**. -
PS036 topology-aware active LLM observability --- F1 0.95 vs 0.65;
telemetry bandwidth -84%; estimated TCO -12.5% --- **Simulation; phrase
cautiously**. - PS042 LLM log prioritization --- raw logs -76% ---
**Industrial Empirical**. - PS047 GitSense --- large F1/precision/recall
improvements; \~0.017s/sample --- **Benchmark; not production
impact**. - PS049 graph multi-agent RCA --- average F1 88.4%; \~9.7K
tokens/fault; 21.4s runtime --- **Benchmark; exposes quality/cost
trade-off**. - PS025 HIDELS --- DT accuracy 99.5361%; ensemble F1 99.7%;
overhead 5--8% --- **Controlled Experimental**. - PS032 proactive
autoscaling --- ensemble more consistent; full autonomy rejected by IT
department due production risk --- **Industrial Empirical**. - PS005
AI-Augmented DevSecOps --- \>95% attack detection; \<5% FP; sub-2s
latency at 10k events/s; 85% zero-day detection --- **Controlled
Experimental**. - PS007 TELUS few-shot LM --- 84.3% Macro F1; 92.0%
Top-2; log-review scope -74.4%; 87% selected segments relevant ---
**Industrial Empirical**. - PS023 Monitorless --- up to 97% accuracy ---
**Controlled Experimental**. - PS024 persistence suppression --- invalid
anomalies reduced \>=28% --- **Controlled Experimental**. - PS045 ARM
--- SLA violation detection 52.9%; mitigation success 70.7% ---
**Controlled Experimental**. - PS050 DualLane --- median plan execution
4.2s; total response 8.5s; judge-human agreement 98% --- **Industrial
Empirical**.

Core conclusion: **technical capability is developing faster than
demonstrated production benefit**, particularly for LLM/agentic AIOps.

## RQ5 --- Challenges and limitations

Qualitative themes; do not invent corpus-wide frequencies: 1. Data
Quality & Availability 2. Class Imbalance 3. Data Leakage & Unrealistic
Evaluation 4. Concept Drift & Model Decay 5. Limited Generalizability 6.
Benchmark-to-Production Gap 7. Explainability & Trust 8. LLM
Hallucination & Reliability 9. Cost, Latency & Resource Consumption 10.
Integration Complexity 11. Safety of Autonomous Remediation 12.
Human-in-the-Loop 13. Security & Privacy 14. Evaluation Metric
Inconsistency

Recommended future evaluation: combine ML metrics with DevOps
operational metrics, e.g. F1/AUC + MTTR + latency + operational cost +
resource use + false-alert burden + human effort.

## Research gaps --- locked

-   **G1** Production-scale validation insufficient --- Highest
-   **G2** Cross-system/organization generalization limited --- High
-   **G3** Concept drift & long-term maintenance under-studied --- High
-   **G4** Explainability, trust & reliability immature --- High
-   **G5** Autonomous-remediation safety mechanisms immature --- Highest
-   **G6** LLM/multi-agent cost, latency & resources under-evaluated ---
    Emerging/High
-   **G7** Human--AI collaboration & organizational adoption
    under-studied --- Emerging/High
-   **G8** No consistent integrated ML + DevOps operational evaluation
    framework --- Highest

Central gap: \> Despite increasingly advanced AI capabilities in DevOps,
a substantial gap remains between experimental capability and
trustworthy production-scale automation. Future work needs to move
beyond model performance toward production-ready, adaptive, explainable,
cost-aware, safely autonomous systems evaluated using real operational
outcomes.

## Future research agenda --- locked

-   FR1 Production-Validated AI-for-DevOps
-   FR2 Adaptive and Generalizable AIOps
-   FR3 Trustworthy and Explainable LLM-AIOps
-   FR4 Safe and Cost-Efficient Agentic DevOps
-   FR5 Human-Centered Autonomous DevOps

Roadmap: **Predictive → Diagnostic → Generative → Agentic → Trustworthy
Autonomous DevOps**

## Claims to avoid

Do not claim: - AI replaces DevOps/SRE engineers. - Agentic systems are
broadly production-ready. - Higher F1/AUC automatically means lower MTTR
or production benefit. - RQ4 B1--B7 or RQ5 challenge frequencies across
all 60 studies unless re-coded from record-level extraction. - PS045
year is final. - The two pre-screening container records were specific
publication types unless evidence is recovered.
