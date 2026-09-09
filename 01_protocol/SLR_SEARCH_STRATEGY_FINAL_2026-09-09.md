# SLR Search Strategy — Final Operational Record

**Project:** Artificial Intelligence in DevOps Automation  
**Review period:** 2016–2026  
**Search execution date:** 7 September 2026  
**Authoritative state date:** 9 September 2026  
**Databases:** ScienceDirect, IEEE Xplore, ACM Digital Library  
**Methodological basis:** Kitchenham & Charters + PICOC + PRISMA 2020

---

## 1. Purpose

This file documents the search strategy actually supported by the preserved SLR repository artifacts.

It intentionally distinguishes between:

1. the **conceptual/PICOC search framework**;
2. **preliminary Boolean strings** developed during protocol design;
3. the **operational search groups and result counts** preserved in the final search logs and RIS exports; and
4. platform-specific exact query syntax that was **not fully preserved**.

This distinction prevents a preliminary query from being retrospectively presented as an exact executed query.

---

## 2. Review Scope

The review focuses on **Artificial Intelligence for DevOps Automation** in Software Engineering.

### Included conceptual scope

DevOps-related concepts include:

- DevOps;
- CI/CD;
- continuous integration;
- continuous delivery;
- continuous deployment;
- software delivery;
- AIOps-related operational contexts.

AI-related scope includes:

- Artificial Intelligence;
- Machine Learning;
- Deep Learning;
- Generative AI;
- Large Language Models;
- AIOps;
- related AI-enabled automation approaches.

### Boundary condition

The review targets **AI-for-DevOps**.

MLOps-only / DevOps-for-AI studies are excluded unless AI is explicitly used to improve a DevOps activity.

---

## 3. PICOC Framework

| PICOC Element | Operational Definition |
|---|---|
| Population | DevOps practices, processes, pipelines, CI/CD, and software delivery |
| Intervention | Artificial Intelligence, Machine Learning, Deep Learning, Generative AI, Large Language Models, and AIOps |
| Comparison | Traditional or non-AI DevOps approaches, where available; comparison was not mandatory |
| Outcomes | Automation, efficiency, reliability, software quality, deployment performance, incident resolution, and related operational outcomes |
| Context | Software engineering, software development, and software operations |

PICOC was used to define the review scope and organize the search concepts. It was not treated as evidence that every platform used exactly the same Boolean syntax.

---

## 4. Preliminary Boolean Search Strings

The protocol-development archive contains preliminary Boolean strings such as:

```text
("DevOps" OR "CI/CD" OR "continuous integration" OR "continuous delivery"
OR "continuous deployment")
AND
("artificial intelligence" OR "machine learning" OR "deep learning"
OR "generative AI" OR "large language model" OR "LLM" OR "AIOps")
```

A more targeted preliminary form was also documented:

```text
("DevOps" OR "DevOps automation" OR "CI/CD"
OR "continuous integration" OR "continuous delivery"
OR "continuous deployment")
AND
("artificial intelligence" OR "machine learning"
OR "generative AI" OR "large language model"
OR "LLM" OR "AIOps")
AND
("automation" OR "optimization" OR "monitoring"
OR "deployment" OR "incident" OR "operations")
```

### Provenance warning

These strings were explicitly recorded during protocol development as **preliminary / not yet final**.

Therefore:

> They must not be described as the exact final executed search strings unless new direct evidence of the platform-specific query execution is recovered.

The final manuscript correctly reports the operational search logs rather than retroactively asserting these preliminary strings as exact executed queries.

---

## 5. Final Operational Search Design

The final search was executed on **7 September 2026** using three primary databases:

1. ScienceDirect
2. IEEE Xplore
3. ACM Digital Library

Seven search-focus groups were used operationally:

| Group | Search focus |
|---|---|
| 01 | `"DevOps"` + AI terms |
| 02 | `"CI/CD"` + AI terms |
| 03 | `"continuous integration"` + AI terms |
| 04 | `"continuous delivery"` + AI terms |
| 05 | `"continuous deployment"` + AI terms |
| 06 | `"software delivery"` + AI terms |
| 07 | `"AIOps"` |

