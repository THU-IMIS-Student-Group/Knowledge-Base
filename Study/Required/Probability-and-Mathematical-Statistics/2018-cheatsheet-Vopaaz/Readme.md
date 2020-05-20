# 概统笔记整理和 cheatsheet

- [预编译的 cheatsheet PDF](Statistics_cheat_sheet.pdf)
- [cheatsheet LaTeX 源代码](Statistics_cheat_sheet.tex)
- [展开 cheatsheet 形成的笔记总结](Statistics_ref.pdf)

预编译的 PDF 仅供预览，它包括整个学期的内容。
在期中/期末考试时请参考源代码删去范围外的部分并重新编译。
为了保证文字的紧凑，结构上作了很多 ad-hoc 的调整，内容更改后会有部分表格或公式呈现效果不好，需要重新调整。

“展开 cheatsheet 形成的笔记总结” 内容与 cheatsheet 完全相同，格式对阅读友好，适合复习，
或在结课后在其他场合需要用到概统知识时作为 reference 使用.

## 编译要求

使用 minted 宏包做 R 语言 highlighting, 需要用到 Python 的 `pygments` 宏包。

1. Prerequisite: Python 3
2. Install Pygments

```bash
$ pip install pygments
```

3. LaTeX的编译命令需要添加 "--shell-escape"
```bash
lualatex -synctex=1 -interaction=nonstopmode --shell-escape Statistics_cheat_sheet.tex
```

