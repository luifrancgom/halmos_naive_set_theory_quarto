# Halmos: Naive Set Theory (Quarto Edition)

[![Quarto Publish](https://github.com/luifrancgom/halmos_naive_set_theory_quarto/actions/workflows/publish.yml/badge.svg)](https://github.com/luifrancgom/halmos_naive_set_theory_quarto/actions/workflows/publish.yml)

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
