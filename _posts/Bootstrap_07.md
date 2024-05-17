---
layout: post
author: jqt

---
# Bootstrap 多媒体对象（Media Object）

本章我们将讲解 Bootstrap 中的多媒体对象（Media Object），如：图像、视频、音频等。 多媒体对象的样式可用于创建各种类型的组件（比如：博客评论），我们可以在组件中使用图文混排，图像可以左对齐或者右对齐。媒体对象可以用更少的代码来实现媒体对象与文字的混排。

接下来我们先来看个实例：

## 实例

<!-- 左对齐 --> <div class="media">   <div class="media-left">     <img src="img_avatar1.png" class="media-object" style="width:60px">   </div>   <div class="media-body">     <h4 class="media-heading">左对齐</h4>     <p>这是一些示例文本...</p>   </div> </div>   <!-- 右对齐 --> <div class="media">   <div class="media-body">     <h4 class="media-heading">左对齐</h4>     <p>这是一些示例文本...</p>   </div>   <div class="media-right">     <img src="img_avatar1.png" class="media-object" style="width:60px">   </div> </div>