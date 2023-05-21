hustreport
==========


>   中文版[点击这里](https://github.com/hust-latex/hustreport/blob/master/README.zh-cn.md)。

An Unofficial Graduate Report Template in LaTeX for [Huazhong University of Science and Technology](http://www.hust.edu.cn). See other templates in <http://hust-latex.github.io>.

## hustreport in 2023

这是一个fork版本，相比上游有如下更改。

1. 删除了填表注意事项的NotePage。
2. 删除了尾页的签字部分。
3. 删除了关于研究生的字眼。

目的是为了让本科生也能体会用LaTeX写作的乐趣（雾），因此添加了一些兼容本科生课程报告的修改。完整的旧版本请参考上游仓库。

提示：

* hustreport无法在texlive 2023下正常编译，你需要使用[texlive 2022](https://ftp.math.utah.edu/pub/tex/historic/systems/texlive/2022/)以前的版本。`autoref`功能不能正常引用。由于上游仓库已经归档，我无法继续往上游提交issue反馈。
* 你可以尝试使用[TexPage](https://www.texpage.com/)来撰写报告。
* 每一章的开头需要重设footnote的counter，否则脚注编号可能出错。
* 切换LuaLaTeX与XeLaTeX编译器时需要记得清除临时文件。

## Requirement

* Install the latest version of [TeXLive](http://www.tug.org/texlive/)(Recommend) or [MiKTeX](http://miktex.org/). Please ensure that all the packages are up-to-date.
* Install following Chinese fonts:
    * `AdobeSongStd-Light`
    * `AdobeKaitiStd-Regular`
    * `AdobeHeitiStd-Regular`
    * `AdobeFangsongStd-Regular`

## Installation

### Install into local

Use the command below to install this template into local.
```
make install
```
If you need uninstall it, use the command below.
```
make uninstall
```

For Windows User who don't install `Make`, use the command below to install.
```
makewin32.bat install
```
If you need uninstall it, use the command below.
```
makewin32.bat uninstall
```
Although `makewin32.bat` behaves much like `Makefile`, I still recommend you install `Make` into your Windows. You can download it from [here](http://gnuwin32.sourceforge.net/packages/make.htm).

### Use without installation

If you want to use this template temporary rather than installing it into local for long term use. Run below command to unpack the package.
```
make unpack
```
For Windows User who don't install `Make`, use the command below to unpack the package.
```
makewin32.bat unpack
```
Then copy following files from directory `hustreport` into your TeX project root directory:
* `hustreport.cls`
* `hust-title.eps`
* `hust-title.pdf`

## Usage

**Important : This template can only be compiled by XeLaTeX or LuaLaTeX[Recommend].**

* Manual: See [hustreport.pdf](https://github.com/hust-latex/hustreport/raw/master/hustreport/hustreport.pdf).
* Example: See [hustreport-zh-example.pdf](https://github.com/hust-latex/hustreport/raw/master/hustreport/hustreport-zh-example.pdf) and [hustreport-en-example.pdf](https://github.com/hust-latex/hustreport/raw/master/hustreport/hustreport-en-example.pdf).

## Disclaimer

This template is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.

## License

Original works are done by [Xu Cheng](https://github.com/xu-cheng). LPPL v1.3 is chosen to be the license of the project. Use as you desire.
```
Copyright (C) 2013-2014 by Xu Cheng <xucheng@me.com>
              2014-2016 by hust-latex <https://github.com/hust-latex>

This work may be distributed and/or modified under the
conditions of the LaTeX Project Public License, either version 1.3
of this license or (at your option) any later version.
The latest version of this license is in
  http://www.latex-project.org/lppl.txt
and version 1.3 or later is part of all distributions of LaTeX
version 2005/12/01 or later.

This work has the LPPL maintenance status `maintained'.

The Current Maintainer of this work is hust-latex Organization.

This work consists of the files hustreport.dtx,
hustreport.ins and the derived file hustreport.cls 
along with its document and example files.
```

