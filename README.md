# cv-renyi

Bilingual CV (English / French) for Ren Yi, built with LaTeX.

## Structure

```
cv-renyi-en/   # English version
cv-renyi-fr/   # French version
```

Each folder contains:
- `main.tex` — entry point
- `preamble.tex` — layout and styling
- `sections/` — individual content sections

## Build

Compile with `pdflatex` or `latexmk`:

```bash
cd cv-renyi-en
latexmk -pdf main.tex
```
