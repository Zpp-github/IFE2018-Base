### `setTimeout()`/`setInterval()`的第三个参数？  
`setTimeout(func, delay, param1, param2, ...)`，第三个参数及以后的参数都可以作为`func`函数的参数。  

### CSS Sprites是什么？  
它是一种网页图片应用处理方式：将一个页面涉及到的零星图片都包含到一张大图中去。这样一来，当访问该页面时，客户端只需要向服务器请求少量的图片，图片越多请求次数越少，造成延迟的可能性也就越小，能有效减轻服务器的压力;再利用CSS的“background-image”、“background-position”的组合进行背景定位，用数字精确地定位出背景图片的位置。

### `background-position`背景定位的原理？   
- 关键字：位置关键字可以按任何顺序出现，最多不能超过两个（一个对应水平方向，另一个对象垂直方向）。如果只出现一个关键字，则认为另一个关键字是`center`。如`background-position:top right;`，背景图片顶部与元素顶部对齐、背景图片右边与元素右边对齐，即它们的右上角重合。  

- 数值：背景图片左上角相对于元素左上角的偏移。如`background-position:10px 10px;`，即元素的左上角向右10像素、向下10像素的位置为背景图片的左上角。  

- 百分数：百分数值同时作用于元素和背景图片，如`background-pisition:40% 20%;`，则以左上角为起点，背景图片的水平40%、垂直20%位置与元素的水平40%、垂直20%位置对齐。如果只指定一个百分数值，所提供的这个值将用作水平方向，垂直方向将假设为50%。

### `getComputedStyle()`是什么？  
`element.style`只能获取元素行内样式；`getComputedStyle`是一个可以获取当前元素所有最终使用的CSS属性值，返回的是一个CSS样式声明对象([object CSSStyleDeclaration])，并且是只读，接受两个参数，第一个是元素，第二个是伪类，没有的话，为`null`。
