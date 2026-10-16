# TrustSECO tool demonstration paper

Target: ICSE 2027 Tool Demonstration and Data Showcase.
Official call: https://conf.researchr.org/track/icse-2027/icse-2027-demonstrations

Build `main.tex` with a TeX distribution that includes IEEEtran:

```sh
latexmk -pdf main.tex
```

The manuscript uses `\documentclass[10pt,conference]{IEEEtran}` and the
IEEEtran bibliography style. The limit is four pages including references,
figures, and tables. Do not change margins, font sizes, or spacing to fit.

Author names, affiliations, email addresses, and ORCIDs have been removed from
this working manuscript while authorship is being decided. This is not a
blinded submission: tool links and scholarly references remain. The track uses
single-anonymous review, so restore the agreed author list before submission.

The old `sample.tex` and `acmart.cls` are retained as legacy template files;
`main.tex` is the manuscript to build.

Validated with Tectonic 0.17.0 after adding ICSE related work: four pages
including references; PDF author metadata is empty. The earlier IEEE manuscript
is preserved in `drafts/before-community-reframing.tex` (reference copy, not a
standalone build target). Historical images remain in `images/` but are no longer
used as screenshots of the current pilot.

See `drafts/editorial-notes.md` for evidence sources and remaining submission work.
