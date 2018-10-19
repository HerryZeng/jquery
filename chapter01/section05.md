## JQuery选择器

---
JQuery选择器允许你对HTML元素组或单个元素进行操作

---

### JQuery选择器

jQuery 选择器允许您对 HTML 元素组或单个元素进行操作。
jQuery 选择器基于元素的 id、类、类型、属性、属性值等"查找"（或选择）HTML 元素。 它基于已经存在的 CSS 选择器，除此之外，它还有一些自定义的选择器。

jQuery 中所有选择器都以美元符号开头：`$()`。

### 元素选择器

jQuery 元素选择器基于元素名选取元素。
在页面中选取所有`<p>`元素:
```jquery
$("p")
```

#### 实例

用户点击按钮后，所有`<p>`元素都隐藏：
```jquery
$(document).ready(function(){
  $("button").click(function(){
    $("p").hide();
  });
});
```

### #id 选择器