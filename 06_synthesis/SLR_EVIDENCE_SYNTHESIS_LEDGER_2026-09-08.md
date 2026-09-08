# SLR AI-for-DevOps — Evidence & Synthesis Ledger
**Updated: 8 September 2026**

## Rules
Corpus PS001–PS060. QA all PASS but evidence strength differs. Benchmark ≠ production impact.
No statistical meta-analysis across heterogeneous metrics.

## RQ1
2016–18=0; 2019=3; 2020=7; 2021=4; 2022=7; 2023=7; 2024=12; 2025=9; 2026=11.
PS045 provisional=2025. Predictive → Diagnostic → Generative → Agentic.

## RQ2
Monitor 35; Operate 31; Incident/RCA 17; Test 16; Build 10; Deploy 9; Develop/IaC 3;
Model Governance 3; Human 1. Strong shift-right concentration.

## RQ3
Classical ML; DL; Unsupervised/Anomaly; Optimization/RL; NLP/Representation;
GenAI/LLM; Agentic/Multi-Agent. AIOps is context, not algorithm.

## RQ4 benefit themes
B1 Speed & Efficiency; B2 Accuracy & Detection Quality; B3 Reliability & Availability;
B4 Cost & Resource Optimization; B5 Automation & Toil Reduction; B6 Security Improvement;
B7 Human Decision Support & Productivity.

Representative anchors:
- PS056 Facebook PTS: ~2x testing infrastructure cost reduction; >95% individual failures;
  >99.9% faulty changes — Production.
- PS057 Alibaba: AUC ~0.92; daily DevOps use — Production.
- PS060 GPT-4 RCA: >100k incidents; ~24.8% improvement vs fine-tuned GPT-3;
  human correctness +43.5% — Industrial Empirical.
- PS012 DeCaf: 4x more valid issues; precision .72 vs .66 — Production.
- PS042 log prioritization: raw logs -76% — Industrial Empirical.
- PS049 multi-agent RCA: avg F1 88.4%; ~9.7K tokens/fault; 21.4s — Benchmark.

## RQ5 challenges
Data/labels; imbalance; temporal leakage; drift; generalization; benchmark-production gap;
explainability/trust; hallucination; cost/latency; integration; remediation safety;
human oversight; privacy/security; non-standard evaluation.

## Gaps
G1 Production validation; G2 Generalization; G3 Drift/lifecycle; G4 Trust/explainability;
G5 Remediation safety; G6 Cost/latency; G7 Human-AI/adoption; G8 Integrated evaluation.

## Future directions
FR1 Production-Validated; FR2 Adaptive/Generalizable; FR3 Trustworthy/Explainable LLM-AIOps;
FR4 Safe/Cost-Efficient Agentic DevOps; FR5 Human-Centered Autonomous DevOps.

## Claims to avoid
Do not claim AI replaces engineers; agents are broadly production-ready; higher F1 guarantees
lower MTTR; all 382 reports were retrieved; 309 were all unavailable; PS045 year is final.
