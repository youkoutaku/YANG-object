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
	<!-- 注释 -->
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

# 3.HTML结构
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
<link type="text/css" rel="stylesheet" hre="css/text.css">
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

## ★CSS属性
- color：文本颜色
- top：指定元素顶部的位置
- text-align：左对齐 or 右对齐 or center
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
### by name
- Auqa
- Black
- Blue
...

```css
body{
	background-color: silver;
}
```

### rgb
- %
```css
body{
	background-color: rgb{80%, 40%, 0%};
}
```
- 0~255
```css
body{
	background-color: rgb{204, 102, 0};
}
```

### hexadecimal（16进制）
	#(red)(green)(blue)
 
```css
body{
	background-color: #cc6600;
}
```

# 9.盒模型
## 内容区
元素中的内容所在的区域

## 内边距(padding)
内容区的周围有一层内边距，可选的，且透明。
```css
.menu{
	padding: 25px;
	padding-left: 80px;
}
```

## 边框(border)
元素周围的边框，包围着内边距，实际上是一条线，可以设定width，color与stlye
```css
.menu{
	border-color: black;
	border-width: 1px;
	border-style: solid;
}
```
### border-style
- solid
- double
- groove(糟线？)
- outset(外凸)
- dotter(虚线)
- dashed(破折线)
- inset(内凹)
- ridge(凸起)

### border-width
- thin
- medium
- thick
- px

### border-color
- red/green/blue/...
- rgb(100%, 0%, 0%)
- \#ff0000

### border-top/right/left/bottom
```css
.menu{
	border-top-color:
	border-left-style:
	border-bottom-width:
}
```
### border-radius(边框圆角)
```css
.menu{
	border-top-left-radius:     3em;
	border-top-right-radius:    3em;
	border-bottom-left-radius:  3em;
	border-bottom-right-radius: 3em;
}
```

## 外边距(margin)
外边距也是可选的，包围着边框。无颜色或装饰，在不同元素之间增加空间。
```css
.menu{
	margin: 30px;
	margin-right: 250px;
}
```

## background-image
```css
.menu{
	background-image:url(../image/b.jpg)
	}
```
### background-position
- top
- left
- right
- bottom
- center

### background-repeat
- repeat
- no-repeat
- repeat-x
- repeat-y
- inherit(继承父元素的设置)

## id
对于唯一的元素用CSS时，使用唯一的id去定义。
```html
<p id="menu">Please steal this page.</p>
```
注)一种元素可以有id的同时，属于一个class。

### id selector
```css
#menu {
	color: red;
}
p#menu{
	color: red;
}
```

## More CSS
```html
<head>
	<link type="text/css" rel="stylesheet" hre="css/text.css"> 
	<link type="text/css" rel="stylesheet" hre="css/menu.css"> 
	<link type="text/css" rel="stylesheet" hre="css/plog.css"> 
</head>
```
优先级：下面的优先级高

### media type
多个CSS可以用于对应不同的设备等。
```html
<html>
	<head>
		<link type="text/css" rel="stylesheet" hre="css/text.css" 
		  media="screen and (max-device-with:480px)">
		  /*有屏幕的设备且屏幕宽度不超过480px*/ 
		<link type="text/css" rel="stylesheet" hre="css/text.css" 
		  media="print">
		  /*为打印机*/
	  </head>
</html>
```
### media search(CSS)
```css
@media screen and (min-device-with: 481px){
	.menu{
		margin-right: 250px
	}
}
@media screen and (max-with: 480px){
	.menu{
		margin-right: 30px
	}
}
@media print{
	body{
		font-family:
	}
}
```
[media属性大全](https://www.w3.org/TR/mediaqueries-3/#media1)

# 10.div and span
## div
相当于各种元素的一个组
```html
<div id="menu">
	<h1></h1>
	<p></p>
	<img src="">
</div>
```
### id selector for div
```css
#menu{
	background-image:url(../img/menu.jpg);
}
```
### width
用width指定内容区的宽度
```css
#menu{
	width:40px;
}
```
### 子孙选择器
```css
div h1{
	color:black;
}
#menu h1{
	color:black;
}
```

## span
内嵌式逻辑组
```html
<span class="book"> Head First HTML and CSS </span>
```
```css
.book{
	font-style: italic;
}
```

## 简写
```css
#menu{
	padding: 0px 20px 30px 10px;/*top-right-bottom-left*/
	margin:  0px 20px 30px 10px;/*top-right-bottom-left*/
	padding:               20px;/*top=right=bottom=left*/
	border:  thin solid #007e7e;/*width-style-color*/
	background:withe url(../img.jpg) repeat-x 
	/*color-image-repeat*/
}
```
## style of a (Pseudo-class) 
- link
- visited
- hover
这些都允许指定style，但并没有在html中设置为class。因此它们被称谓伪类（Pseudo-class）.
```css
#menu a:link{
	color:green;
}
#menu a:visited{
	color:  red;
}
#menu a:hover{
	background:red;
	color: yellow;
}
```

## 层叠
对于一个页面来说，有三个CSS。
- 最优先的是作者提供的CSS。
- 其次是读者可以浏览器的设置更改CSS。
- 最后是浏览器默认的CSS。

### 排序
1) 收集所以CSS
2) 找到排序属性的所有声明
3) 利用"作者-读者-浏览器"排序
4) 利用"特定性"排序
5) 对于冲突规则，按最下面的优先

