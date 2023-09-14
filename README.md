# Tufte LaTeX包使用指南

欢迎使用Tufte LaTeX包，它可以帮助你制作符合Tufte风格的讲义、报告和笔记。

## 快速入门

尝试使用以下命令对`sample-handout.tex`进行排版：

```shell
pdflatex sample-handout
bibtex   sample-handout
pdflatex sample-handout
pdflatex sample-handout
```

结果应该看起来像`sample-handout.pdf`。

要编译示例书籍，请使用以下命令：

```
pdflatex sample-book
bibtex sample-book
texindy --language english sample-book.idx
# 或者使用 makeindex sample-book.idx
pdflatex sample-book
pdflatex sample-book
pdflatex sample-book
```

## 故障排除

如果你遇到以下形式的错误：

```latex
! LaTeX Error: File `paralist.sty' not found.
```

你需要从 [CTAN](http://ctan.org) 获取缺少的包。有关包的安装说明以及许多其他问题的答案，请参阅 [UK TeX FAQ](http://www.tex.ac.uk/faq/) 或搜索 [`comp.text.tex` 群组](http://groups.google.com/group/comp.text.tex)。


## 以下包是必需的：

(我在每个宏包名称后面简要说明一下它们的主要作用)


- `chngpage` 或 `changepage`：用于调整页面布局。
- `fancyhdr`：用于自定义页眉和页脚。
- `fontenc`：用于控制字体编码和输出字符。
- `geometry`：用于设置页面尺寸和边距。
- `hyperref`：用于创建超链接和 PDF 书签。
- `natbib` 和 `bibentry`：用于处理参考文献和引用。
- `optparams`：用于设置参数选项。
- `paralist`：用于自定义列表格式。
- `placeins`：用于控制浮动对象（如图表）的位置。
- `ragged2e`：用于调整文本对齐方式。
- `setspace`：用于设置行距。
- `textcase`：用于控制文本的大小写。
- `textcomp`：提供额外的文本符号。
- `titlesec`：用于自定义章节标题格式。
- `titletoc`：用于自定义目录的格式。
- `xcolor`：用于控制颜色。
- `xifthen`：提供条件语句。

希望这些简要说明有助于你理解每个宏包的用途。如果你需要更详细的信息，可以查阅相应宏包的文档或手册。

## 以下包是可选的，如果安装了将会自动使用：

- `beramono`：提供一种等宽字体（Mono字体）。
- `helvet`：使用Helvetica字体。
- `ifpdf`：用于检测文档是否正在生成为PDF。
- `ifxetex`：用于检测文档是否在XeTeX引擎下编译。
- `letterspace`（在microtype宏包中）：用于微调字符之间的间距，以改善排版。
- `mathpazo`：使用Palatino字体作为数学字体。
- `soul`：提供各种文本修饰功能，如高亮、下划线等。

这些可选宏包可以根据你的需求选择性地安装和使用，以满足特定的排版要求。希望这些简要说明有助于你理解它们的作用。如有需要，你可以查阅相应宏包的文档以获取更详细的信息。

# 错误/功能/支持

如果你有赞誉、功能请求、补丁或与此Tufte-LaTeX包特定相关的支持请求，即不是一般的LaTeX问题，请使用此项目的问题跟踪器，网址为 [Tufte-LaTeX](https://github.com/Tufte-LaTeX/tufte-latex/issues)。

# 贡献

通过问题跟踪器提交补丁和拉取请求非常欢迎！提交一系列高质量的补丁，你将成为这个项目的开发人员之一。

# 许可证

由Kevin Godby、Bil Kleb和Bill Wood于2007年至2015年编写。

根据Apache许可证第2.0版（"许可证"）许可，除非符合许可证要求，否则不能使用此文件。你可以在以下网址获取许可证的副本：

http://www.apache.org/licenses/LICENSE-2.0

除非适用法律要求或书面同意，否则按照"原样"分发的软件不附带任何明示或暗示的担保或条件。请查看许可证以获取特定语言的详细信息以及许可证下的限制。
