---
layout: post
author: jqt
---
- # Bootstrap 表单

  在本章中，我们将学习如何使用 Bootstrap 创建表单。Bootstrap 通过一些简单的 HTML 标签和扩展的类即可创建出不同样式的表单。

  ## 表单布局

  Bootstrap 提供了下列类型的表单布局：

  - 垂直表单（默认）
  - 内联表单
  - 水平表单

  ### 垂直或基本表单

  基本的表单结构是 Bootstrap 自带的，个别的表单控件自动接收一些全局样式。下面列出了创建基本表单的步骤：

  - 向父 <form> 元素添加 *role="form"*。
  - 把标签和控件放在一个带有 class *.form-group* 的 <div> 中。这是获取最佳间距所必需的。
  - 向所有的文本元素 <input>、<textarea> 和 <select> 添加 class ="*form-control*" 。