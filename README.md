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

Compile with `latexmk` using **LuaLaTeX** (needed to render the Chinese name 任一
with the TeX Live–bundled FandolSong font):

```bash
cd cv-renyi-en
latexmk -lualatex main.tex
```

> A `pdflatex` build still compiles, but shows the name romanized ("Ren Yi")
> only — the Chinese characters appear under LuaLaTeX. (The French CV is still
> built with `pdflatex`.)
