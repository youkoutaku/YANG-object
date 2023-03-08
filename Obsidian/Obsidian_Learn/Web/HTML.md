# 1.HTML
HTML:HyperText Markup Language

## ML
### head & title
```html
<html>
	<head>
		<title></title>
	</head>
<\html>
```

### body
### h1,h2...
### p
```html
<html>
	<head>
		<title></title>
	</head>
	<body>
		<h1></h1>
			<p></p>
		<h2></h2>
			<p><p>
	</body>
<\html>
```

- 标记文法
```html
<html>
	<head>
		<title></title>
	</head>
	<body>
		<h1>一级标题</h1>
		<h2>二级标题</h2>
		<p>一个段落</p>
	</body>
</html>
```

### Style
(CSS)样式
CSS:Cascading Style Sheets(层叠样式表)
```html
<html>
	<head>
		<title></title>
		<style type = "text/css">
			body{

                background-color:#d2b48c; <--背景颜色-->

                margin-left: 20%; <--字体·-->

                margin-right: 20%;

                border: 2px dotted black;

                padding: 10px 10px 10px 10px;

                font-family: sans-serif;

            }
        </style>
	</head>
	<body>
		<h1>一级标题</h1>
		<h2>二级标题</h2>
		<p>一个段落</p>
	</body>
</html>
```
# 2.HL
## 超文本
### a元素
```html
<--a元素-->
<a href="URL/.html">text</a>
```
a元素可以把图片，标题等作为链接的窗口。

## 属性(Attributes)

## 组织
管理资源及附页面
```html
<--a元素-->
<a href="URL/.html">text</a>
```

# 3.HTMLの仕組み
## em
斜体
```html
	<em></em>
```
## q元素
引用功能，作为段落中的一部分⇒inline元素
```html
<--q元素-->
<q>text</q>
```
## blockquote
长引用，独立存在⇒块元素
```html
<--q元素-->
<blockquote>text</blockquote>
```
q与blockquote是文章结构化的关键。

## br元素
换行
```html
<--q元素-->
<blockquote>
	Mrs Judy,<br>
	I wish...
</blockquote>
```

## 列表元素(li)
### 有序列表（ol）
```html
<--li元素-->
	<ol>
			<li>数学</li>
			<li>物理</li>
			<li>化学</li>
			<li>生物</li>
			</ol>
```

### 无序列表（ul）
```html
<--li元素-->
	<ul>
			<li>数学</li>
			<li>物理</li>
			<li>化学</li>
			<li>生物</li>
	</ul>
```
列表元素是，块元素。

## 特殊字符
&

# 4.发布web
## 服务器

## 域名

## 上传

## FTP

## URL

## HTTP

## 绝对路径

## titile in a
```html
<a href="http://www.google.com"
   title="go to the website">Googke</a>
```

## id
### 为h标题添加id
```html
<head>
	<title>youkoutaku.github.io</title>
</head>
<body>
<h1 id="math">Math</h1>
</body>
```

跳转至链接的特殊id位置
```html
<a href="youkoutaku.github.io#math"
   title="go to the website">youkoutaku</a>
```

## target
打开新的窗口显示页面
```html
<a target="_blank_" href="youkoutaku.github.io#math"
   title="go to the website">youkoutaku</a>
```

# 5.网页中的图像
## 图像
### JPEG
### GIF
### PNG

## Img
### 本地图片
```html
	<img scr="../imp/p.jpg">
```
### 网络图片
```html
	<img scr="http://www.xxxx.com/xx/xx/xx.jpg">
```
### alt 
为无法加载图像的用户提供指示。
```html
	<img scr="http://www.xxxx.com/xx/xx/xx.jpg" 
		alt="This is a ...">
```
### Image Size
- width
- height

```html
	<img src="../img/food.jpg" 
		width="48" height="100">
```
注)虽然可以通过img属性调节图片的大小，但是更好的做法是改变图片文件的大小。

## 缩略图(thumbnail)
通常情况下，制作一个专用的缩略图文件夹来存放所有图片的缩略图，在页面中展示缩略图，并使用a元素来链接至原图地址。为此我们可以为每一个照片创造一个html页面.

