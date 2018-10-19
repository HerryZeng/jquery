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
