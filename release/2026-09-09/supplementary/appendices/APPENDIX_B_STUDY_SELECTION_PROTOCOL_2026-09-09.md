# Appendix B — Study Selection Protocol

Study selection followed a staged process consisting of deduplication, title/abstract screening, full-text retrieval, eligibility assessment, and quality assessment. The review boundary was **AI-for-DevOps**: studies were eligible when AI, ML, deep learning, Generative AI, LLMs, AIOps, or related techniques were used to improve, support, analyze, optimize, or automate a DevOps activity. Studies focused only on MLOps or DevOps-for-AI were excluded unless AI itself was used to improve DevOps.

The protocol-development archive documented the following inclusion criteria: publication during 2016–2026; explicit DevOps or CI/CD relevance; application of AI/ML/GenAI/LLM to DevOps; peer-reviewed journal or conference publication; English language; accessible full text; and evidence relevant to at least one research question. The corresponding draft exclusion framework covered duplicate records, non-DevOps studies, AI without DevOps application, MLOps-only / DevOps-for-AI studies, non-primary or non-peer-reviewed material, unavailable full text, non-English publications, and secondary studies.

Because the surviving protocol source labels these IC/EC tables as **draft**, this appendix does not claim that the wording represents a separately preserved pre-registered final protocol. Instead, it reports both the documented criteria and the final operational selection outcomes.

## B.1 Selection Flow

```text
1,132 records identified
        ↓
2 records removed before screening
        ↓
1,130 records entering deduplication
        ↓
317 duplicate occurrences removed
        ↓
813 unique records screened
        ↓
431 title/abstract records excluded
        ↓
382 reports sought for retrieval
        ↓
309 reports not retrieved
        ↓
73 reports retrieved / assessed
        ↓
13 full-text reports excluded
        ↓
60 primary studies included
        ↓
Quality assessment: 60/60 PASS
```

The numerical reconciliation is:

```text
1,130 - 317 = 813
813 - 431 = 382
382 - 309 = 73
73 - 13 = 60
```

## B.2 Title and Abstract Screening

After deduplication, **813 unique records** underwent title/abstract screening. A total of **431 records** were excluded, leaving **382 reports** for full-text retrieval.

The main operational relevance boundary was whether the study addressed AI applied to a DevOps activity. Records clearly focused on unrelated Software Engineering topics or DevOps-for-AI without AI-for-DevOps contribution were not retained.

## B.3 Retrieval

Retrieval was attempted for all **382 reports**. Full texts were obtained for **73 reports**, while **309 reports were not retrieved**.

The 309 unavailable reports were reported in PRISMA as **reports not retrieved**, not as full-text eligibility exclusions.

## B.4 Full-Text Eligibility Assessment

The **73 retrieved reports** underwent full-text eligibility assessment. **60 studies were included** and **13 were excluded**.

| Code | Full-text exclusion reason | Count |
|---|---|---:|
| FT3 | No AI/ML/GenAI/AIOps intervention | 2 |
| FT4 | MLOps only / DevOps-for-AI | 1 |
| FT5 | Secondary or non-primary publication | 7 |
| FT6 | Insufficient substantive evidence for the RQs | 3 |
|  | **Total** | **13** |

Only FT3–FT6 are reported because these are the exclusion categories observed in the final locked full-text dataset.

## B.5 Quality Assessment

All **60 included primary studies** underwent quality assessment using five questions covering clarity of objectives, AI-and-DevOps relevance, adequacy of method/evaluation, evidence support for findings, and discussion of limitations or implications.

Scoring used:

```text
Yes     = 1.0
Partial = 0.5
No      = 0.0
PASS    = score >= 3.0 / 5
```

All **60 studies passed**. Quality Assessment therefore did not reduce the final study count. A PASS result was treated as a minimum quality threshold and not as evidence that all studies had equal methodological or empirical strength.

## B.6 Final Included Corpus

The final corpus consists of **60 primary studies**, each assigned a `PS001–PS060` manuscript identifier and mapped one-to-one to the corresponding `Uxxxx` screening identifier. This mapping provides traceability from the final manuscript back to the screening workflow.
