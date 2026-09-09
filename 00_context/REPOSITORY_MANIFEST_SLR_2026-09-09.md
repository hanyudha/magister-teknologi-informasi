# SLR Repository Manifest & Reproducibility Guide

**Updated: 9 September 2026**

## Must keep — authoritative / irreplaceable

### Context and decisions
- `README.md`
- `00_context/SLR_SESSION_HANDOFF_2026-09-09.md`
- `00_context/SLR_CONTEXT_MASTER_2026-09-09.md`
- `00_context/SLR_Milestone_AI_DevOps_2016-2026.md`
- `00_context/SLR_EVIDENCE_SYNTHESIS_LEDGER_2026-09-09.md`

### Search / screening backbone
- raw ScienceDirect export(s)
- raw IEEE Xplore export(s)
- raw ACM Digital Library export(s)
- search log: search date, query labels, filters, result counts
- deduplication master
- 382-record screening master
- `Full-Text Screening_73total.xlsx`
- final PRISMA reconciliation workbook

### Extraction / identity
- `master extraction-recovered.xlsx`
- `SLR_60_Included_Uxxxx_RECOVERED_2026-09-09.xlsx`
- `SLR_PS001-PS060_Uxxxx_FULL_EXACT_MAPPING_FINAL_2026-09-09.xlsx`

### Synthesis
- RQ1 final table/chart workbook
- RQ2 final table/chart workbook
- RQ3 taxonomy workbook
- RQ4 evidence-anchor workbook
- RQ5 challenges/gaps/future-research workbook
- scripts/notebooks used to generate charts

### PRISMA
- `SLR_PRISMA_RECONCILIATION_WORKSHEET_2026-09-09.md`
- final PRISMA reconciliation workbook
- `PRISMA_2020_AI_DevOps_AUTHORITATIVE.svg`

### References
- `SLR_Primary_Study_Reference_Ledger_EXTERNAL_VERIFICATION_COMPLETE_2026-09-09.xlsx`
- `SLR_Final_PS_to_IEEE_Mapping_7-66_2026-09-09.xlsx`
- `SLR_Final_Citation_Integrity_Audit_2026-09-09.xlsx`

### Manuscript
- latest editable manuscript DOCX
- final submission DOCX
- final PDF when generated
- supplementary/appendix files

## Strongly recommended

- Zotero export `.bib` or `.ris` for the 60 included studies
- full-text PDFs only if copyright/license and repository policy permit
- checksums for final artifacts
- `CHANGELOG.md`
- `REPRODUCE.md`
- source files for figures/tables, not only rendered images
- scripts used for deterministic transformations

## Raw-data rule

Store raw database exports under:

```text
02_search/raw/
```

Treat them as immutable. Derived files should be stored separately.

## Suggested layout

```text
magister-teknologi-informasi/
├── README.md
├── 00_context/
│   ├── SLR_SESSION_HANDOFF_2026-09-09.md
│   ├── SLR_CONTEXT_MASTER_2026-09-09.md
│   ├── SLR_Milestone_AI_DevOps_2016-2026.md
│   ├── SLR_EVIDENCE_SYNTHESIS_LEDGER_2026-09-09.md
│   └── REPOSITORY_MANIFEST_SLR_2026-09-09.md
├── 01_protocol/
├── 02_search/
│   ├── raw/
│   ├── logs/
│   └── derived/
├── 03_screening/
│   ├── dedup/
│   ├── title-abstract/
│   ├── full-text/
│   └── prism-reconciliation/
├── 04_quality/
├── 05_extraction/
├── 06_synthesis/
│   ├── rq1/
│   ├── rq2/
│   ├── rq3/
│   ├── rq4/
│   └── rq5/
├── 07_prisma/
├── 08_manuscript/
│   ├── draft/
│   ├── figures/
│   ├── tables/
│   └── final/
├── 09_references/
├── 10_supplementary/
└── 99_archive/
```

## Do not treat as source of truth

- screenshots when XLSX/source exists
- rendered bitmap when SVG/source exists
- temporary exports with unclear dates
- superseded intermediate generated files
- invalid older PRISMA image
- canonical files with `(1)`, `(2)`, `(3)` suffixes after clean copies are created

Move superseded files to `99_archive/`.

## Recovery priority

1. raw search exports
2. dedup/screening master
3. 73-study full-text log
4. extraction master
5. PS↔U mapping
6. synthesis workbooks
7. PRISMA reconciliation
8. reference ledger
9. latest manuscript
10. context/handoff files

## Current remaining work

- Appendices / Supplementary Material
- optional PDF / submission-template formatting