```html
<a href ="html/xxxx.html">
	<img scr=".../thumbnails/food.jpg" 
		alt="This is a ...">	
</a>
```

# 6.标准：严格的HTML
- HTML 1.0~2.0
- HTML 3
- HTML4
- HTML4.01
- XTHML
- **HTML5**

## HTML5定义
```html
<!doctype html>
```
向后兼容性

## 校验工具（web）
 
## meta
selact encoding
```html
<!doctype html>
<head>
	<meta charset="utf-8">
</head>
```

## 注意事项
- doctype开头
- 接着html元素
- html中的head与body
- head中的meta指定字符编码
- head中的title
- 元素间的嵌套
- 检查属性

# 7.CSS入门
对于元素的样式进行修饰
```css
body{

    background-color:#d2b48c;

    margin-left: 20%;

    margin-right: 20%;

    border: 2px dotted black;

    padding: 10px 10px 10px 10px;

    font-family: sans-serif;

}

p{

    background-color: red;

    border: 1px solid gray;

}

h1, h2{

    font-family: sans-serif;

    color: gray;

}

h1{

    border-bottom: 1px solid black;

}
```
## link元素
- link：链入外部信息
- type：信息类型
- rel：html与链接的关系
- hre：链接

### link to css
```html
<link type="text/css" rel="stylesheet" hre="css/text.css"
```

## 元素继承
对于css中元素的一部分属性（如字体），元素中的其他元素会继承这一属性。
```css
body{
	font-family: sans-serif;
}
```
## 覆盖继承
CSS会优先与最特定的规则。
```css
body{
	font-family: sans-serif;
}
p{
	font-family: serif;
}
```
## Class

例：为某个p元素分类
```html
	<p class="menu">
		...
	<\p>
```

### Class Selector

例：对p元素的menu类
```css
	p.menu{
		color: black;
	}
```
### Classes
```css
	blockquote.greentea, p.menu{
		color: black;
	}
```

### one Class
对所有元素的类
```css
	.menu{
		color:black;
	}
```

### more Classes
```html
	<p class="menu note logo">
		...
	<\p>
```

## 优先级
- Class  Selector
- 继承
- 默认
### 定义重复
- 当优先级相同而定义重复时，以最后的规则为准。

## 校验CSS

## CSS属性
- color：文本颜色
- top：指定元素顶部的位置
- text-align：左对齐or右对齐
- letter-spacing：字母之间的设置
- backgound-color：背景颜色
- border：在元素周围加边框
- font-style：设置斜体文本
- list-style：列表外观
- padding：内边距（内容与边缘之间距离）
- left：指定元素左边所在的位置
- line-height：元素中的行间距
- font-size：字体大小
- background-image: 元素背景图
- ...

# 8.字体与颜色
## 文本
### font-family
设定字体
```css
body{
	font-family: Verdana, Geneva, Arial, sans-serif;
}
```

### font-size
字体大小
```css
body{
	font-size: 14px;
}
```

### color
```css
body{
	color: silver;
}
```

### font-weight
字体粗细
- lighter
- normal
- bold
- bolder

```css
body{
	font-weight: bold;
}
```

### font-style
- 斜体(ltalic)
- 倾斜(oblique)

```css
p.menu{
	font-style:italic;
}
```

### text-decoration
修饰
- none
- underline
- overline
- line-through
```css
body{
	text-decoration: underline;
}
```

## 字体系列
- Sans-serif
- Serif
- Monospace
- Cursive
- Fantasy

### web字体font-face
- TrueType: .ttf
- OpenType: .otf
- Embedded OpenType: .eot
- SVG: .svg
- web: .woff

## Size
- px
- %
- em
```css
body{
	font-size:14px;/*默认字体大小*/
}
h1{
	font-size:150%;
}
h2{
	font-size:1.2em;
}
```
- 关键字
	- xx-small
	- x-small
	- small
	- medium
	- large
	- x-large
	- xx-large

## Web Color

# 9.盒模型

# 10.div and span

# 11. 布局与定位
## 布局
## 排版

# 12.HTML5标记

# 13.表格与更多列表

# 14. HTML表单 

# 附录
