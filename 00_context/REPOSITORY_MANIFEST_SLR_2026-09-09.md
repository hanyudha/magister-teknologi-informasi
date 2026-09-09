# SLR Repository Manifest & Reproducibility Inventory

**Updated: 9 September 2026**  
**State:** Analytical artifacts, Appendix A–E, Supplementary Dataset Master, and visual publication-ready artifacts synchronized

## 1. Authoritative context

Must keep:

```text
README.md
REPRODUCE.md
00_context/SLR_CONTEXT_MASTER_2026-09-09.md
00_context/SLR_SESSION_HANDOFF_2026-09-09.md
00_context/SLR_EVIDENCE_SYNTHESIS_LEDGER_2026-09-09.md
00_context/REPOSITORY_MANIFEST_SLR_2026-09-09.md
00_context/FINAL_VISUAL_QA_REPORT_2026-09-09.md
```

Historical milestones belong under `99_archive/` and are not current source of truth.

## 2. Protocol and methodological records

```text
01_protocol/SLR_SEARCH_STRATEGY_FINAL_2026-09-09.md
01_protocol/SLR_STUDY_SELECTION_PROTOCOL_FINAL_2026-09-09.md
01_protocol/SLR_DATA_EXTRACTION_AND_CODING_FRAMEWORK_FINAL_2026-09-09.md
04_quality/QA_CRITERIA_AND_SCORING_FINAL_2026-09-09.md
```

These files preserve the operationally supportable protocol state. They deliberately distinguish documented draft criteria from final observed operational outcomes where provenance requires it.

## 3. Raw search evidence — immutable

```text
02_search/raw/sciencedirect/
02_search/raw/ieee/
02_search/raw/acm/
02_search/logs/
```

Final database contribution entering deduplication:

```text
ScienceDirect = 185
IEEE Xplore   = 765
ACM DL        = 180
Total         = 1,130
```

Two ACM proceedings/container records are retained in PRISMA identification accounting as removed before screening, producing 1,132 identified records.

## 4. Screening backbone

```text
03_screening/dedup/SLR_Master_Deduplication_2026-09-07.xlsx
03_screening/title-abstract/SLR_Master_Maybe_Resolved_813_2026-09-08.xlsx
03_screening/full-text/SLR_Master_FullText_Screening_Ready_382_2026-09-08.xlsx
03_screening/full-text/Full-Text Screening_73total.xlsx
03_screening/full-text/SLR_60_Included_Uxxxx_RECOVERED_2026-09-09.xlsx
03_screening/prism-reconciliation/SLR_Master_PRISMA_Reconciliation_382_2026-09-08_FINAL.xlsx
```

Locked chain:

```text
1,130 → 813 → 382 → 73 → 60
```

## 5. Quality Assessment

```text
04_quality/QA_CRITERIA_AND_SCORING_FINAL_2026-09-09.md
```

Final QA state:

```text
60 assessed
60 PASS
0 FAIL
threshold >= 3.0 / 5
```

Exact historical numeric scores per paper are unrecovered. Do not fabricate them.

## 6. Extraction and identity

```text
05_extraction/SLR_Data_Extraction_60_Studies_26Fields_FINAL_2026-09-09.xlsx
05_extraction/SLR_PS001-PS060_Uxxxx_FULL_EXACT_MAPPING_FINAL_2026-09-09.xlsx
```

Canonical extraction:

```text
60 studies
26 fields
PS001–PS060 ↔ Uxxxx = 60/60 one-to-one
```

Known identity safeguards:

```text
PS009 → U0669
PS047 → U0459
PS045 → U0041, year 2026
```

## 7. RQ synthesis

