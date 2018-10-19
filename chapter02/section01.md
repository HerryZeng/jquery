## jQuery 效果- 隐藏和显示

---

隐藏、显示、切换，滑动，淡入淡出，以及动画，哇哦！

---

### jQuery hide() 和 show()

通过 jQuery，您可以使用 `hide()` 和 `show()`方法来隐藏和显示 HTML 元素：
```jquery
$("#hide").click(function(){
  $("p").hide();
});
 
$("#show").click(function(){
  $("p").show();
});
```

#### 语法:

```jquery
$(selector).hide(speed,callback);

$(selector).show(speed,callback);
```

可选的 speed 参数规定隐藏/显示的速度，可以取以下值："slow"、"fast" 或毫秒。

可选的 callback 参数是隐藏或显示完成后所执行的函数名称。

下面的例子演示了带有 speed 参数的 hide() 方法：
```jquery
$("button").click(function(){
  $("p").hide(1000);
});
```

### jQuery toggle()

通过 jQuery，您可以使用 toggle() 方法来切换 hide() 和 show() 方法。

显示被隐藏的元素，并隐藏已显示的元素：
```jquery
$("button").click(function(){
  $("p").toggle();
});
```

#### 语法:

```jquery
$(selector).toggle(speed,callback);
```
可选的 speed 参数规定隐藏/显示的速度，可以取以下值："slow"、"fast" 或毫秒。

可选的 callback 参数是隐藏或显示完成后所执行的函数名称。

#### 对于可选的 callback 参数，有以下两点说明：

1. `$(selector)`选中的元素的个数为n个，则callback函数会执行n次；

2. `callback`函数名后加括号，会立刻执行函数体，只会调用一次 而不是等到显示/隐藏完成后才执行；如果不加括号，元素显示或隐藏后调用函数，才会调用多次。

3. `callback`既可以是函数名，也可以是匿名函数；