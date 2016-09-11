#“css揭秘”读书笔记
1. 父元素和子元素的字号关系：子元素使用百分比来设置，同时行高最好使用倍数设置
2. 涉及到：四个变量，其中一个特殊 的情况 把特殊的单独提出来 更便于维护
``` css
broder-width:10px;
border-left-width:0px
```

 3. currentColor 所有分割线的颜色跟文本颜色一致
```css
 hr{
	 height: .5em;
	 background: currentColor;
 }
```
4.  inherit 继承：
	把超链接颜色设置为钰页面中其他文本相同:
``` css
a {color:inherit}
```
提示框：小箭头自动继承背景边框样式
```css
.callout {position:relative}
.callout:before {
	content: '',
	position: absolute;
	top: -.5em; left: 1em;
	padding: .35em;
	background: inherit;
	border: inherit;
	border-right: 0;
	border-bottom: 0;
	transform: rotate(45deg);	
}
```