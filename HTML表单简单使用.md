# HTML表单的简单使用

## HTML `<form>`标签
在HTML中，我们可以使用`<form>`标签创建一个表单，如下所示：  

    <form action="xxx" method="get">
    </form>
在`<form>`标签中,常用属性如下所示：  

|属性|值|描述|
|:-:|:-:|:-:|
|action|URL|规定当提交表单时向何处发送表单数据|
|autocomplete|on/off|是否启用表单的自动完成功能，仅HTML 5|
|method|get/post|规定用于发送表单数据的方法|
|name|名称|规定表单的名称|  

表单能够包含的元素中，常用到input和label 元素，下面分别它们的使用方法。  
**仅有被`<form>`标签包裹元素中采集的数据才会被提交，标签外的数据不会被提交。**

## `<label>`标签的使用
- `<label>`标签为input元素定义标注（标记）。  
- label元素不会向用户呈现任何特殊效果。不过，它为鼠标用户改进了可用性。如果在 label 元素内点击文本，就会触发此控件。就是说，当用户选择该标签时，浏览器就会自动将焦点转到和标签相关的表单控件上。  
- 为了完成上述动作，`<label>`标签的 for 属性应当与相关元素的 id 属性相同。
- HTML 5中，该标签新增了form属性，规定 label所属的一个或多个表单。form属性的值必须是其所属的表单的 id。如需引用一个以上的表单，请使用空格分隔的列表。  

使用示例：  
```
<form action="#" method="get" id="genderform">
<label>Male
<input type="radio" name="sex" id="male" value="male" />
</label>
<label>Female
<input type="radio" name="sex" id="female" value="female"  />
</label>
</form>
<p>下面有一个用于第一个单选按钮的 label 位于 form 元素之外，但仍然是表单的一部分。</p>
<label for="male" form="nameform">Male</label>
```

## `<input>`标签的使用
`<input>`标签用于搜集用户信息,根据不同的 type 属性值，输入字段拥有很多种形式。
### text
`<input type="text" />` 定义用户可输入文本的单行输入字段。  
### button
`<input type="button" />` 定义可点击的按钮，但没有任何行为。button 类型常用于在用户点击按钮时启动 JavaScript 程序。  
### checkbox
`<input type="checkbox" />` 定义复选框。复选框允许用户在一定数目的选择中选取一个或多个选项。
### file
`<input type="file" /> `用于文件上传。  
### hidden
`<input type="hidden" />` 定义隐藏字段。隐藏字段对于用户是不可见的。隐藏字段通常会存储一个默认值，它们的值也可以由 JavaScript 进行修改。
### image
`<input type="image" />` 定义图像形式的提交按钮。  
### password
`<input type="password" />` 定义密码字段。密码字段中的字符会被掩码（显示为星号或原点）。
### radio
`<input type="radio" />` 定义单选按钮。单选按钮允许用户在一个分组中选取一个选项,它的分组是根据name属性进行的。  
### reset
`<input type="reset" />` 定义重置按钮。重置按钮会清除表单中的所有数据。  
### submit
- `<input type="submit" />` 定义提交按钮。提交按钮用于向服务器发送表单数据。数据会发送到表单的 action 属性中指定的页面。
- `<input>`标签在HTML 5中还具有formaction属性，用于覆盖form元素的action属性。该属性适用于 type="submit" 以及 type="image"。
***
表单中还有一些常会用到的标签，下面进行介绍。
## `<textarea>`标签
`<textarea>` 标签定义多行的文本输入控件,文本区中可容纳无限数量的文本，可以使用以下代码实现：`<textarea> </textarea>`  

## `<select>`标签
`<select>标签`可创建单选或多选菜单。`<select>标签`包裹的`<option>`标签用于定义列表中的可用选项。例如：  
```
<select>
  <option value ="apple">苹果</option>
  <option value ="banana">香蕉</option>
</select>
```   
## `<fieldset>`标签  
- `<fieldset>` 标签将表单内容的一部分打包，生成一组相关表单的字段。当一组表单元素放到`<fieldset>`标签内时，浏览器会以特殊方式来显示它们。  
- `<fieldset>` 标签没有必需的或唯一的属性，`<legend>` 标签为 fieldset 元素定义标题。
```  
<fieldset>
    <legend>健康信息</legend>
    身高：<input type="text" />
    体重：<input type="text" />
  </fieldset>  
```
## HTML 表单示例

