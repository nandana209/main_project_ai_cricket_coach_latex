# AI Cricket Coach

LaTeX source for the project report on AI Cricket Coach — an AI-powered cricket batting analysis uses deep learning to evaluate different types of batting shots from images and provide instant feedback, helping players improve technique, reduce errors, and maintain consistent performance.

## Authors
- Abiya Mariyam Alex
- M Yadhu Krishna
- Nandana Biju
- Sania Sajan John

## Project Structure 
```text
├── main.tex              # Main document entry point
├── references.bib        # Bibliography (BibTeX)
├── compile.bat           # Build script (Windows)
├── compile.sh            # Build script (Linux/macOS)
├── Figures/              # Images, logos, and graphics
├── content/              # Source/working files
├── logs/                 # Build output directory
├── Preamble/             # Modular preamble configuration
│   ├── packages.tex      # Package imports
│   ├── fonts.tex         # Font configuration
│   ├── pagestyle.tex     # Page geometry, headers, and footers
│   ├── sectionoptions.tex# Chapter/section formatting
│   └── macro.tex         # Code listings and hyperref setup
├── Front/                # Title page, certificate, abstract, etc.
│   ├── titlepage.tex
│   ├── certificate.tex
│   ├── declaration.tex
│   ├── acknowledgements.tex
│   ├── abstract.tex
│   ├── LOA.tex
│   ├── LOS.tex
│   ├── glossary.tex
└── chapters/             # Main content chapters
    ├── chapter1.tex
    ├── chapter2.tex
    ├── chapter3.tex
    ├── chapter4.tex
    ├── chapter5.tex
    ├── chapter6.tex
    ├── chapter7.tex
    ├── chapter8.tex
    ├── chapter9.aux
    ├── chapter9.tex
    ├── Appendix.tex
```
## Building the Document

### Prerequisites
- A LaTeX distribution (e.g., TeX Live or MiKTeX)
- `xelatex` and `biber` available in your system PATH

## Compile

### Windows

```bash
xelatex -output-directory=logs -interaction=nonstopmode main.tex
biber logs/main
xelatex -output-directory=logs -interaction=nonstopmode main.tex
xelatex -output-directory=logs -interaction=nonstopmode main.tex
```

### Linux/macOS

```bash
mkdir -p logs

xelatex -output-directory=logs -interaction=nonstopmode main.tex

biber logs/main

xelatex -output-directory=logs -interaction=nonstopmode main.tex

xelatex -output-directory=logs -interaction=nonstopmode main.tex

mv -f logs/main.pdf .
```

## License
This project report is intended for academic purposes only.
