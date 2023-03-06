# 1.HTML
HTML:HyperText Markup Language

## HTMLのML
### head

### title

### body

### h1,h2...

### p

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
# 2.HTMLのHL
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

## imp
### 本地图片
```html
	<imp scr="../imp/p.jpg">
```
### 网络图片
```html
	<imp scr="http://www.xxxx.com/xx/xx/xx.jpg">
```
### alt 
为无法加载图像的用户提供指示。
```html
	<imp scr="http://www.xxxx.com/xx/xx/xx.jpg" 
		alt="This is a ...">
```

# 6.严格的HTML

# 7.XHTML

# 8.CSS

# 9.字体与颜色

# 10.盒模式

# 11.高级网站构建div and span

# 12. 布置元素
## 布局
## 排版

# 13.表格与列表

# 14. 交互：XHTML

# Go to HTML5
