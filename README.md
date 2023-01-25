# stac33-worksheets

STAC33H3: Introduction to Applied Statistics (Winter 2023) - Worksheet Sample Solutions.

## Compiling

To knit the Rnoweb file for a particular worksheet into a LaTeX file, first navigate to
the appropriate directory (e.g., `1/` for Worksheet 1). Then, use [`knitr`][1] in the R
console:
```
knitr::knit("ws1_main.Rnw")
```

To compile the LaTeX file into a PDF file using `xelatex` (as opposed to `pdflatex`), use
[`latexmk`][2] with the `-pdfxe` option (outside of the R console):
```
latexmk -pdfxe ws1_main.tex
```

[1]: https://github.com/yihui/knitr 'yihui/knitr: A general-purpose tool for dynamic report generation in R'
[2]: https://www.ctan.org/pkg/latexmk/ 'CTAN: Package latexmk'
