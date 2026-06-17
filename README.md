# Smart Transaction Sorter and Analytics System — Thesis Documentation

This repository contains the official LaTeX thesis documentation for the **Smart Transaction Sorter and Analytics System**, developed as a Final Year Project (FYP).

## 📁 Repository Structure

*   `chapters/` — Individual LaTeX files for each chapter (01 to 06):
    *   `01_introduction.tex` — Project Introduction & Related Applications Survey.
    *   `02_requirements.tex` — Software Requirements Specification (SRS) & Ingestion Scenarios.
    *   `03_usecase.tex` — Use Case Specifications & Component Lifecycles.
    *   `04_construction.tex` — System Implementation details, Environment Versions, & AI Safety borders.
    *   `05_testing.tex` — Quality Assurance, Performance Latencies, & Test Case matrices.
    *   `06_user_guide.tex` — Visual End-User manual including NayaPay and multi-file instructions.
*   `images/` — Screenshots and static system diagrams referenced in the text.
*   `diagram_sources/` — Editable `.drawio` source files for the sequence and system diagrams.
*   `main.tex` — The primary entrypoint file for compiling the LaTeX document.
*   `references.bib` — The BibTeX database containing all referenced academic papers and market studies.
*   `cover.pdf` — The official thesis cover page PDF (included at the start of compilation).
*   `approval.pdf` — The official project approval certificate PDF (included at the start of compilation).
*   `titlepage.tex` — The LaTeX source template for the Federal Urdu University title page border.

## 🛠️ How to Compile the Document

To compile the LaTeX source into a unified PDF, use any standard LaTeX distribution (such as MiKTeX or TeX Live) with **XeLaTeX** and **BibTeX**.

Run the following commands in sequence to build the document and resolve all citations:

```bash
# 1. First XeLaTeX compile to build auxiliary indexes
xelatex main.tex

# 2. Run BibTeX to resolve citations from references.bib
bibtex main

# 3. Compile again to link references in the text
xelatex main.tex

# 4. Final compile to generate the correct Table of Contents and PDF bookmarks
xelatex main.tex
```

The compiled output will be generated as `main.pdf` in the root folder.
