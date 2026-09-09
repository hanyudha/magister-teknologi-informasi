# Appendix A — Search Strategy

The systematic search was designed using PICOC to operationalize the review scope around DevOps practices and AI-enabled automation. The Population covered DevOps processes, pipelines, CI/CD, and software delivery; the Intervention covered Artificial Intelligence, Machine Learning, Deep Learning, Generative AI, Large Language Models, and AIOps. Comparisons with non-AI approaches were considered where available but were not mandatory. Outcomes included automation, efficiency, reliability, software quality, deployment performance, incident resolution, and related operational effects, within software engineering, software development, and software operations contexts.

The final literature search was conducted on **7 September 2026** in **ScienceDirect, IEEE Xplore, and ACM Digital Library**, covering publications from **2016 to 2026**. Operational search groups were organized around seven DevOps-related concepts: `"DevOps"`, `"CI/CD"`, `"continuous integration"`, `"continuous delivery"`, `"continuous deployment"`, `"software delivery"`, and `"AIOps"`. The first six groups were combined operationally with AI-related terms; AIOps was also searched as a dedicated group.

The review preserves operational search logs and RIS exports for all three databases. Preliminary Boolean strings were developed during protocol design, but the exact platform-specific textual syntax used in every final query was not fully preserved. Therefore, those preliminary strings are not reported as exact executed queries. This avoids retrospectively reconstructing query syntax that cannot be verified from the preserved evidence.

## A.1 ScienceDirect

ScienceDirect searches were performed in the **Title, abstract or author-specified keywords** field for 2016–2026.

| Search ID | Focus | Results |
|---|---|---:|
| SD-01 | `"DevOps"` + AI terms | 48 |
| SD-02 | `"CI/CD"` + AI terms | 28 |
| SD-03 | `"continuous integration"` + AI terms | 50 |
| SD-04 | `"continuous delivery"` + AI terms | 11 |
| SD-05 | `"continuous deployment"` + AI terms | 12 |
| SD-06 | `"software delivery"` + AI terms | 3 |
| SD-07 | `"AIOps"` | 33 |
|  | **Total** | **185** |

The seven preserved ScienceDirect RIS exports independently reproduce the total of **185 records**.

## A.2 IEEE Xplore

IEEE Xplore searches used the **Abstract** field, restricted to **conference and journal publications** for 2016–2026.

| Search ID | Focus | Results |
|---|---|---:|
| IE-01 | `"DevOps"` + AI terms | 179 |
| IE-02 | `"CI/CD"` + AI terms | 129 |
| IE-03 | `"continuous integration"` + AI terms | 159 |
| IE-04 | `"continuous delivery"` + AI terms | 38 |
| IE-05 | `"continuous deployment"` + AI terms | 53 |
| IE-06 | `"software delivery"` + AI terms | 23 |
| IE-07 | `"AIOps"` | 184 |
|  | **Total** | **765** |

Several result sets were exported in batches because they exceeded individual export batch sizes. The preserved IEEE RIS files reproduce **765 records** in total. For the AIOps group, the requested date range was 2016–2026, although the returned records were within 2019–2026.

## A.3 ACM Digital Library

ACM Digital Library searches used the **Abstract** field and covered January 2016 through September 2026.

| Search ID | Focus | Initial results in search log | Preserved article RIS |
|---|---|---:|---:|
| ACM-01 | `"DevOps"` + AI terms | 38 | 38 |
| ACM-02 | `"CI/CD"` + AI terms | 15 | 15 |
| ACM-03 | `"continuous integration"` + AI terms | 46 | 46 |
| ACM-04 | `"continuous delivery"` + AI terms | 7 | 7 |
| ACM-05 | `"continuous deployment"` + AI terms | 9 | 8 |
| ACM-06 | `"software delivery"` + AI terms | 4 | 3 |
| ACM-07 | `"AIOps"` | 63 | 63 |
|  | **Total** | **182** | **180** |

The operational ACM search log records **182 initial results**. Two proceedings/container records were removed before article screening, leaving **180 bibliographic article records**, which is also the total reproduced by the preserved ACM RIS exports.

## A.4 Identification Reconciliation

The final searchable bibliographic corpus entering deduplication was:

| Source | Records entering deduplication |
|---|---:|
| ScienceDirect | 185 |
| IEEE Xplore | 765 |
| ACM Digital Library | 180 |
| **Total** | **1,130** |

PRISMA identification reports **1,132 records identified** because it also accounts for the **two ACM proceedings/container records removed before screening**:

```text
1,132 identified
− 2 removed before screening
= 1,130 bibliographic records entering deduplication
```

The subsequent deduplication removed 317 duplicate occurrences, resulting in 813 unique records for title/abstract screening.

## A.5 Search Reproducibility Limitation

The repository preserves the database selection, search date, search fields, year restrictions, search-focus groups, result counts, and RIS exports. However, exact character-for-character platform-specific query syntax was not preserved for every executed search, particularly for ACM Digital Library. Consequently, the review reports the verifiable operational search record rather than presenting protocol-stage Boolean strings as exact executed queries.
