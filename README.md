# html-css
这是关于html与css脚本的练习仓库

## 网页的要素
网页分为三个要素，分别是：

结构（html）

表现（css）-> 层叠样式

行为（javascript）
## 属性
一般的写在尖括号里面的关键字标签被称作属性，他们控制了标签在网页中的表现形式

### 标识符：`id=""`

## 块
<code>
    在这之间的元素可以是文本也可以是下级标签
</code>



# css
## css设置标签风格
`<style>`标签内部有这与`html`不同的编写规则

1.在标签内部使用style来设置：css代码使用名值对来设置对象属性，如：`style="color: VALUE;"`，其中`color`是名，`VALUE`是值

2.编写在`<head>`标签中的`style`属性中，同时要在`<head>`标签内部写css样式选择器`<style>  </style>`；通过css选择器选中相应标签类型的所有对象并对其设置样式

3.外部样式引进：在外部创建一个css文件，并在文件中设置好样式代码，然后通过`<link rel="stylesheet" href="ADDRESS">`将代码关联到`html`文件中
## 内联样式：
直接在标签内设置好的样式，只能对一个标签生效的样式是内联样式


## css基本语法

1.选择器 `标签标识符`

多选相同标签

    Type{
        /*  */
    }
`id`选中特定标签:有时只能同时给一个元素添加样式

    #idName{
        /*  */
    }
`class`更改特定的自定义种类的标签，可以重复使用，也可以对一个标签对象指定多个`class`

`CSS`

    <style> 
    Type.class{
        /*  */
    }
    </style>
`HTML`

    <Type class="someClass"> </Type>
通配选择器:可以选择所有的标签

    *{
        /*  */
    }
交集选择器：交集选择器中如果含有元素选择器，则必须写元素选择器

    Type.class1.class2...{
        /* code */
    }
并集选择器（选择器分组）：同时选择多个标签类型的元素，并对其设置样式

    Type1,Type2...{
        /* code */
    }


2.声明块 `{ 名值对 }`

## 标签之间的关系
1.父子

    直接被父元素包含的元素叫做子元素

2.祖先与后代

    祖先元素：直接或者间接包含后代元素的元素叫做祖先元素
    后代元素：被祖先元素直接或者间接被祖先元素包含的元素

3.兄弟元素

    拥有相同父元素的元素叫做兄弟元素
## 关系选择器
1.子元素选择器

    fatherType > childType...{

    }
2.后代元素选择器

    fatherType childrenTypes{

    }
3.兄弟元素选择器

    Type1 + Type2 ...{
        
    } 