# 11. 布局与定位
## 布局
### flow
- 对于box and block elemen，从上至下的布局
- 对于内联元素，从左上至右下的布局

### 布局时的外边框
- 在左右排放元素时，元素间的距离为双方元素外边距的和
- 在上下排放元素时，共用外边距，因此距离为最大外边距
### liquid layouts(流动布局)
#### float
让元素独立与主流，且主流的元素会围绕float之后的元素。
```css
#menu{
	width: 200px;
	float:left;
}
```

#### clear
通过clear可以避免这一元素某一方向与float元素出现重叠问题.
```css
#footer{
	clear: right;
}
```
#### float main
对于小设备来说，浮动的侧栏会影响到主内容阅读，用户需要滚动页面才能了解到主内容，因此可以将主内容float以解决此问题。

### frozen layouts(冻结布局)
通过指定元素的宽度，固定元素内容大小，即冻结布局
```css
#allcontent{
	width: 800px;
	padding-top: 5px;
	padding-bottom: 5px;
	background-color: #675c47;
}
```

### Jello(凝胶布局)
凝胶布局 ，在冻结布局与流动布局之间。内容固定居中，但没有固定的外边距。
```css
#allcontent{
	width: 800px;
	padding-top: 5px;
	padding-bottom: 5px;
	background-color: #675c47;
	margin-left: auto;
	margin-right: auto;
}
```

## position(定位)
- static(静态：正常流入页面)
- absolute（对于父元素的绝对定位）
- fixed（对于浏览器窗口的固定定位）
- relative（相对定位：流入页面，但需要相对偏移）

### 绝对定位
```css
#menu{
	position: absolute;
	top: 150px;
	left: 100px;
	width: 400px;
}
```
#### 重叠的绝对定位(z-index)
```css
#div1{
	position: absolute;
	top: 150px;
	left: 100px;
	width: 400px;
	z-index: 0;
}
#div2{
	position: absolute;
	top: 150px;
	left: 100px;
	width: 400px;
	z-index: 1;
}
```
### 固定定位
```css
#menu{
	position: fixed;
	top: 5%px;
	left: 10%px;
	width: 200px;
}
```

## CSS表格
```html
	<div id="tableContainer"> <!--表格--->
		<div id="tableRow"> <!--第一行-->
			<div>    <!--第1列-->
			</div>
			...
			<div>    <!--第n列-->
			</div>
		</div>
		...
		<div id="tableRow"> <!--第n行-->
			<div>    <!--第1列-->
			</div>
			...
			<div>    <!--第n列-->
			</div>
		</div>
	</div>
```

```css
div#tableContainer{
	display: table;/*作为表格*/
	border-spacing: 10px;/*表格中的单元格增加10外边距*/
}
div#tableRow{
	display: table-row;/*作为表格中的第一行*/
}
#main{
	display: table-cell;
	vertical-align: top;/*表格内容上对齐*/
}
#sidebar{
	display:table-cell;
	vertical-align: top;/*表格内容上对齐*/
}
```


# 12.HTML5
## header(页眉)

## section(文章)

## aside(导航)

## footer(页脚)

# 13.表格与更多列表


# 14. HTML表单：实现交互


# 附录
