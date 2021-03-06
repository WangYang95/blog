# Markdown的使用
***
## 简介
  Markdown 是一种轻量级「标记语言」，它用简洁的用「标记」语法，来代替常见的排版格式。
***
## 语法的简要规则
### 标题
如果一段文字被定义为标题，只要在这段文字前加#号，并在#号后加一个空格即可。  

	# 一级标题
	## 二级标题
	### 三级标题
以此类推，总共六级标题。
***
## 列表
列表分为有序列表和无序列表。  
无序列表使用`*`、`+`或`-`来做为列表的标记；有序列表则是使用数字紧接着`.`作为列表的标记。
例如：  
 
	- one
	- two
	- three

被识别为：  

- one
- two
- three
***
### 链接
Markdown支持行内和参考两种形式。  
行内形式为：  `[文本显示的内容](链接)`，例如：  
This is an [example link](http://#/).  
参考形式可以为链接定一个名称，之后在文件的其他地方定义该链接的内容，例如：

	常用的搜索引擎有：[Google][1]、[百度][2]和[Bing][3]。
	[1]: https://www.google.com/
	[2]: https://www.baidu.com/
	[3]: https://cn.bing.com/
这会显示为：  
常用的搜索引擎有： [Google][1]、[百度][2]和[Bing][3]。  

[1]: https://www.google.com/
[2]: https://www.baidu.com/
[3]: https://cn.bing.com/
***
### 图片
图片的语法与链接相似，是在前面添加`!`。  
行内形式为：`![图片标题](图片路径)`；  
参考形式为：`![图片标题][图片id]`，之后在文档的某一处添加：`[图片id]: 图片路径`。 
***
### 代码
在一段文字中，随时可以使用一对反引号来表示代码。  
如果显示多行代码，仅需在每行均缩进4个空格或一个tab即可。
***
### 引用、修辞与强调
文字的引用可以使用`>`来标识。Markdown还支持多级引用，有几级就使用几个`>`即可。  
Markdown支持文字的斜体与粗体。一对处于文字两端的`*`或`_`可以表示斜体；两对处于文字两端的`*`或`_`可以表示粗体。例如：`*斜体*`和`**粗体**`将会显示为：  
*斜体* 和 **粗体**。
***
### 表格
表格的语法比较复杂，例如：
<pre>
	|表头1|表头2|表头3|
	|-|:-:|-:|
	|1|1|1|
	|2|2|2|
</pre>
将显示为：

|表头1|表头2|表头3|
|-|:-:|-:|
|1|1|1|
|2|2|2|

第一行是表头；第二行设置格式并将表头与表内容隔开，其中`-`为左对齐、`:-:`为居中、`-:`为右对齐；第三行起为表项。表的每一列用`|`隔开。
***
## 参考资料
1. riku.[Markdown: Basics （快速入门）](http://wowubuntu.com/markdown/basic.html)  
2. Te_Lee.[Markdown——入门指南](http://www.jianshu.com/p/1e402922ee32)


