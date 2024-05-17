---
layout: post
author: jqt

---
# Bootstrap 下拉菜单（Dropdowns）

本章将重点介绍 Bootstrap 下拉菜单。下拉菜单是可切换的，是以列表格式显示链接的上下文菜单。这可以通过与 [下拉菜单（Dropdown） JavaScript 插件](https://www.runoob.com/bootstrap/bootstrap-dropdown-plugin.html) 的互动来实现。

如需使用下拉菜单，只需要在 class **.dropdown** 内加上下拉菜单即可。下面的实例演示了基本的下拉菜单：

## 实例

<div class="dropdown">     <button type="button" class="btn dropdown-toggle" id="dropdownMenu1" data-toggle="dropdown">主题         <span class="caret"></span>     </button>     <ul class="dropdown-menu" role="menu" aria-labelledby="dropdownMenu1">         <li role="presentation">             <a role="menuitem" tabindex="-1" href="#">Java</a>         </li>         <li role="presentation">             <a role="menuitem" tabindex="-1" href="#">数据挖掘</a>         </li>         <li role="presentation">             <a role="menuitem" tabindex="-1" href="#">数据通信/网络</a>         </li>         <li role="presentation" class="divider"></li>         <li role="presentation">             <a role="menuitem" tabindex="-1" href="#">分离的链接</a>         </li>     </ul> </div>