## JQuery语法
---

通过JQuery，可以选取（query）HTML元素，并对它们执行操作（actions）

---

### JQuery语法

JQuery语法是通过选取HTML元素，并对选取的元素执行某些操作。
基础语法：`$(selector).action()`
+ 美元符号定义JQuery
+ 选择符（`selector`）查询HTML元素
+ JQuery的`action()`执行对元素的操作

实例：
+ `$(this).hide()`    隐藏当前元素
+ `$("p").hide()`    隐藏所有`<p>`元素
+ `$("p.test").hide()` - 隐藏所有`class="test"`的`<p>`元素
+ `$("#test").hide()` - 隐藏所有`id="test"`的元素

>你对 CSS 选择器熟悉吗？
jQuery 使用的语法是 XPath 与 CSS 选择器语法的组合。在本教程接下来的章节，您将学习到更多有关选择器的语法。


### 文档就绪事件

您也许已经注意到在我们的实例中的所有 jQuery 函数位于一个 document ready 函数中：
```jquery
$(document).ready(function(){
 
   // 开始写 jQuery 代码...
 
});
```
这是为了防止文档在完全加载（就绪）之前运行 jQuery 代码，即在 DOM 加载完成后才可以对 DOM 进行操作。

如果在文档没有完全加载之前就运行函数，操作可能失败。下面是两个具体的例子：
+ 试图隐藏一个不存在的元素
+ 获得未完全加载的图像的大小

提示：简洁写法（与以上写法效果相同）:
```jquery
$(function(){
 
   // 开始写 jQuery 代码...
 
});
```