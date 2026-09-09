# Repository Lock & Git Release Checklist — 2026-09-09

## Release identity

- Branch: `main`
- Proposed release tag: `slr-ai-devops-2026-09-09`
- Release title: `AI for DevOps SLR — Visual Publication-Ready 2026-09-09`
- Evidence state: locked
- Visual publication state: QA PASS

## Authoritative publication artifacts

```text
08_manuscript/final/SLR_AI_DevOps_VISUAL_PUBLICATION_READY_FINAL_2026-09-09.docx
08_manuscript/final/SLR_AI_DevOps_VISUAL_PUBLICATION_READY_FINAL_2026-09-09.pdf
00_context/FINAL_VISUAL_QA_REPORT_2026-09-09.md
```

## Control documents synchronized

```text
README.md
REPRODUCE.md
00_context/REPOSITORY_MANIFEST_SLR_2026-09-09.md
```

## Release snapshot

```text
release/2026-09-09/
```

The release directory should contain the authoritative manuscript DOCX/PDF, QA report,
PRISMA SVG, Appendix A–E, supplementary datasets, release notes, submission README,
and SHA256 checksums.

## Files that must NOT be accidentally committed as changes

The audited working snapshot showed CRLF/LF-only churn in:

```text
02_search/raw/
02_search/logs/
99_archive/milestone/SLR_Milestone_AI_DevOps_2016-2026.md
```

`git diff --ignore-space-at-eol` showed no substantive differences for these paths.
Restore those working-tree changes before the final release commit if they are still present.

Raw RIS exports are immutable evidence and must not be normalized or rewritten.

## Recommended cleanup before staging

```bash
git restore -- \
  02_search/raw \
  02_search/logs \
  99_archive/milestone/SLR_Milestone_AI_DevOps_2016-2026.md
```

Use the command above only when `git diff --ignore-space-at-eol` is empty for those paths.

## Recommended selective staging

```bash
git add \
  .gitattributes \
  .gitignore \
  README.md \
  REPRODUCE.md \
  00_context/REPOSITORY_MANIFEST_SLR_2026-09-09.md \
  00_context/FINAL_VISUAL_QA_REPORT_2026-09-09.md \
  00_context/REPOSITORY_LOCK_AND_GIT_RELEASE_CHECKLIST_2026-09-09.md \
  01_protocol/SLR_SEARCH_STRATEGY_FINAL_2026-09-09.md \
  01_protocol/SLR_STUDY_SELECTION_PROTOCOL_FINAL_2026-09-09.md \
  01_protocol/SLR_DATA_EXTRACTION_AND_CODING_FRAMEWORK_FINAL_2026-09-09.md \
  04_quality/QA_CRITERIA_AND_SCORING_FINAL_2026-09-09.md \
  08_manuscript/final/SLR_AI_DevOps_VISUAL_PUBLICATION_READY_FINAL_2026-09-09.docx \
  08_manuscript/final/SLR_AI_DevOps_VISUAL_PUBLICATION_READY_FINAL_2026-09-09.pdf \
  10_supplementary/appendices \
  10_supplementary/datasets \
  release/2026-09-09
```

If `.gitkeep` files under populated directories appear deleted, their deletion is expected once real files exist there.

## Pre-commit validation

```bash
git status --short
git diff --check
git diff --cached --stat
git diff --cached --name-status
```

Confirm that:

- no raw RIS file appears as modified;
- no search log appears as modified unless deliberately corrected;
- no obsolete manuscript is promoted to authoritative;
- visual-final DOCX/PDF and final QA report are staged;
- release SHA256SUMS matches the frozen release directory;
- RQ1 remains 2025=8 / 2026=12;
- PS045 remains bibliographic year 2026.

## Recommended commit

```bash
git commit -m "release: lock AI-for-DevOps SLR visual publication package"
```

## Recommended annotated tag

```bash
git tag -a slr-ai-devops-2026-09-09 \
  -m "AI for DevOps SLR — visual publication-ready release, 2026-09-09"
```

## Push

```bash
git push origin main
git push origin slr-ai-devops-2026-09-09
```

## GitHub release attachment

Attach externally:

```text
SLR_AI_DevOps_VISUAL_FINAL_RELEASE_2026-09-09.zip
```

The ZIP should normally be a GitHub Release attachment rather than a committed repository binary.

## Final lock rule

Any future substantive correction must begin from the affected canonical evidence artifact,
then propagate through synthesis/context/manuscript/release. Presentation-only changes must
preserve the locked analytical state and receive an updated visual QA/release record.
