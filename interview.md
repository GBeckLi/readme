HTMl

1: Doctype的作用

  答案：doctype的作用是用来声明文档类型的，文档类型有三种：怪异模式，部分怪异模式，标准模式。使用<Doctype html>会告诉浏览器使用标准模式对页面进行渲染。可以使用document.compatMode来检查当前模式。当返回值为BackCompat时为怪异模式，当返回值为CSS1Compat时为标准模式。

2： div+css的布局较table布局有什么优点

  答案：
  1：结构更加明了，符合W3C规范，结构，样式和行为分离，更易维护。
  2：布局更加灵活多变。
  3：布局改版更加容易。
  4：利于SEO
  5：首页加载速度更快。table需要将所有东西都加载完再显示，div+css是边加载边显示。

3： strong与em的区别

  答案：
  1：语义上，em表示强调，strong表示更强烈的强调，em为局部强调，strong为全局性强调；em表示内容的重点，会改变句子的语义，strong表示强烈的重要性，紧迫性，严重性，但是不会改变语义。
  2：表现上，em为斜体，strong为粗体

4：渐进增强和优雅降级

  答案：
  优雅降级：一开始就构建站点的完整功能，然后针对浏览器测试和修复。比如一开始使用 CSS3 的特性构建了一个应用，然后逐步针对各大浏览器进行 hack 使其可以在低版本浏览器上正常浏览。

  渐进增强：一开始就针对低版本浏览器进行构建页面，完成基本的功能，然后再针对高级浏览器进行效果、交互、追加功能达到更好的体验。


5：为什么用多个域名来存储网站资源会更有效？

  答案：
  1：静态资源和动态资源分服务器存放可以提升服务器的相应效率。
  2：由于浏览器对于同一个域名下的资源会有并发请求数的限制，一般为2-8个不等。使用多个域名可以提升资源加载速度。
  3：跨域不会传cookie，可以节省带宽。像请求图片等资源没有必要携带cookie

6： Cookie，sessionStorage，localStorage的区别？

  答案：
  cookie：分为内存cookie和硬盘cookie两种，内存cookie存在内存中，当浏览器关闭时就会被清理。硬盘cookie保存在硬盘中，  除非用户手动清理或者过期，否则一直存在。
    缺点：(1):cookie会附加在每个HTTP请求上，浪费带宽；(2):cookie是明文的，有安全问题；(3):cookie大小只有4k左右，只能用于简单的存储。(4): 不可跨域使用。
  sessionStorage：5M左右，当页面关闭时被清除，刷新不会重新设置
  localStorage：5M左右，只有用户主动清除才会被清除。


7：src和href的区别

  答案：
  src: 指向外部资源，将外部资源下载并应用到当前文档中,会阻塞其他资源的加载
  href: 指向外部资源，建立资源和当前文档或者锚点的链接，会下载链接中的资源，但不会阻塞

8：HTML结构的语义化

  答案：