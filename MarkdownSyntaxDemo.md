# 前言

> 最近在开源个人的实战react-native项目和微信小程序项目，等项目开发完成后，打算写几篇详细的关于实战项目的技术博客，首先想到的就是使用简书，但是写简书需要知道Markdown常用的语法，于是乎就在网上搜一些介绍Markdown语法的博客，发现博主们总结的Markdown语法基本上都不是很全面，所以索性自己做一个Markdown语法的史上最全面总结。

# 认识 Markdown
> Markdown 是一种用来写作的轻量级「标记语言」，它用简洁的语法代替排版，而不像一般我们用的字处理软件 Word 或 Pages 有大量的排版、字体设置。它使我们专心于码字，用「标记」语法，来代替常见的排版格式。例如此文从内容到格式，甚至插图，键盘就可以通通搞定了。目前来看，支持 Markdown 语法的编辑器有很多，包括很多网站（例如简书）也支持了 Markdown 的文字录入。Markdown 从写作到完成，导出格式随心所欲，你可以导出 HTML 格式的文件用来网站发布，也可以十分方便的导出 PDF 格式。

# Markdown 的优点

> * 页面内容可读性强，简洁直观。
> * 纯文本，兼容性强，几乎任何文本编辑器都可打开。
> * 格式转换简便，轻松的导出HTML、PDF、.md等多种格式文件。
> * 不需太过于关心页面排版，只需关注内容。

# Markdown 官方文档

