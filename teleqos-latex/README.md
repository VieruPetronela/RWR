# TeleQoS IEEE LaTeX Project

Editable IEEE conference-paper source converted from `IEEE Conference Paper - TeleQoS.pdf`.

## Files

- `main.tex`: paper source, IEEE conference layout, and compile-safe figure placeholders.
- `references.bib`: the nine references listed in the source paper.

The compiled `main.pdf` is included. The original paper refers to five figures, but the image files were not provided separately; `main.tex` uses boxed placeholders for them. Replace those placeholders with the original images before submitting a final paper. Check the citation metadata and complete any missing publication details against the sources you used.

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

The build produces `main.pdf`. The included PDF was built with MiKTeX using the commands above.