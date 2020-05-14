# DOM
DOM 是一种树状数据结构，在构建网站的过程中，HTML 元素通过嵌套构成 DOM 结构，上溯可以寻找到**父节点**（根节点），被内嵌的元素是**子元素**，同一级的元素是**兄弟节点**。浏览器会将收到的**所有 HTML 转换为 JavaScript 对象**，叫做[文档对象模型 DOM（Document Object Model）](https://developer.mozilla.org/zh-CN/docs/Web/API/Document_Object_Model)

文档对象模型 DOM 将 web 页面与到脚本或编程语言连接起来。通常是指  JavaScript，但将 HTML、SVG 或 XML 文档建模为对象并不是 JavaScript 语言的一部分。DOM模型用一个逻辑树来表示一个文档，树的每个分支的终点都是一个节点 node，每个节点都包含着对象 objects。DOM 的方法 methods 让你可以用特定方式操作这个树，用这些方法你可以改变文档的结构、样式或者内容。节点可以关联上事件处理器，一旦某一事件被触发了，那些事件处理器就会被执行。

## document
在 JavaScript 中 document 指的是当前状态的网页，document 即是 DOM，包含了网站可见元素的所有信息。通过 DOM 操作方法可修改网页的元素

### 访问元素
* 通过给定的 ID 获取单个页面元素对象 `getElementById("ID_name")`，注意方法名称中的单词 `Element `是单数形式，由于 `id` 属性是唯一的。
* 通过给定的 Class 获取多个页面元素对象 `getElementsByClassName("class_name")`，注意方法名称中的单词 `Elements` 是单词复数，由于 `class` 属性与元素并非一一对应。

### 访问元素属性
`.style` 属于 [DOM 属性](https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement.style)，用于更改所选页面元素的 CSS 样式。`.style` 之后的属性是这段代码将更改的 CSS 样式。[此处](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Properties_Reference)是你可以更改的所有 CSS 属性列表。

示例
```javascript
// 将 id 值为 education 的元素隐藏
document.getElementById("education").style.display = "none";
```