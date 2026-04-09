![seuthesis2024b](https://teddy-van-jerry.github.io/seuthesis2024b-cfp/seuthesis2024b-banner-thin.png)

LaTeX template for Southeast University bachelor's thesis, 2026 edition based on the 2025 design.

[[**Demo PDF**](https://easymoneytiger.github.io/SEU-Bachelor-Thesis/)] [[Demo TeX Source](seuthesis2026b.tex)]

> [!IMPORTANT]
> This project is under active development.
>
> 此**非官方**（unofficial）模板基于《东南大学本科毕业设计（论文）参考模板（2025版 Word 模板）》设计。具体格式要求请使用者自行核对。
>
> **2026 Edition**: This repository is a 2026 edition derived from the 2025 Word-based design, with **Teddy van Jerry**'s project used as the reference source [Repository](https://github.com/Teddy-van-Jerry/seuthesis2024b.git). See [Contributions](#contributions).

## Template Summary
This project provides a **LaTeX3** class file for Southeast University bachelor's theses: [`seuthesis2026b.cls`](seuthesis2026b.cls).
Day-to-day editing should happen in [`seuthesis2026b.tex`](seuthesis2026b.tex); you do not need to touch the LaTeX3 internals unless you are changing the template itself.

Use class options to adapt the template to your environment. On Windows, select the correct font source and remove `fontset = mac ms`.

## Usage
### Engine Supported
**XeLaTeX** only (TeX Live 2022 or later).
Compile with `latexmk -pdfxe seuthesis2026b.tex`.

### Fonts Preparation
There are two options:
1. Copy the required fonts to the `fonts` directory, or point the template to the directory that already contains them. See [`fonts/README.md`](fonts/README.md) for details. Use `font dir = {{/path/to/fonts/}}` to specify the directory, with the double brace and trailing slash preserved.
2. Use `fontset = mac ms` if you have Microsoft Word installed on macOS. On Windows, point `font dir` to `C:/Windows/Fonts/` or the equivalent local font directory.

### Recommended Entry Point
Most users only need to edit [`seuthesis2026b.tex`](seuthesis2026b.tex). It already contains:
- document metadata such as title, author, and supervisor
- bibliography resource declarations
- theorem environment setup
- abstract content and chapter imports

If you need broader adjustments, prefer class options first, then the class file defaults in [`seuthesis2026b.cls`](seuthesis2026b.cls).


## Recommended Readings
- [LaTeX v.s. Typst: What is TeX Community's Future Plan?](https://tex.stackexchange.com/q/705199/234654) (yes, my question on TeX.SX)
- [在 LaTeX 中使用 OpenType 字体（二）](https://stone-zeng.site/2019-07-06-use-opentype-fonts-ii)
- [CTeX 宏集手册](https://mirrors.ctan.org/language/chinese/ctex/ctex.pdf) (or `texdoc ctex` on your PC with local TeX installation)
- [PDF2PPT](https://github.com/Teddy-van-Jerry/pdf2ppt) (convert PDF beamer to MS PPTX presentations)
- [Wuqiong Zhao's Publications](https://wqzhao.org/publications)

## Contributions

### Original Project
This template was originally created by **Teddy van Jerry (Wuqiong Zhao)** based on the Southeast University's official MS Word template from January 2024.

### 2026 Edition Updates
- Updated the documentation to describe the template as a 2026 edition based on the 2025 Word design
- Kept the template compatible with both Windows and macOS font setups
- Preserved backward compatibility with the original thesis workflow
- Added fallback support for Chinese font filenames such as `Kaiti`/`Fangsong` and `STKAITI`/`STFANGSO`


This version keeps the original thesis workflow intact while adapting the 2025-based design for continued use in 2026.

### Additional Contributor
EasyMoneyTiger contributed changes and maintenance updates to this repository: [bachelor-thesis](https://github.com/EasyMoneyTiger/SEU-Bachelor-Thesis.git).

## License
This project is distributed by the [MIT License](LICENSE).
