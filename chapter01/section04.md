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