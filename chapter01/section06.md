## JQuery事件

---

JQuery是为事件处理特别设计的

---

### 什么是事件

页面对不同访问者的响应叫做事件。
事件处理程序指的是当`HTML`中发生某些事件时所调用的方法。
实例
+ 在元素上移动鼠标
+ 选取单选按钮
+ 点击元素

在事件中经常使用术语**触发**（或**激发**）,如，当你按下按键时触发`keypress`事件。
常见DOM事件

鼠标事件|键盘事件|表单事件|文档/窗口事件
---|---|---|---
click|keypress|submit|load
dbclick|keydown|change|resize
mouseenter|keyup|focus|scroll
mouseleave|hover|blur|unload

### JQuery事件方法语法

在JQuery中，大多数`DOM`事件都有一个等效的JQuery方法。
页面中指定一个点击事件
```jquery
$("p").click()
```
下一步是定义什么时候触发事件，你可以通过一个事件函数实现：
```jquery
$("p").click(function(){
    // 动作触发后执行的代码
});
```

### 常用的JQuery事件方法

#### `$(document).read()`

`$(document).read()`方法允许我们在文档完全加载后执行的函数。

### `click()`

`click()`方法是在按钮点击事件被触发时会调用一个函数。
在下面的实例中，当点击事件在某个`<p>`元素上触发时，隐藏当前`<p>`元素：
```jquery
$("p").click(function(){
    $(this).hide();
});
```
### `dbclick()`

当双击元素时，会发生`dbclick`事件
`dbclick()`方法触发`dbclick`事件，或规定当发生`dbclick`事件时运行的函数：
```jquery
$("p").dbclick(function(){
    $(this).hide();
});
```

### `mouseenter()`

当鼠标指针补穿过元素时，会发生mouseenter事件
`mouseenter()`方法触发mouseenter事件，或规定当发生mouseenter事件时运行的函数：
```jquery
$("#p1").mouseenter(function(){
    alert('你的鼠标移到了id="p1"的元素上！');
});
```

