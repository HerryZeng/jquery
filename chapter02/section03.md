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

## 替代方案

如果不希望下载并存储JQuery，那么也可以通过CDN(内容分发网络)引用它。
如果你的站点用户是国内的，建议使用百度、又拍云、新浪等国内CDN地址，如果你站点用户是国外的可以使用谷歌和微软。

```html
<head>
<script src="https://ajax.aspnetcdn.com/ajax/jQuery/jquery-3.3.1.min.js">
</script>
</head>
```

```html
<head>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.3.1/jquery.min.js">
</script>
</head>
```

使用 Staticfile CDN、百度、又拍云、新浪、谷歌或微软的 jQuery，有一个很大的优势：

许多用户在访问其他站点时，已经从百度、又拍云、新浪、谷歌或微软加载过 jQuery。所以结果是，当他们访问您的站点时，会从缓存中加载 jQuery，这样可以减少加载时间。同时，大多数 CDN 都可以确保当用户向其请求文件时，会从离用户最近的服务器上返回响应，这样也可以提高加载速度。