```text
06_synthesis/rq1/RQ1_Final_Publication_Trend_AI_DevOps_2016-2026.xlsx
06_synthesis/rq2/RQ2_Final_DevOps_Stages_and_Application_Areas_AI_DevOps_2016-2026.xlsx
06_synthesis/rq3/RQ3_Final_AI_Taxonomy_and_Methods_DevOps_2016-2026.xlsx
06_synthesis/rq4/RQ4_Final_Benefits_Impacts_Evidence_Anchors_AI_DevOps_2016-2026.xlsx
06_synthesis/rq5/RQ5_Final_Challenges_Gaps_Future_Research_AI_DevOps_2016-2026.xlsx
```

Locked safeguards:

- RQ1: 2025=8, 2026=12.
- RQ2: multi-label; counts need not sum to 60.
- RQ3: final primary taxonomy sums to 60.
- RQ4: no unsupported corpus-wide B1–B7 prevalence.
- RQ5: G1–G8 and FR1–FR5 are synthesis constructs derived from study evidence.

## 8. PRISMA

```text
07_prisma/PRISMA-2020-F_AI_DevOps_AUTHORITATIVE.svg
07_prisma/SLR_PRISMA_RECONCILIATION_WORKSHEET_2026-09-09.md
03_screening/prism-reconciliation/SLR_Master_PRISMA_Reconciliation_382_2026-09-08_FINAL.xlsx
```

Locked PRISMA:

```text
Identified = 1,132
Entering deduplication = 1,130
Duplicate occurrences removed = 317
Screened = 813
Title/abstract excluded = 431
Reports sought = 382
Not retrieved = 309
Assessed = 73
Full-text excluded = 13
Included = 60
```

## 9. Manuscript and publication rendering

### Authoritative publication artifacts

```text
08_manuscript/final/SLR_AI_DevOps_VISUAL_PUBLICATION_READY_FINAL_2026-09-09.docx
08_manuscript/final/SLR_AI_DevOps_VISUAL_PUBLICATION_READY_FINAL_2026-09-09.pdf
```

Current authority:

```text
Authoritative editable manuscript:
SLR_AI_DevOps_VISUAL_PUBLICATION_READY_FINAL_2026-09-09.docx

Authoritative publication rendering:
SLR_AI_DevOps_VISUAL_PUBLICATION_READY_FINAL_2026-09-09.pdf

Final visual QA record:
00_context/FINAL_VISUAL_QA_REPORT_2026-09-09.md
```

The visual-publication pass is presentation-only and does not alter the locked analytical SLR state.

### Pre-visual / provenance artifacts

```text
08_manuscript/final/SLR_AI_DevOps_Consolidated_FINAL_CITATIONS_2026-09-09.docx
08_manuscript/final/SLR_AI_DevOps_PUBLICATION_READY_FINAL_2026-09-09.docx
```

`SLR_AI_DevOps_PUBLICATION_READY_FINAL_2026-09-09.docx` is retained as the **pre-visual publication baseline / rollback artifact** and must not override the authoritative visual publication-ready DOCX/PDF.


## 10. References and bibliographic verification

```text
09_references/SLR_Primary_Study_Reference_Ledger_EXTERNAL_VERIFICATION_COMPLETE_2026-09-09.xlsx
09_references/SLR_Final_PS_to_IEEE_Mapping_7-66_2026-09-09.xlsx
09_references/SLR_Final_Citation_Integrity_Audit_2026-09-09.xlsx
```

Locked state:

```text
DOI coverage = 60/60
External verification = 60/60
Background refs = [1]–[6]
Primary refs = [7]–[66]
Citation integrity = PASS
```

## 11. Appendices

```text
10_supplementary/appendices/APPENDIX_A_SEARCH_STRATEGY_2026-09-09.md
10_supplementary/appendices/APPENDIX_B_STUDY_SELECTION_PROTOCOL_2026-09-09.md
10_supplementary/appendices/APPENDIX_C_QUALITY_ASSESSMENT_2026-09-09.md
10_supplementary/appendices/APPENDIX_D_INCLUDED_PRIMARY_STUDIES_2026-09-09.md
10_supplementary/appendices/APPENDIX_E_DATA_EXTRACTION_AND_CODING_FRAMEWORK_2026-09-09.md
```

