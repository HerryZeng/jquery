## JQuery安装
---

### 网页中添加JQuery

可以通过多种方法在网页中添加JQuery，你可以使用以下方法：
+ 从[jquery.com](jquery.com)下载JQuery库
+ 从CDN中载入JQuery，如从Google中加载JQuery

### 下载JQuery

有两个版本的JQuery可供下载
+ Production Version:  用于实际的网站中，已被精简和压缩
+ Development Version: 用于测试和开发（未压缩，是可读写的代码）

JQuery库是一个`JavaScript`文件，可以使用`HTML`标签引用它：
```html
<head>
    <script src="jquery-3.3.1.min.js"></script>
</head>
```
是否很疑惑为什么我们没有在`<script>`标签中使用`type="text/javascript"`,在HTML5中，不必这样做，`JavaScript`是HTML5以及所有现代浏览器中默认脚本语言。