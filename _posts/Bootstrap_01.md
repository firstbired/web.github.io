---
layout: post
author: jqt
---
# Bootstrap 环境安装

Bootstrap 安装是非常容易的。本章将讲解如何下载并安装 Bootstrap，讨论 Bootstrap 文件结构，并通过一个实例演示它的用法。

## 下载 Bootstrap

您可以从 http://getbootstrap.com/ 上下载 Bootstrap 的最新版本。当您点击这个链接时，您将看到如下所示的网页：

![Bootstrap 下载](https://www.runoob.com/wp-content/uploads/2014/06/bootstrapdowloadscreen.jpg)

您会看到两个按钮：

- *Download Bootstrap*：下载 Bootstrap。点击该按钮，您可以下载 Bootstrap CSS、JavaScript 和字体的预编译的压缩版本。不包含文档和最初的源代码文件。
- *Download Source*：下载源代码。点击该按钮，您可以直接从 from 上得到最新的 Bootstrap LESS 和 JavaScript 源代码。

如果您使用的是未编译的源代码，您需要编译 LESS 文件来生成可重用的 CSS 文件。对于编译 LESS 文件，Bootstrap 官方只支持 [Recess](http://twitter.github.io/recess/)，这是 Twitter 的基于 [less.js](http://lesscss.org/) 的 CSS 提示。

为了更好的了解和更方便的使用，我们将在本教程中使用 Bootstrap 的预编译版本。

由于文件是被编译过和压缩过的，在独立的功能开发中，您不必每次都包含这些独立的文件。

本教程编写时，使用的是最新版（Bootstrap 3）。

## 文件结构

### 预编译的 Bootstrap

当您下载了 Bootstrap 的已编译的版本，解压缩 ZIP 文件，您将看到下面的文件/目录结构：

![已编译的 Bootstrap 文件结构](https://www.runoob.com/wp-content/uploads/2014/06/compiledfilestructure.jpg)

如上图所示，可以看到已编译的 CSS 和 JS（bootstrap.*），以及已编译压缩的 CSS 和 JS（bootstrap.min.*）。同时也包含了 Glyphicons 的字体，这是一个可选的 Bootstrap 主题。

### Bootstrap 源代码

如果您下载了 Bootstrap 源代码，那么文件结构将如下所示：

![Bootstrap 源代码结构](https://www.runoob.com/wp-content/uploads/2014/06/sourcecodefilestructure.jpg)

- *less/*、*js/* 和 *fonts/* 下的文件分别是 Bootstrap CSS、JS 和图标字体的源代码。
- *dist/* 文件夹包含了上面预编译下载部分中所列的文件和文件夹。
- *docs-assets/*、*examples/* 和所有的 **.html* 文件是 Bootstrap 文档。