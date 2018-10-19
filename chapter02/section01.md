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