# script-template

A reusable LaTeX template for mathematical scripts.

Features:

- Multilanguage support
- Custom theorem environments
- GitHub Actions PDF build
- Ready to use as a GitHub template repository

---

## Preview

Generated PDFs are placed in:

```text
output/
├── main-de.pdf
└── main-en.pdf
```

---

## Local Build

Build manually:

```bash
latexmk -r latexmkrc main-de.tex
latexmk -r latexmkrc main-en.tex
```

or inside VS Code using the LaTeX Workshop extension (recommended):

```text
Cmd + Option + B
```

using:

```text
latexmk (latexmkrc)
```

---

## GitHub Actions

PDFs are automatically generated on:

- push to `main`
- push to `dev`
- pull requests

Workflow:

```text
.github/workflows/build.yml
```

Artifacts:

```text
output/*.pdf
```

---

## Creating New Script Repositories

This repository is intended to be used as a GitHub template.

Click:

```text
Use this template
```

Create:

```text
real-analysis-script
```

Clone locally:

```bash
git clone https://github.com/<username>/real-analysis-script.git
```

---

## License

PDF content and educational material:
CC BY-NC-ND 4.0

Source files:
Contributions via pull requests are welcome.
Modified redistribution requires permission.