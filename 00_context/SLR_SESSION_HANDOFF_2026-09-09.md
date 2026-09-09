# SLR AI-for-DevOps — Session Handoff

**Updated: 9 September 2026 — publication-ready manuscript state**

## Purpose

Use this file as the first context file in a new ChatGPT session. It records the current authoritative project state and supersedes older handoff notes where they conflict.

## Locked scope

- Domain: Software Engineering
- Topic: **Artificial Intelligence for DevOps Automation**
- Period: **2016–2026**
- Search date: **7 September 2026**
- Boundary: **AI-for-DevOps**, excluding MLOps-only / DevOps-for-AI
- AI scope: AI, ML, Deep Learning, AIOps, Generative AI, LLM, AI Agents
- Databases: ScienceDirect, IEEE Xplore, ACM Digital Library
- Methodology: Kitchenham & Charters + PICOC + PRISMA 2020
- Citation style: IEEE
- Synthesis: descriptive quantitative + qualitative thematic; no statistical meta-analysis

## Locked Research Questions

- **RQ1:** research trends, 2016–2026
- **RQ2:** DevOps stages/activities where AI is applied
- **RQ3:** AI techniques/methods/technologies used
- **RQ4:** benefits and impacts
- **RQ5:** challenges, limitations, and future research opportunities

## Final PRISMA accounting

```text
Records identified from databases                    1,132
  ScienceDirect                                        185
  IEEE Xplore                                          765
  ACM Digital Library                                  180
Other/container records removed before screening         2
Bibliographic records entering deduplication          1,130
Duplicate occurrences removed                          317
Unique records screened                                813
Title/abstract records excluded                        431
Reports sought for retrieval                           382
Reports not retrieved                                  309
Reports retrieved / assessed                            73
Full-text reports excluded                              13
Studies included                                        60
```

Retrieval was attempted via Zotero for all 382 reports; only 73 full texts were obtained. The 309 are therefore validly classified as `Reports not retrieved`.

Full-text exclusions:
- FT3 — No AI/ML/GenAI/AIOps intervention: 2
- FT4 — MLOps only / DevOps-for-AI: 1
- FT5 — Secondary or non-primary publication: 7
- FT6 — Insufficient substantive evidence for RQs: 3

The authoritative PRISMA SVG is locked.

## QA and extraction

- QA: **60/60 assessed; 60 PASS; 0 FAIL**
- Threshold: **>= 3.0 / 5**
- PASS does not imply equal evidence strength.
- Data Extraction: **60/60 complete**
- Final schema: **26 fields**
- Evidence Strength: Production; Industrial Empirical; Controlled Experimental; Benchmark; Simulation; Conceptual

## PS/U mapping and bibliography

- 60 included `Uxxxx` records recovered.
- `PS001–PS060 ↔ Uxxxx`: **60/60 one-to-one mapping complete**
- Known anchor cross-checks: **16/16 PASS**
- Primary-study DOI coverage: **60/60**
- External bibliographic verification: **60/60 complete**
- Background references: **[1]–[6]**
- Primary-study references: **[7]–[66]**
- Citation integrity audit: PASS
- `PSxxx` identifiers remain only in the primary-study overview table as traceability IDs.

Recovery exception:
- recovered extraction master duplicated *Commit Artifact Preserving Build Prediction* into PS009 and PS047;
- PS047 is independently verified as `U0459`;
- the unique remaining included record `U0669` resolves PS009 to *Predicting build outcomes in continuous integration using textual analysis of source code commits*.

## PS045 final resolution

**PS045 is final = 2026.**

- `PS045 ↔ U0041`
- Title: *ARM: Autonomous Remediation and Management With LLM Agents for Intent-Driven Control*
- Venue: IEEE Internet of Things Journal
- Bibliographic year: **2026**
- DOI: `10.1109/JIOT.2025.3648858`

The 2025 date reflects early-access/DOI timing; the final bibliographic issue year is 2026.