Status: **Appendix A–E complete**.

## 12. Supplementary datasets

```text
10_supplementary/datasets/SLR_INCLUDED_PRIMARY_STUDIES_60_FINAL_2026-09-09.xlsx
10_supplementary/datasets/SLR_SUPPLEMENTARY_DATASET_MASTER_2026-09-09.xlsx
```

The master workbook provides audit views for:

```text
00_README
01_Primary_Studies
02_QA
03_Extraction_26F
04_PS_U_Mapping
05_RQ1
06_RQ2
07_RQ3
08_RQ4
09_RQ5
10_PRISMA
```

It is a consolidated audit package and does not replace raw or stage-specific source files.

## 13. Release snapshot

Recommended release location:

```text
release/2026-09-09/
├── manuscript/
│   ├── SLR_AI_DevOps_VISUAL_PUBLICATION_READY_FINAL_2026-09-09.docx
│   └── SLR_AI_DevOps_VISUAL_PUBLICATION_READY_FINAL_2026-09-09.pdf
├── qa/
│   └── FINAL_VISUAL_QA_REPORT_2026-09-09.md
├── supplementary/
├── figures/
├── SUBMISSION_README.md
└── SHA256SUMS.txt
```

The release directory is an immutable submission/share snapshot. It does not replace the authoritative source artifacts under `08_manuscript/final/`, `00_context/`, `07_prisma/`, or `10_supplementary/`.

## 14. Archive

```text
99_archive/milestone/SLR_Milestone_AI_DevOps_2016-2026.md
```

Archive files are historical only. They may contain obsolete intermediate values and must not override current context.

## 15. Source-of-truth priority

For conflicts, use this priority:

1. current externally verified / final record-level workbook for the affected analytical layer;
2. `SLR_CONTEXT_MASTER_2026-09-09.md`;
3. final synthesis / PRISMA artifact;
4. authoritative visual publication-ready DOCX/PDF for the current manuscript/rendering state;
5. final visual QA report for presentation/rendering verification;
6. supplementary consolidation;
7. pre-visual manuscript baselines;
8. historical/recovered/archived artifacts.

The supplementary master is convenient for audit, but provenance-sensitive corrections should be made first in the relevant canonical source artifact. Visual/layout corrections must not override analytical source-of-truth artifacts.

## 16. Raw-data and copyright rule

- Raw database exports under `02_search/raw/` are immutable.
- Do not overwrite raw/recovered files to make them look final; create a validated final artifact.
- Full-text publisher PDFs should not be committed to a public repository unless redistribution is permitted.
- Prefer DOI/RIS/BibTeX/reference ledgers for public reproducibility.

## 17. Recovery priority

1. `README.md` + `REPRODUCE.md`
2. context master + session handoff
3. raw search exports and logs
4. dedup / screening workbooks
5. PRISMA reconciliation
6. final extraction + PS↔U mapping
7. RQ1–RQ5 synthesis
8. reference ledgers
9. supplementary master
10. authoritative visual publication-ready DOCX
11. authoritative visual publication-ready PDF
12. final visual QA report
13. pre-visual publication baseline only if rollback/provenance is required

## 18. Remaining work

No additional analytical appendix or substantive SLR revision is required for the current evidence state.

Remaining work is release/submission administration only:

- synchronize the final release snapshot under `release/2026-09-09/`;
- include the authoritative visual DOCX/PDF and final visual QA report;
- refresh `SUBMISSION_README.md` if the release package is maintained;
- regenerate `SHA256SUMS.txt` after the release contents are frozen;
- optionally create a Git tag/release;
- apply university/journal template-specific formatting only if required by the target venue;
- prepare submission-specific files if required.

Any future analytical change must be treated as a controlled correction and propagated through the affected evidence, synthesis, context, manuscript, and release artifacts.
