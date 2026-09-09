# Quality Assessment Criteria and Scoring — Final Operational Record

**Project:** Artificial Intelligence in DevOps Automation  
**Review period:** 2016–2026  
**Authoritative state:** 9 September 2026  
**Included primary studies:** 60

---

## 1. Purpose

This document records the Quality Assessment (QA) procedure supported by the preserved SLR artifacts.

The QA process was used to ensure that included primary studies met a minimum level of methodological and evidentiary adequacy before synthesis.

The preserved repository supports:

- the five QA questions;
- the scoring scheme;
- the PASS threshold;
- completion of QA for all 60 included studies;
- the final result of 60 PASS and 0 FAIL.

The repository does **not** preserve the exact numeric QA score for every individual study in the current canonical extraction workbook. The final extraction records each study as:

```text
PASS — exact score unrecovered
```

Therefore, this file does not reconstruct or invent paper-level numeric scores.

---

## 2. Quality Questions

The documented QA instrument contains five questions.

| ID | Quality Question |
|---|---|
| QA1 | Is the research objective clearly described? |
| QA2 | Are the AI application and DevOps context clearly described? |
| QA3 | Is the research/evaluation method adequately described? |
| QA4 | Are the reported results supported by evidence or data? |
| QA5 | Are limitations, threats, implications, or equivalent study constraints discussed? |

The wording above is normalized into English from the preserved project record while retaining the original meaning.

---

## 3. Scoring Scheme

Each QA question was scored as:

```text
Yes     = 1.0
Partial = 0.5
No      = 0.0
```

Maximum score:

```text
5.0
```

PASS threshold:

```text
QA Score >= 3.0 / 5
```

A study with a total score below 3.0 would fail QA.

---

## 4. Final QA Outcome

QA was completed for all 60 included primary studies.

```text
QA candidates = 60
QA assessed   = 60
QA PASS       = 60
QA FAIL       = 0
QA progress   = 100%
```

No study was removed from the final corpus because all 60 studies met the minimum threshold.

---

## 5. Relationship Between QA and Evidence Strength

A QA PASS indicates that a study met the minimum quality threshold.

It does **not** mean that all studies provide evidence of equal strength.

The extraction framework separately records:

```text
Industrial Context
Evidence Type
Evidence Strength
```

Evidence Strength categories are:

```text
Production
Industrial Empirical
Controlled Experimental
Benchmark
Simulation
Conceptual
```

This distinction is important because a conceptually well-reported study may pass QA while still providing weaker empirical evidence than a production deployment or industrial empirical evaluation.

Therefore:

> QA status should not be used as a substitute for evidence-strength classification.

---

## 6. Current Paper-Level QA Recoverability

Canonical extraction artifact:

```text
05_extraction/
SLR_Data_Extraction_60_Studies_26Fields_FINAL_2026-09-09.xlsx
```

The bibliographic sheet includes a `QA Score` column for all 60 studies.

However, the current values are recorded as:

```text
PASS — exact score unrecovered
```

This means the repository supports the following paper-level statement:

```text
Each PS001–PS060 = PASS
```

but does not support exact reconstructed values such as:

```text
PS001 = 4.0
PS002 = 4.5
...
```

unless an older QA batch artifact containing the numeric scores is recovered.

---

## 7. Provenance Note

The archived milestone records show that QA was conducted in **six batches** and reconciled so that all 60 unique included studies were assessed.

The preserved final summary is:

```text
60 assessed
60 PASS
0 FAIL
threshold >= 3.0 / 5
```

The exact batch-level score sheets are not present in the current repository snapshot.

Accordingly, the final repository should distinguish between:

- **verified final QA status** — recoverable;
- **exact historical numeric score per paper** — currently unrecovered.

---

## 8. Reproducibility Boundary

A reproducible QA reconstruction from the current repository can verify:

- QA1–QA5 definitions;
- scoring rule;
- maximum score;
- threshold;
- number of studies assessed;
- PASS/FAIL totals;
- PASS status for each of the 60 included studies.

It cannot verify:

- the exact individual QA1–QA5 decisions for each paper;
- the exact total numeric QA score of each paper;
- the original six-batch score sheets.

These values must not be recreated from interpretation of the extraction data alone.

---

## 9. Recommended Repository Treatment

This file should be stored as:

```text
04_quality/
QA_CRITERIA_AND_SCORING_FINAL_2026-09-09.md
```

The current `.gitkeep` may be removed after this file is added.

Do not create a fabricated numeric QA workbook merely to populate `04_quality/`.

If historical batch-level QA files are recovered later, preserve them under a source/recovery location and perform a controlled reconciliation before updating the canonical QA record.

---

## 10. Integrity Checks

The QA layer is internally consistent when:

```text
Included studies = 60
QA assessed      = 60
QA PASS          = 60
QA FAIL          = 0
```

and:

```text
PASS threshold = >= 3.0 / 5
```

The final corpus therefore remains:

```text
60 primary studies
```

after QA.

---

## 11. Status

**Quality Assessment operational record: FINAL for the currently preserved evidence.**

Exact paper-level numeric QA scores remain unrecovered and must not be invented.
