---
layout: post
author: jqt
---
# Bootstrap 代码

Bootstrap 允许您以两种方式显示代码：

- 第一种是 <code> 标签。如果您想要内联显示代码，那么您应该使用 <code> 标签。
- 第二种是 <pre> 标签。如果代码需要被显示为一个独立的块元素或者代码有多行，那么您应该使用 <pre> 标签。

请确保当您使用 <pre> 和 <code> 标签时，开始和结束标签使用了 unicode 变体： **<** 和 **>**。

让我们来看看下面的实例：

## 实例

<p><code>&lt;header&gt;</code> 作为内联元素被包围。</p> <p>如果需要把代码显示为一个独立的块元素，请使用 &lt;pre&gt; 标签：</p> <pre>     &lt;article&gt;         &lt;h1&gt;Article Heading&lt;/h1&gt;     &lt;/article&gt; </pre>


[尝试一下 »](https://www.runoob.com/try/try.php?filename=bootstrap3-code)

实例展示如下图：

![代码](https://www.runoob.com/wp-content/uploads/2014/06/code_demo.jpg)