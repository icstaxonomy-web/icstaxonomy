# IC3SA / ARES SecIndustry 2026 submission package

LNCS-formatted workshop paper for **ARES 2026 / 5th Workshop on Cybersecurity
in Industry 4.0 and Beyond (SecIndustry)**. Page limit: 18 pages including
references; double-blind. Current PDF: **18 pages**.

## Contents

| File | Purpose |
|---|---|
| `mainsecind.tex` | LaTeX source (LNCS class, `llncs.cls`) |
| `mybib.bib` | 34 BibTeX entries (style: `splncs04`) |
| `mainsecind.pdf` | Compiled paper (for sanity-check) |
| `figures/` | Two figures actually referenced (`conceptpm.png`, `methodo.png`) |
| `IC3SA_Taxonomy_Construction_Methodology__5_.xlsx` | Supplementary workbook (Stages 1–5, 12 sheets), cited in the paper as `\cite{ic3sa_workbook}` |

## Build instructions

Requires `texlive-publishers` (for `llncs.cls`) and `texlive-latex-extra`.

```bash
pdflatex mainsecind
bibtex   mainsecind
pdflatex mainsecind
pdflatex mainsecind
```

## Anonymity notes (for submission)

- Title block uses `\author{Anonymous Authors}`; real author block is
  commented out in the source.
- Acknowledgments are masked ("omitted for double-blind review").
- The supplementary workbook (`ic3sa_workbook`) and the web navigator
  (`icstaxonomy`) are both hosted under anonymized identities — the URLs
  in `mybib.bib` point to the anonymous accounts you set up.
- The author block, full acknowledgments, and any non-anonymous URLs
  should be restored at camera-ready.

## Known minor items

- The InCReASE and Bitton bibliography entries list co-author surnames in
  their metadata. The body wording is third-person and does not flag the
  references as self-citations; you've accepted this risk per discussion.
- Four `Overfull \hbox` warnings of 15–27pt remain in long paragraphs;
  cosmetic, no visible margin overflow.
