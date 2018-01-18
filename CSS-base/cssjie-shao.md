# CSS基础介绍

* CSS通过将规则与HTML元素相关联的方式来工作。这些规则用来控制指定元素中的内容如何显示。
* 一条CSS规则包含两个部分：一个选择器和一条声明。

```CSS
p{font-family: Arial;}
```
## 01-01-01
### 使用外部CSS

## `<link>`

* 在HTML文档中，`<link>`元素可用来告诉浏览器在何处寻找用于定义页面样式的CSS文件。它是一个空元素（也就是说它不需要结束标签），而且位于`<head>`元素中。
* 它应该使用以下三个特性：

#### `href`

* 该特性表示CSS文件的路径（通常位于CSS或styles文件夹中）。

#### `type`

* 该特性表明页面所链接文档的类型。它的值是`text/css`。

#### `rel`

* 该特性表明HTML页面与被链接文件的关系。当链接到一个`CSS`文件时，该特性的值应该为`stylesheet`。

## HTML

```HTML
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title></title>
    <link href="css/styles.css" type="text/css" rel="stylesheet"/>
  </head>
  <body>
    <h1>这是 H1</h1>
  </body>
</html>
```

## CSS `styles.css`

```CSS
body{
  font-family: arial;
  background-color: rgb(185, 179, 175);
}
h1{
  color: rgb(255, 255, 255);
}
```

### 使用内部CSS

# `<style>`

* 还可以在HTML页面添加CSS规则，这时需要将规则写在`<style>`元素内，`<style>`元素通常位于页面的`<head>`元素中。
* `<style>`元素应该使用`type`特性来表明这些演示实在CSS中