The phrase **“AI terms”** is preserved in the operational logs as a conceptual group. The exact database-specific textual syntax used to combine those AI terms was not fully retained in the repository.

---

# 6. ScienceDirect

## 6.1 Search configuration

**Search field:** Title, abstract or author-specified keywords  
**Publication period:** 2016–2026  
**Search date:** 7 September 2026

## 6.2 Operational search results

| ID | Focus | Results |
|---|---|---:|
| SD-01 | `"DevOps"` + AI terms | 48 |
| SD-02 | `"CI/CD"` + AI terms | 28 |
| SD-03 | `"continuous integration"` + AI terms | 50 |
| SD-04 | `"continuous delivery"` + AI terms | 11 |
| SD-05 | `"continuous deployment"` + AI terms | 12 |
| SD-06 | `"software delivery"` + AI terms | 3 |
| SD-07 | `"AIOps"` | 33 |
|  | **Total** | **185** |

## 6.3 Preserved RIS exports

```text
02_search/raw/sciencedirect/
├── SD-01_DevOps_AI_2016-2026_2026-09-07.ris
├── SD-02_CICD_AI_2016-2026_2026-09-07.ris
├── SD-03_ContinuousIntegration_AI_2016-2026_2026-09-07.ris
├── SD-04_ContinuousDelivery_AI_2016-2026_2026-09-07.ris
├── SD-05_ContinuousDeployment_AI_2016-2026_2026-09-07.ris
├── SD-06_SoftwareDelivery_AI_2016-2026_2026-09-07.ris
└── SD-07_AIOps_2016-2026_2026-09-07.ris
```

Independent record counting of the preserved RIS files reproduces:

```text
48 + 28 + 50 + 11 + 12 + 3 + 33 = 185
```

Thus the ScienceDirect operational log and preserved export set reconcile exactly.

---

# 7. IEEE Xplore

## 7.1 Search configuration

**Search field:** Abstract  
**Publication types:** Conferences + Journals  
**Publication period:** 2016–2026

For the AIOps search group, the requested period was 2016–2026, while the actual returned records were within 2019–2026.

## 7.2 Operational search results

| ID | Focus | Results |
|---|---|---:|
| IE-01 | `"DevOps"` + AI terms | 179 |
| IE-02 | `"CI/CD"` + AI terms | 129 |
| IE-03 | `"continuous integration"` + AI terms | 159 |
| IE-04 | `"continuous delivery"` + AI terms | 38 |
| IE-05 | `"continuous deployment"` + AI terms | 53 |
| IE-06 | `"software delivery"` + AI terms | 23 |
| IE-07 | `"AIOps"` | 184 |
|  | **Total** | **765** |

## 7.3 Export batching

Search groups exceeding the platform/export batch size were stored in multiple RIS files.

Examples:

```text
IE-01:
  batch01 = 100
  batch02 = 79
  total   = 179

IE-02:
  batch01 = 100
  batch02 = 29
  total   = 129

IE-03:
  batch01 = 100
  batch02 = 59
  total   = 159

IE-07:
  batch01 = 100
  batch02 = 84
  total   = 184
```

Independent counting of the preserved IEEE RIS exports reproduces a total of:

```text
765 records
```

Thus the IEEE operational log and preserved export set reconcile exactly.

---

# 8. ACM Digital Library

## 8.1 Search configuration

**Search field:** Abstract  
**Publication period:** January 2016 – September 2026

The exact platform-specific ACM textual query syntax was not preserved in the available repository.

## 8.2 Operational search log

The search log records:

| ID | Focus | Search-log results |
|---|---|---:|
| ACM-01 | `"DevOps"` + AI terms | 38 |
| ACM-02 | `"CI/CD"` + AI terms | 15 |
| ACM-03 | `"continuous integration"` + AI terms | 46 |
| ACM-04 | `"continuous delivery"` + AI terms | 7 |
| ACM-05 | `"continuous deployment"` + AI terms | 9 |
| ACM-06 | `"software delivery"` + AI terms | 4 |
| ACM-07 | `"AIOps"` | 63 |
|  | **Initial search-log total** | **182** |

