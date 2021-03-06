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

### `mouseleave()`
当鼠标指针离开元素时，会发生 mouseleave 事件。

mouseleave() 方法触发 mouseleave 事件，或规定当发生 mouseleave 事件时运行的函数：
```jquery
$("#p1").mouseleave(function(){
    alert("再见，您的鼠标离开了该段落。");
});
```

### `mousedown()`

当鼠标指针移动到元素上方，并按下鼠标按键时，会发生 mousedown 事件。

mousedown() 方法触发 mousedown 事件，或规定当发生 mousedown 事件时运行的函数：
```jquery
$("#p1").mousedown(function(){
    alert("鼠标在该段落上按下！");
});
```

### `mouseup()`

当在元素上松开鼠标按钮时，会发生 mouseup 事件。

mouseup() 方法触发 mouseup 事件，或规定当发生 mouseup 事件时运行的函数：
```jquery
$("#p1").mouseup(function(){
    alert("鼠标在段落上松开。");
});
```

### `hover()`

hover()方法用于模拟光标悬停事件。

当鼠标移动到元素上时，会触发指定的第一个函数(mouseenter);当鼠标移出这个元素时，会触发指定的第二个函数(mouseleave)。
```jquery
$("#p1").hover(
    function(){
        alert("你进入了 p1!");
    },
    function(){
        alert("拜拜! 现在你离开了 p1!");
    }
);
```

### `focus()`

当元素获得焦点时，发生 focus 事件。

当通过鼠标点击选中元素或通过 tab 键定位到元素时，该元素就会获得焦点。

focus() 方法触发 focus 事件，或规定当发生 focus 事件时运行的函数：
```jquery
$("input").focus(function(){
  $(this).css("background-color","#cccccc");
});
```

### `blur()`
当元素失去焦点时，发生 blur 事件。

blur() 方法触发 blur 事件，或规定当发生 blur 事件时运行的函数：
```jquery
$("input").blur(function(){
  $(this).css("background-color","#ffffff");
});
```