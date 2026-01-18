# Halmos: Naive Set Theory (Quarto Edition)

[![Quarto Publish](https://github.com/luifrancgom/halmos_naive_set_theory_quarto/actions/workflows/publish.yml/badge.svg)](https://github.com/luifrancgom/halmos_naive_set_theory_quarto/actions/workflows/publish.yml)
[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

This repository contains a modern re-edition of Paul R. Halmos's classic **Naive Set Theory**, authored using [Quarto](https://quarto.org/). 

The project is based on the LaTeX source and OCR work by [Matheus Girola Macedo Barbosa](https://github.com/matheusgirola/Halmos-Naive-Set-Theory-OCR-LaTeX-Reedition). 

The original text is currently in the public domain and can be accessed via the [Hathi Trust Digital Library](https://babel.hathitrust.org).

---

## 📖 Read Online

You can access the rendered versions of the book through the following links:

| Format | Link |
| :--- | :--- |
| **🌐 HTML** | [View Web Version](https://luifrancgom.github.io/halmos_naive_set_theory_quarto/) |
| **📄 PDF** | [Download PDF](https://luifrancgom.github.io/halmos_naive_set_theory_quarto/Naive-Set-Theory.pdf) |
| **📑 DOCX** | [Download DOCX](https://luifrancgom.github.io/halmos_naive_set_theory_quarto/Naive-Set-Theory.docx) |

---

## 🛠 Build from Source

To generate the book locally, ensure you have [Git](https://git-scm.com/) and [Quarto](https://quarto.org/docs/download/) installed on your system.

### Clone the Repository

Open your terminal and run the following commands to download the code and enter the project folder:

```bash
git clone https://github.com/luifrancgom/halmos_naive_set_theory_quarto.git
cd halmos_naive_set_theory_quarto
```

### Install Dependencies

To render the PDF version, you need a LaTeX distribution. If you do not have one installed, Quarto can set up a lightweight version (TinyTeX) for you:

```bash
quarto install tinytex
```
### Render the Book

Once the dependencies are ready, you can render all formats (HTML and PDF) with a single command:

```bash
quarto render
```

### Accessing Intermediate Files

By default, Quarto cleans up intermediate files after rendering. If you want to inspect the generated `.tex` (LaTeX) or `.md` (Markdown) source files, you must modify the `_quarto.yml` configuration file. 

Uncomment (or add) the following options under the pdf format section:

```yaml
format:
  pdf:
    keep-md: true
    keep-tex: true
```
After saving the changes to `_quarto.yml`, run `quarto render` again. The files will then remain in your project directory for you to access.

## ⚖️ License and Attribution

This project is licensed under the [CC BY-NC-SA 4.0](LICENSE.md).

### Credits

* **Original Text:** *Naive Set Theory* (1960) by **Paul Halmos**. The original content is in the **Public Domain** and can be accessed via the [HathiTrust Digital Library](https://babel.hathitrust.org/cgi/pt?id=mdp.39015002409556).
* **LaTeX Source & OCR:** This edition is based on the LaTeX conversion and OCR work by [Matheus Girola Macedo Barbosa](https://github.com/matheusgirola/Halmos-Naive-Set-Theory-OCR-LaTeX-Reedition). Used with permission.
* **Quarto Conversion:** Modernized and converted to Quarto by [Luis Francisco Gomez Lopez](https://github.com/luifrancgom/halmos_naive_set_theory_quarto).
* **Cover Image:** Corresponds to a fragment of [The Garden of Earthly Delights](https://en.wikipedia.org/wiki/The_Garden_of_Earthly_Delights) by Hieronymus Bosch (circa 1450–1516), which is a **Public Domain** work.
