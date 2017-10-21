# 01-06
## 布局

* 布局-将元素以正确的大小摆放在正确的位置上

## 目录
* [01-06-01]()

## 01-06-01
### display

* 设置元素的显示方式
* display: none | inline | block | list-item | inline-list-item | inline-block | inline-table | table | table-cell | table-column | table-column-group | table-footer-group | table-header-group | table-row | table-row-group | flex | inline-flex | grid | inline-grid | run-in | ruby | ruby-base | ruby-text | ruby-base-container | ruby-text-container | contents

```CSS
body{
  display: none

  display: inline
  display: block
  display: contents
  display: list-item
  display: inline-block
  display: inline-table
  display: table
  display: table-cell
  display: table-column
  display: table-column-group
  display: table-footer-group
  display: table-header-group
  display: table-row
  display: table-row-group
  display: flex
  display: inline-flex
  display: grid
  display: inline-grid
  display: ruby
  display: ruby-base
  display: ruby-text
  display: ruby-base-container
  display: ruby-text-container
  display: run-in

  display: inherit
  display: initial
  display: unset
}
```

# display:block

<p align="center"><img src="http://pic2.orsoon.com/2016/1108/20161108044419740.png" /></p>

* 块级元素
* 默认宽度为父元素宽度
* 可设置宽高
* 换行显示
* 默认`display:block`元素
  - div|p|h1-h6|ul|form ...

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>display block demo</title>
    <style media="screen">
      .sample{background-color: pink}
      .sample{width: 200px;height: 200px;}
    </style>
  </head>
  <body>
    <span>block之前的元素</span>
    <div class="sample">
      display:block;
    </div>
    <span>block之后的元素</span>
  </body>
</html>
```

# display:inline

<p align="center"><img src="http://pic2.orsoon.com/2016/1108/20161108044419740.png" /></p>

* 默认宽度是内容宽度
* 不可设置宽高度
* 同行显示

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>display inline demo</title>
    <style>
    .sample{background-color: pink}
    /*.sample{width: 200px;height: 200px}*/
    em{display: block;}
    </style>
  </head>
  <body>
    <span>inline之的元素</span>
    <span class="sample">display:inline;</span>
    <em>inline之后的元素</em>
  </body>
</html>
```