Final RQ1 distribution:

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
Total=60
```

## RQ1–RQ5 locked synthesis

### RQ1
Trajectory: **Predictive AI → Diagnostic AIOps → Generative AI → Agentic AI**

### RQ2
- Monitor / Observability: 35 (58.3%)
- Operate / Operations: 31 (51.7%)
- Incident / RCA / Remediation: 17 (28.3%)
- Test: 16 (26.7%)
- Build / CI: 10 (16.7%)
- Deploy / Release: 9 (15.0%)
- Develop / Code / IaC: 3 (5.0%)
- AIOps Model Governance: 3 (5.0%)
- Human / Cross-cutting: 1 (1.7%)

Main interpretation: **shift-right concentration** toward Monitor → Operate → Incident/RCA.

### RQ3
Taxonomy:
Classical ML | Deep Learning | Unsupervised/Anomaly AI | Optimization & RL | NLP/Representation | GenAI/LLM | Agentic/Multi-Agent

Primary distribution:
27 | 8 | 6 | 3 | 4 | 7 | 5

AIOps = application paradigm, not algorithm.

### RQ4
Benefit themes:
B1 Speed & Efficiency; B2 Accuracy & Detection Quality; B3 Reliability & Availability; B4 Cost & Resource Optimization; B5 Automation & Toil Reduction; B6 Security Improvement; B7 Human Decision Support & Productivity.

Do not invent corpus-wide B1–B7 frequencies.

Core interpretation:
**technical capability is developing faster than demonstrated production benefit**, especially for LLM/agentic approaches.

### RQ5
Research gaps:
G1 Production-scale validation; G2 Cross-system generalization; G3 Concept drift & long-term maintenance; G4 Explainability/trust/reliability; G5 Autonomous-remediation safety; G6 LLM/agent cost & latency; G7 Human–AI collaboration & adoption; G8 Unified ML + DevOps operational evaluation.

Future agenda:
FR1 Production-Validated AI-for-DevOps; FR2 Adaptive and Generalizable AIOps; FR3 Trustworthy and Explainable LLM-AIOps; FR4 Safe and Cost-Efficient Agentic DevOps; FR5 Human-Centered Autonomous DevOps.

Long-term trajectory:
**Predictive → Diagnostic → Generative → Agentic → Trustworthy Autonomous DevOps**

## Manuscript status

Locked:
- Abstract + Keywords
- Section 1 — Introduction
- Section 2 — Background
- Section 3 — Research Methodology
- Section 4 — Results
- Section 5 — Discussion
- Section 6 — Threats to Validity
- Section 7 — Conclusion
- PRISMA authoritative SVG
- IEEE citations [1]–[66]
- References
- PS045 year = 2026

Controlled correction applied:
- Section 4.2 RQ1 counts updated to 2025=8 and 2026=12.
- Section 6.4 obsolete PS045 uncertainty paragraph removed.
- Primary-study overview PS045 year updated to 2026.

Current publication-ready manuscript:
`SLR_AI_DevOps_PUBLICATION_READY_FINAL_2026-09-09.docx`

## Current remaining work

1. **Appendices / Supplementary Material**
2. Optional final formatting to a specific university/journal template
3. Optional export to PDF
4. Final submission package / repository cleanup

## Recommended next action

> Start with **Appendices / Supplementary Material**. Do not reopen locked manuscript sections unless a concrete evidence or formatting issue is found.

## Continuation prompt

> Use `SLR_SESSION_HANDOFF_2026-09-09.md` and `SLR_CONTEXT_MASTER_2026-09-09.md` as authoritative current state. The SLR body, PRISMA, PS001–PS060↔Uxxxx mapping, PS045=2026, IEEE citations [1]–[66], references, and publication-ready DOCX are finalized. Do not revert to the old PS045 uncertainty or provisional 2025=9/2026=11 RQ1 counts. Next step: build appendices/supplementary material and final submission package.