[创始人 John Gruber 的 Markdown 语法说明](https://daringfireball.net/projects/markdown/syntax)

[Markdown 中文版语法说明](http://wowubuntu.com/markdown/#list)

# 常用的Markdown工具

![MacDown logo](http://upload-images.jianshu.io/upload_images/6342050-90f0cce4e19be7c9.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

### MacOS平台(个人推荐使用Macdown)

**在 Mac OS X 上，个人强烈建议使用 Macdown 这款免费且十分好用的 Markdown 编辑器，它支持实时预览，既左边是你编辑 Markdown 语言，右边会实时的生成预览效果。**

![Macdown](http://upload-images.jianshu.io/upload_images/6342050-96ae1052c31645c9.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

### Windows平台

**Windows用户建议尝试以下两款产品：**

* MarkdownPad 

* MarkPad

# Markdown 语法的简要介绍

[1.换行符](#换行符)

[2.强调(Strong and Emphasize)](#强调)

[3.标题(Headers)](#标题)

[4.URL链接](#URL链接)

[5.引用图片](#引用图片)

[6.列表](#列表)

[7.引用](#引用)

[8.Inline Code](#InlineCode)

[9.Block Code](#BlockCode)

[10.Code Block](#CodeBlock)

[11.分割线](#分割线)

[12.表格](#表格)

[13.锚点](#锚点)

[14.del标签](#del)

[15.u标签](#u)

[16.mark标签](#mark)

[17.font标签](#font)

<a id="换行符"></a>
### 1.换行符(Line Breaks)
> 在Markdown语法中，换行需要敲两个回车键，即在两段文本之间添加一个空行来达到换行的效果。

*敲一个回车键*

**这是第一个段落**
**这是第二个段落**

*上面的写法在编辑器中显示是两行，但是在Macdown预览效果发现，他们还是在同一行，只是两个段落中间多出来一个空格。(注意：简书中的效果是两行显示的，在简书中编辑时，敲一个回车键即可实现换行效果!)*

**这时我们在两行中间多敲一个回车键就能达到换行的效果**

*敲两个回车键键的效果：*

**这是第一个段落**

**这时第二个段落**

*有同学发现，我本来只是想让同一句话换个行显示而已，你这中间还多出来一空行，不够美观。能不能中间没有留白的空行，但是也能实现换行的效果尼？当然办法总是有的，下面就介绍第二种换行方式。*

**另一种方式实现换行的方式，两个段落之间没有空行**
> 官方解释：To force a line break, put two spaces and a newline (return) at the end of the line.

*在同一段落中，在需要换行的字符后敲两个空格，再敲回车键就能达到同一段落换行的效果*

*例如这样：*

**这是第一个段落**  
**这时第二个段落**

<a id="强调"></a>
### 2.强调(Strong and Emphasize)
> 在Markdown语法中，想要着重强调某一部分内容时，可以使用`*`或者是`_`来包裹要着重强调的内容。`**`或`__`表示字体加粗，`*`或`_`表示字体斜体，（个人推荐使用`*`）

*这里的内容强调分两种语法，一种是字体加粗强调，另一种是为斜体强调*

1. 加粗（**可以使用快捷键生成加粗符号：Command+b**）

* 方式1：**这是字体加粗强调**
* 方式2：__这是字体加粗强调__

2. 斜体（**可以使用快捷键生成斜体符号：Command+i**）

* 方式1：*这是斜体强调*
* 方式2：_这是斜体强调_

<a id="标题"></a>
### 3.标题(Headers)
> 在Markdown语法中，添加标题使用`#`，就会有标题加粗的效果出现。标题分为六个等级，即1个#代表一级标题，2个#代表二级标题，直到六级标题。

# Header 1
## Header 2
### Header 3
#### Header 4
##### Header 5
###### Header 6

*这可以使用下面的方式来设置一级、二级标题，不过不推荐使用。*

Header 1
========
Header 2
---------

<a id="URL链接"></a>
### 4.可点击URL链接(Links and Email)
> 在写自己的博客中，经常有需求要跳转到某一个网页或者邮件。这时需要使用link链接。link链接方式分为内联(Inline)和外部引用(Reference)

* Inline

*将邮箱地址包裹在<>内部，就形成了可以点击的邮箱地址: <1126756952@qq.com>*

*<a name="markdown-anchor"></a>*

*将网页url包裹在<>内部，就形成了可以点击访问的网页地址: <http://www.jianshu.com/u/023338566ca5>*

*自定义网页链接的标题`[标题](链接)`: [光强的简书](http://www.jianshu.com/u/023338566ca5)*

* Reference (外部引用的好处可以在整个文章中重复引用网页地址或者图片地址而不需要多些拷贝同一个url)

*Make [a link][arbitrary_id] `[a link][arbitrary_id]`*
  
*[like this][] `[like this][]`*

[arbitrary_id]: http://www.jianshu.com/u/023338566ca5
[like this]: http://www.jianshu.com/u/023338566ca5

<a id="引用图片"></a>
### 5.引用图片
> Markdown中引用图片资源同样也是分为内联(Inline)和外部引用(Reference)

* Inline

 *语法：*

`![Alt Image Text](图片地址)`

*使用方式：* 

![Alt Image Text](http://upload-images.jianshu.io/upload_images/6342050-4dba8fa19b2fef6e.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

* Reference  

*语法*  

`![Alt Image Text][image-id]`

`[image-id]: http://ovyjkveav.bkt.clouddn.com/17-10-19/15885901.jpg`

*使用方式：*

![Alt Image Text][image-id]

[image-id]: http://ovyjkveav.bkt.clouddn.com/17-10-19/15885901.jpg

<a id="列表"></a>
### 6.列表
> Markdown语法中，列表分为三类：有序列表、无序列表、嵌套列表

* ####有序列表

1. 列表1
2. 列表2
3. 列表3

* ####无序列表(无序列表中，`*`、`+`、`-`效果一样，个人推荐使用`*`)

* 列表1
* 列表2
+ 列表4
+ 列表5
- 列表7
- 列表8

* ####缩进层次嵌套列表

	* 这是一个嵌套列表
		1. 列表1
		2. 列表2
		3. 列表3

<a id="引用"></a>
### 7.引用(Block Quote)
> Markdown语法中，使用`>`表示引用，引用名人名言或者是别人的一段文本等。

---

> "三天不学习，赶不上刘少奇。" - 毛泽东 

*当然引用也可以嵌套使用的*

> 这时一级引用
>> 这时二级引用
>>> 这时三级引用  
>>> 还是三级引用

>> 二级引用

> 一级引用

*引用也可以和其他的markdown语法混合使用*

> ###这是一级引用
>> *这是二级引用*
>>> * 这是三级引用  
>>> * 还是三级引用
>>> 1. 还是三级标题
>>> 1. 还是三级标题

>> **二级引用**

> [一级引用][arbitrary_id]

<a id="InlineCode"></a>
### 8.Inline Code
>内嵌文本，当我们想让某一文本内容内嵌在边框内，我们可以使用一对反引号包裹内容:`内容`

**使用方式：**

*内容本身不包含反引号*

* `Inline code`

*内容本身包含反引号。当文本内容中正好包含有反引号，这时需要使用空格隔开：*

* ``code has `backticks` ``

* ```` ``Code with `backticks` `` ````
 
<a id="BlockCode"></a>
### 9.Block Code(不推荐使用)
> 当我们敲4个空格键或者是一个tab键，这样就形成一个代码块区域。

**使用方式：**

	print('This is a code block')
	print('The block must be preceded by a blank line')
	print('Then indent at least 4 spaces or 1 tab')
	print('Nesting does nothing. Your code is displayed Literally')

<a id="CodeBlock"></a>
### 10.Code Block
> 对于程序员来说，很多时候我们写技术博客都需要贴上自己的代码来给读者讲解，这时就用到了代码引用语法：三个反引号```Code```或者三个波浪号~~~Code~~~。

* 方式1

```
render() {
    	const dataArr = this.state.dataSource
    	return (
     	 <ListView
        	style={styles.listStyle}
        	dataSource={dataArr}
        	renderRow={this.renderRow}
        	renderSeparator={() => this._renderSeparator()}
      	/>
    )
  }
```

* 方式2

~~~
render() {
    	const dataArr = this.state.dataSource
    	return (
     	 <ListView
        	style={styles.listStyle}
        	dataSource={dataArr}
        	renderRow={this.renderRow}
        	renderSeparator={() => this._renderSeparator()}
      	/>
    )
  }
~~~

<a id="分割线"></a>
### 11.分割线(Horizontal Rules)
> 当我们想对文章的某些内容做上下分割，这时我们可以使用分割线语法：`***或---`

*在MacDown编辑器中，分割线分为粗线和细线。*

**注意：在简书中，`***`或`---`不显示粗线,只有细线，一个或者两个`-`也不显示细线**

* 粗线

***

or 

---

* 细线(细线只需一个或者两个`-`)

-

or 

--

<a id="表格"></a>
### 12.表格(Table)
> 表格的使用肯定我们每一位同学都不陌生，因为我们经常使用Excel表格来展示各种数据报表。很庆幸Markdown同样也支持表格制作，而且使用方式很简单。表格由行与列组成，这里只需要注意表格的内容对齐方式即可。

*没有设置对齐方式*

First Header  | Second Header
------------- | -------------
Content Cell  | Content Cell
Content Cell  | Content Cell

*中间表格对齐*

| Left Aligned  | Center Aligned  | Right Aligned |
|:------------- |:---------------:| -------------:|
| col 3 is      | some wordy text |         $1600 |
| col 2 is      | centered        |           $12 |
| zebra stripes | are neat        |            $1 |

**这里需要注意：表格的左边和右边的`|`可以省略不需要使用，表格左右两边加上`|`主要基于美观考虑，表格的对齐方式仅仅取决于`:`**

<a id="锚点"></a>
### 13.跳转到指定的内容位置(a标签)
>在写文章时，有时候我们有这样的需求，从文章的某一个位置直接跳转到指定的另一个位置，这时使用到a标签的锚点语法。

**注意: a标签跳转到指定位置在简书中无效**

*使用方式：*

**在待跳转到的位置上添加一行：`<a name="markdown-anchor"></a>`**

**`[*Markdown高级用法：* 跳转到作者的简书链接处](#markdown-anchor)`：通过name就可以找到指定的位置**

[*Markdown高级用法：* 跳转到作者的简书链接处](#markdown-anchor)

<a id="del"></a>
### 14.中划线(del标签)
> 内容中间添加一条横线: `<del>xxx</del>`

**注意：del标签在简书中无效**

First Header  | Second Header
------------- | -------------
Content Cell  | <del>Content Cell</del>
Content Cell  | Content Cell  

<a id="u"></a>
### 15.下划线(u标签)
> 内容底部添加一条横线: `<u>xxx</u>`

**注意：u标签在简书中无效**

First Header  | Second Header
------------- | -------------
Content Cell  | <u>Content Cell</u>
Content Cell  | Content Cell

<a id="mark"></a>
### 16.标记(mark标签)
> 内容颜色高亮处理: `<mark>xxx</mark>`

**注意：mark标签在简书中无效**

First Header  | Second Header
------------- | -------------
Content Cell  | <mark>Content Cell</mark>
Content Cell  | Content Cell 

<a id="font"></a>
### 17.修改文字颜色(font标签)
> 设置文本的字体颜色: `<font color=Red>xxx</font>`

**注意：font标签在简书中无效**

<font color=Red>修改文本的字体颜色为红色</font>

# 注意事项

* 换行符MacDown编辑器和简书编辑器语法效果上略有不同
* 简书编辑不支持快捷键生成标签
* 在简书中，`***`或`---`不显示粗线,只有细线，一个或者两个`-`也不显示细线
* 简书中使用a标签跳转到指定的位置没有效果
* 简书中使用del、u、mark、font等标签都没有效果

#总结

**以上内容是作者花了好几个小时总结出来的常用Markdown语法，介绍了Markdown的十几种常用的语法知识，并逐一的进行了示例展示。可以说足以满足读者们日常中各种使用Markdown编写文章的需求。老铁们要是感觉文章对您有帮助，请 点赞 关注 666**

*最后再啰嗦一句：一定要趁热打铁！*

**强烈建议读者们认真浏览作者的这篇文章后，自己使用Markdown写一篇文章，体会一下Markdown语法的优雅之处！**