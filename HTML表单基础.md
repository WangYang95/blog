# HTML表单基础

### form表单有什么作用？有哪些常用的input 标签，分别有什么作用？
- `<form>`标签用于为用户输入创建 HTML 表单。表单能够包含input 元素，还可以包含 menus、textarea、fieldset、legend 和 label 元素。
**表单用于向服务器传输数据（数据采集）**。  
- `<input>`标签用于搜集用户信息。根据不同的 type 属性值，输入字段拥有很多种形式。输入字段可以是文本字段、复选框、单选按钮、按钮等等。其常用属性如下：  

  |属性|值|描述|
  |:-:|:-:|:-:|
  |accept|文件类型|file类型合用，规定提交文件的类型|
  |alt|文字|image类型合用，图像输入替代的文本|
  |autocomplete|on/off|是否使用输入字段的自动完成功能|
  |autofocus|autofocus|页面加载时是否获得焦点（不适用于隐藏域）|
  |checked|checked|此input元素首次加载时应当被选中|
  |disabled|disabled|input 元素加载时禁用此元素|
  |name|名称|定义 input 元素的名称|
  |pattern|正则表达式|规定输入字段的值的模式或格式|
  |placeholder|文字|帮助用户填写输入字段的提示|
  |readonly|readonly|只读|
  |required|required|指示输入字段的值是必需的|
  |src|URL|以提交按钮形式显示的图像的 URL|
  |type|类型|input 元素的类型|
  |value|值|规定 input 元素的值|
  
  关于type属性的说明如下所示：  
  
  |type的值|说明|
  |:-:|:-:|
  |button|按钮|
  |checkbox|复选框|
  |file|文件上传|
  |hidden|隐藏域|
  |image|图片形式的提交按钮|
  |password|密码域|
  |radio|单选框|
  |reset|重置按钮|
  |submit|提交按钮|
  |text|文本域|

### POST和GET方式的区别？
GET和POST是两种常用的HTTP请求方式，GET方式从指定的资源请求数据；POST方式向指定的资源提交要被处理的数据。两者对比如下表所示：  

|项目|GET|POST|备注|
|:-:|:-:|:-:|:-:|
|后退按钮/刷新|无害|数据会被重新提交（浏览器应该告知用户数据会被重新提交）||
|书签|可收藏为书签|不可收藏为书签||
|缓存|能被缓存|不能缓存||
|编码类型|application/x-www-form-urlencoded|application/x-www-form-urlencoded 或 multipart/form-data||
|历史|参数保留在浏览器历史中|参数不会保存在浏览器历史中||
|对数据长度的限制|受限制|无限制|HTTP协议并没有对数据长度进行限制，而是浏览器和一些服务器对URL长度进行了限制。GET请求将参数放置于URL中，因此受限|
|对数据类型的限制|只允许 ASCII 字符|没有限制||
|安全性|与POST相比，安全性较差|比GET安全|由历史和可见性可以得到此条结论，使用POST方式不能轻易改为GET方式。**但是，传输敏感数据时仍需使用密文、HTTPS等措施。**|
|可见性|数据在URL中对所有人可见|数据不会显示在URL中||

- 使用GET方式：交互更像是一个问题（即它是一个安全的操作，如查询，读取操作或查找）。例如我们刷微博时查看时间线上的内容。  
- 使用POST方式：交互更像一个订单、交互以用户将感知到的方式（例如，订阅服务）来改变资源的状态、或者用户对交互的结果负责。例如，我们从淘宝下一个订单、发送微博或在微博上点赞等等。

>参考资料：  
>1. [URIs, Addressability, and the use of HTTP GET and POST](https://www.w3.org/2001/tag/doc/whenToUseGet.html)  
>2. [HTTP 方法：GET 对比 POST](http://www.w3school.com.cn/tags/html_ref_httpmethods.asp)  

### 在input里，name有什么作用？
- name 属性规定 input 元素的名称。  

- name 属性用于对提交到服务器后的表单数据进行标识，或者在客户端通过 JavaScript 引用表单数据。  

- 只有设置了 name 属性的表单元素才能在提交表单时传递它们的值。

### radio如何分组?
radio根据input中的name属性进行分组。

### placeholder属性有什么作用?
- placeholder属性提供可描述输入字段预期值的提示信息。
- 该提示会在输入字段为空时显示，并会在字段获得焦点时消失。
- placeholder 属性适用于以下的 `<input>` 类型：text, search, url, telephone, email 以及 password。
- placeholder 属性是 HTML5 中的新属性。

### type=hidden隐藏域有什么作用? 举例说明。
- type=hidden定义隐藏的输入字段。隐藏字段对于用户是不可见的。隐藏字段通常会存储一个默认值，它们的值也可以由 JavaScript 进行修改。例如：  
  - 可以储存临时值供表单访问；
  - 储存key供服务器校验用户信息；
  - 更新条目时，储存id供更新使用。 








