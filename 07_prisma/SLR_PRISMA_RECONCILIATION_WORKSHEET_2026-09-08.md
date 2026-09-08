# SLR AI-for-DevOps --- PRISMA Final Reconciliation Worksheet

**Updated: 8 September 2026 --- FINAL RETRIEVAL ACCOUNTING**

## Status

**Reconciliation complete.** This file supersedes the earlier worksheet
where retrieval counts were marked Unknown.

The user explicitly confirmed:

> Full-text retrieval was attempted for all 382 reports via Zotero, and
> only 73 full texts were successfully obtained.

This confirmation is the audit basis for classifying the remaining 309
reports as `Not Retrieved`.

## Final PRISMA accounting

  ------------------------------------------------------------------------
  PRISMA item                                  Count Status / audit basis
  --------------------- ---------------------------- ---------------------
  Records identified                           1,132 Locked
  from databases                                     

  ScienceDirect                                  185 Locked

  IEEE Xplore                                    765 Locked

  ACM Digital Library                            180 Locked

  Other/container                                  2 Locked; exact types
  records removed                                    not established
  before screening                                   

  Bibliographic records                        1,130 Locked
  entering                                           
  deduplication                                      

  Duplicate occurrences                          317 Locked
  removed                                            

  Records screened                               813 Locked

  Records excluded at                            431 Locked
  title/abstract                                     

  Reports sought for                             382 Locked
  retrieval                                          

  Retrieval attempted                            382 User-confirmed

  Reports retrieved                               73 User-confirmed /
                                                     reconstructed
                                                     screening log

  Reports not retrieved                          309 382 attempted - 73
                                                     obtained; valid after
                                                     user confirmation

  Reports assessed for                            73 Locked
  eligibility                                        

  Full-text reports                               13 Locked
  excluded                                           

  Studies included in                             60 Locked
  review                                             

  Full-text pending                                0 Locked
  ------------------------------------------------------------------------

Arithmetic checks:

``` text
1,132 - 2 = 1,130
1,130 - 317 = 813
813 - 431 = 382
382 - 309 = 73
73 - 13 = 60
```

## Full-text exclusion reasons

  Code        Definition                                         Count
  ----------- ----------------------------------------------- --------
  FT3         No AI/ML/GenAI/AIOps intervention                      2
  FT4         MLOps only / DevOps-for-AI                             1
  FT5         Secondary or non-primary publication                   7
  FT6         Insufficient substantive evidence for the RQs          3
  **Total**                                                     **13**

FT1/FT2/FT7 are not listed in the final exclusion box because their
counts are zero in the assessed corpus.

## Reconstructed 73-study log

Source screening log: `Full-Text Screening_73total.xlsx`.

Final state: - 73 unique full-text papers - Include = 60 - Exclude =
13 - Pending = 0

The earlier pending record No. 47, Shetty et al., **"Neural Knowledge
Extraction From Cloud Service Incidents"**, was finalized as:
`Exclude — FT5`.

All 73 studies were mapped uniquely back to the 382-record baseline: -
normalized-exact title matches: 65 - fuzzy title matches: 8 - all fuzzy
mappings retained with match method/score for auditability

Known fuzzy mappings: - No 5 → U0222 --- 95 - No 7 → U0152 --- 95 - No
13 → U0584 --- 95 - No 49 → U0801 --- 96.2 - No 52 → U0069 --- 95 - No
54 → U0316 --- 89.7 - No 65 → U0041 --- 97.5 - No 72 → U0371 --- 99.6

No.47 mapped to U0718.

## Authoritative workbook

`SLR_Master_PRISMA_Reconciliation_382_2026-09-08_FINAL.xlsx`

Workbook logic: - 309 records: Retrieval Attempted=Yes; Full Text
Obtained=No; Retrieval Status=Not Retrieved; PRISMA Status=Report Not
Retrieved. - 73 records: Retrieval Attempted=Yes; Full Text
Obtained=Yes; Retrieval Status=Retrieved. - 73 assessed: 60 Include + 13
Exclude.

## Exact text for final PRISMA flow

``` text
Records identified from databases (n = 1,132)
- ScienceDirect (n = 185)
- IEEE Xplore (n = 765)
- ACM Digital Library (n = 180)

Other/container records removed before screening (n = 2)

Bibliographic records entering deduplication (n = 1,130)

Duplicate occurrences removed (n = 317)

Records screened (title/abstract) (n = 813)

Records excluded (n = 431)

Reports sought for retrieval (n = 382)

Reports not retrieved (n = 309)
- Full-text retrieval attempted via Zotero for all 382 reports; 73 obtained

Reports assessed for eligibility (n = 73)

Reports excluded (n = 13):
- FT3 — No AI/ML/GenAI/AIOps intervention (n = 2)
- FT4 — MLOps only / DevOps-for-AI (n = 1)
- FT5 — Secondary or non-primary publication (n = 7)
- FT6 — Insufficient substantive evidence for the RQs (n = 3)

Studies included in review (n = 60)
```

## Critical diagram warning

An earlier generated PRISMA image is **invalid and must not be reused**.
It contained incorrect database counts and incorrect FT-code
descriptions.

Correct database counts: - ScienceDirect 185 - IEEE Xplore 765 - ACM
Digital Library 180

Do not invent the type/reason for the two removed container records. Use
only: `Other/container records removed before screening (n=2)`.

## Exit criteria

-   [x] All 382 have retrieval state
-   [x] Retrieval attempted documented
-   [x] Reports vs studies distinguished
-   [x] Full-text exclusions have reasons
-   [x] Included corpus = 60
-   [x] Arithmetic reproducible
-   [x] Final reconciliation workbook created
-   [ ] Authoritative final PRISMA 2020 flow diagram created

## Next

Create the corrected authoritative PRISMA 2020 flow diagram from the
exact text/counts above.