## 8.3 Preserved ACM RIS exports

The preserved RIS files contain:

| ID | Preserved RIS records |
|---|---:|
| ACM-01 | 38 |
| ACM-02 | 15 |
| ACM-03 | 46 |
| ACM-04 | 7 |
| ACM-05 | 8 |
| ACM-06 | 3 |
| ACM-07 | 63 |
| **Total** | **180** |

Thus:

```text
Initial ACM search-log results = 182
Preserved article records      = 180
Difference                     =   2
```

The project’s final PRISMA reconciliation classifies these two records as **proceedings/container records removed before article screening**.

The archived ACM RIS dataset therefore represents the **180 bibliographic article records retained for deduplication**, not the 182 initial result containers displayed in the operational search log.

This interpretation is consistent with:

```text
ACM initial results                  182
Container/proceedings records removed 2
ACM records entering deduplication   180
```

### Important limitation

The repository supports the numerical reconciliation above, but it does not preserve enough direct platform-query evidence to reconstruct the exact textual ACM query syntax character-for-character.

---

# 9. Cross-Database Identification Accounting

The final database contribution entering the SLR is:

| Database | Records |
|---|---:|
| ScienceDirect | 185 |
| IEEE Xplore | 765 |
| ACM Digital Library article records | 180 |
| **Bibliographic records entering deduplication** | **1,130** |

The PRISMA identification layer additionally retains the two ACM container/proceedings records that were removed before screening:

```text
1,130 bibliographic records
+    2 removed container/proceedings records
=1,132 records identified
```

Final identification accounting:

```text
Records identified from database searches = 1,132
Records removed before deduplication       =     2
Records entering deduplication             = 1,130
```

---

# 10. Search Evidence Locations

Operational logs:

```text
02_search/logs/
├── Search Log ScienceDirect (Chatgpt).txt
├── Search Log IEEE Xplore (Chatgpt).txt
└── Search Log ACM (Chatgpt).txt
```

Raw/preserved exports:

```text
02_search/raw/
├── sciencedirect/
├── ieee/
└── acm/
```

Downstream deduplication:

```text
03_screening/dedup/SLR_Master_Deduplication_2026-09-07.xlsx
```

Final PRISMA reconciliation:

```text
03_screening/prism-reconciliation/
SLR_Master_PRISMA_Reconciliation_382_2026-09-08_FINAL.xlsx
```

Supporting reconciliation narrative:

```text
07_prisma/SLR_PRISMA_RECONCILIATION_WORKSHEET_2026-09-09.md
```

---

# 11. Reproducibility Statement

The repository currently supports **operational reproducibility** of:

- database selection;
- search date;
- search focus groups;
- search fields;
- year filters;
- result counts;
- preserved RIS exports;
- database contribution totals;
- transition into deduplication.

The repository does **not** fully support character-for-character reconstruction of every platform-specific executed Boolean query.

Accordingly, publication and supplementary materials should use wording such as:

> The review used operational search logs preserved for ScienceDirect, IEEE Xplore, and ACM Digital Library. Search concepts were organized around DevOps/CI/CD terminology and AI-related terms using PICOC. Preliminary Boolean strings were documented during protocol development, but because exact platform-specific syntax was not fully preserved, these preliminary strings are not presented as exact executed queries.

This statement is more defensible than reconstructing exact syntax retrospectively.

---

# 12. Search Strategy Integrity Checks

A correct reproduction should satisfy:

```text
ScienceDirect RIS total = 185
IEEE Xplore RIS total   = 765
ACM preserved RIS total = 180

185 + 765 + 180 = 1,130
1,130 + 2 removed container records = 1,132
```

It should also preserve:

```text
Search date = 7 September 2026
Review period = 2016–2026
Databases = ScienceDirect + IEEE Xplore + ACM Digital Library
```

---

# 13. Status

**Search strategy documentation: FINAL for the currently preserved evidence.**

This file may only be revised if:

1. new primary search-execution evidence is recovered;
2. a database-specific exact query log is found; or
3. a controlled correction is made to the identification accounting.

Do not replace the operational record with reconstructed assumptions.
