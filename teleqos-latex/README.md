# TeleQoS IEEE LaTeX Project

Editable IEEE conference-paper source converted from `IEEE Conference Paper - TeleQoS.pdf`.

## Files

- `main.tex`: paper source, IEEE conference layout, and compile-safe figure placeholders.
- `references.bib`: the nine references listed in the source paper.

The original PDF refers to five figures, but the figures were not provided as separate image files. Replace the boxed placeholders in `main.tex` with the original images before submitting a final paper. Check the citation metadata and complete any missing publication details against the sources you used.

## Build

Install a LaTeX distribution that includes the IEEEtran class, BibTeX, and the `cite`, `graphicx`, `amsmath`, and `url` packages. From this directory, run:

```text
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

Alternatively, with `latexmk`:

```text
latexmk -pdf main.tex
```

The resulting file is `main.pdf`. The source machine did not have a LaTeX compiler available, so a compiled PDF is not included yet.