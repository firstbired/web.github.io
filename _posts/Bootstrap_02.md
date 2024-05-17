---
layout: post
author: jqt
---
- ## HTML 5 文档类型（Doctype）

  Bootstrap 使用了一些 HTML5 元素和 CSS 属性。为了让这些正常工作，您需要使用 HTML5 文档类型（Doctype）。 因此，请在使用 Bootstrap 项目的开头包含下面的代码段。

  ```
  <!DOCTYPE html>
  <html>
  ....
  </html>
  ```

  如果在 Bootstrap 创建的网页开头不使用 HTML5 的文档类型（Doctype），您可能会面临一些浏览器显示不一致的问题，甚至可能面临一些特定情境下的不一致，以致于您的代码不能通过 W3C 标准的验证。

  ## 移动设备优先

  移动设备优先是 Bootstrap 3 的最显著的变化。

  在之前的 Bootstrap 版本中（直到 2.x），您需要手动引用另一个 CSS，才能让整个项目友好的支持移动设备。

  现在不一样了，Bootstrap 3 默认的 CSS 本身就对移动设备友好支持。

  Bootstrap 3 的设计目标是移动设备优先，然后才是桌面设备。这实际上是一个非常及时的转变，因为现在越来越多的用户使用移动设备。

  为了让 Bootstrap 开发的网站对移动设备友好，确保适当的绘制和触屏缩放，需要在网页的 head 之中添加 **viewport meta** 标签，如下所示：

  ```
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  ```

  *width* 属性控制设备的宽度。假设您的网站将被带有不同屏幕分辨率的设备浏览，那么将它设置为 *device-width* 可以确保它能正确呈现在不同设备上。

  *initial-scale=1.0* 确保网页加载时，以 1:1 的比例呈现，不会有任何的缩放。

  在移动设备浏览器上，通过为 **viewport meta** 标签添加 *user-scalable=no* 可以禁用其缩放（zooming）功能。

  通常情况下，*maximum-scale=1.0* 与 user-scalable=no 一起使用。这样禁用缩放功能后，用户只能滚动屏幕，就能让您的网站看上去更像原生应用的感觉。

  注意，这种方式我们并不推荐所有网站使用，还是要看您自己的情况而定！

  ```
  <meta name="viewport" content="width=device-width, 
                                       initial-scale=1.0, 
                                       maximum-scale=1.0, 
                                       user-scalable=no">
  ```

  ## 响应式图像

  ```
  <img src="..." class="img-responsive" alt="响应式图像">
  ```

  通过添加 *img-responsive* class 可以让 Bootstrap 3 中的图像对响应式布局的支持更友好。

  接下来让我们看下这个 class 包含了哪些 css 属性。

  在下面的代码中，可以看到*img-responsive* class 为图像赋予了 max-width: 100%; 和 height: auto; 属性，可以让图像按比例缩放，不超过其父元素的尺寸。

  ```
  .img-responsive {
    display: block;
    height: auto;
    max-width: 100%;
  }
  ```

  这表明相关的图像呈现为 *block*。当您把元素的 display 属性设置为 block，以块级元素显示。

  设置 *height:auto*，相关元素的高度取决于浏览器。

  设置 *max-width* 为 100% 会重写任何通过 width 属性指定的宽度。这让图片对响应式布局的支持更友好。

  如果需要让使用了 .img-responsive 类的图片水平居中，请使用 .center-block 类，不要用 .text-center。