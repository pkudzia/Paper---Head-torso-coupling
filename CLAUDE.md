# Paper: Head-torso coupling

Secondary video analysis of Reynier et al. 2020 head-impact footage,
quantifying head-torso coupling under passive vs. co-contracted muscle
conditions. Target journal: Annals of Biomedical Engineering (ABME).

## Folder layout

- `Annals Submission/` — frozen submitted v1 (Mar 2026). Do not edit.
- `Working Version/` — active working copy. All edits go here.
- `Data/` — raw per-participant CSVs (passive + co-contracted); private
  (chmod 700) because participants are identifiable in the source video.
  Not in git.
- `Working Version/Figures/` — `Figure 1.png` ... `Figure 6.png` (mirror
  of submitted figures until revised).
- `Working Version/papers/paper_notes.jsonl` — structured reference list.
- `Working Version/citations/ref.bib` + `verified.jsonl` — generated bib
  + verification records (see Citation workflow below).
- `Working Version/old/` — prior revision archive; never the source of truth.

## Writing rules (manuscript is .docx → passive voice)

The global rule "active for LaTeX, passive for Word" applies: this
manuscript is `.docx`, so use passive voice. Bold topic sentences. No
citations in topic sentences. Frame results honestly (no "innovations"
when "modifications" is accurate).

## Reading/editing the manuscript

The manuscript is binary `.docx`. Convert to markdown for analysis:

```bash
pandoc "Working Version/Manuscript_Submission_Final.docx" \
       -o /tmp/manuscript.md --wrap=none
```

`python-docx` is installed if you need programmatic edits.

## Citation workflow

1. Edit `papers/paper_notes.jsonl` (one JSON object per reference;
   bibkey = firstauthor+year, a/b suffix for collisions).
2. Run resolver (PubMed first, Crossref fallback; validates title overlap
   ≥ 0.60 before claiming `verified_online`). Script at
   `/tmp/resolve_citations.py` (move into repo if you re-run often).
3. Regenerated outputs: `citations/ref.bib` (BibTeX, ready to `\cite{}`)
   and `citations/verified.jsonl` (verification audit trail).

Current state: 38/39 refs verified_online. Outstanding:
- `friedman2010` — SAE Technical Paper not indexed in Crossref. Look up
  manually at sae.org; expected DOI pattern `10.4271/YYYY-XX-XXXX`.

Watch for Crossref returning "Yearbook of Sports Medicine" reprints
(DOI prefix `10.1016/s0162-0908`) instead of original journal articles —
title overlap will be 1.0 but container will be wrong. Always validate
`container-title` matches expected journal.

## Reviewer-feedback backlog (from peer review, 2026-05-18)

Items to address before resubmission/revision:
1. Add EMG %MVC quantification for passive vs. co-contracted conditions
   (currently described qualitatively in Methods).
2. Apply BH-FDR correction to Tables 2–3, OR pre-specify primary vs.
   secondary outcomes explicitly.
3. Move torso-tracking CV=56% disclosure from Discussion to Results;
   add a brief sensitivity analysis on bias direction.

## ML training note

If running pose-estimation / DeepLabCut pilots: 2 participants first for
quick validation before scaling up (matches global rule).
