---
layout: post
author: jqt

---
# Bootstrap 面包屑导航（Breadcrumbs）

面包屑导航（Breadcrumbs）是一种基于网站层次信息的显示方式。以博客为例，面包屑导航可以显示发布日期、类别或标签。它们表示当前页面在导航层次结构内的位置。

Bootstrap 中的面包屑导航（Breadcrumbs）是一个简单的带有 **.breadcrumb** class 的无序列表。分隔符会通过 CSS（bootstrap.min.css）中下面所示的 class 自动被添加：

```
.breadcrumb > li + li:before {
    color: #CCCCCC;
    content: "/ ";
    padding: 0 5px;
}
```

下面的实例演示了面包屑导航：

## 实例

<ul class="breadcrumb">    <li><a href="#">Home</a></li>    <li><a href="#">2013</a></li>    <li class="active">十一月</li> </ul>