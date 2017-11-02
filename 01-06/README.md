# 01-06
## 布局

* 布局-将元素以正确的大小摆放在正确的位置上

## 目录
* [01-06-01](https://github.com/TYRMars/CSSLearn/tree/master/01-06#01-06-01)`display`
* [01-06-02](https://github.com/TYRMars/CSSLearn/tree/master/01-06#01-06-02)`position`
* [01-06-03](https://github.com/TYRMars/CSSLearn/tree/master/01-06#01-06-03)`float`
* [01-06-04](https://github.com/TYRMars/CSSLearn/tree/master/01-06#01-06-04)`flex`
* [01-06-05](https://github.com/TYRMars/CSSLearn/tree/master/01-06#01-06-05)`grid`

## 01-06-01
### display

* [01-06-01-01](https://github.com/TYRMars/CSSLearn/tree/master/01-06#01-06-01-01)`display:block`
* [01-06-01-02](https://github.com/TYRMars/CSSLearn/tree/master/01-06#01-06-01-02)`display:inline`
* [01-06-01-03](https://github.com/TYRMars/CSSLearn/tree/master/01-06#01-06-01-03)`display:inline-block`
* [01-06-01-04](https://github.com/TYRMars/CSSLearn/tree/master/01-06#01-06-01-04)`display:none`

* 设置元素的显示方式
* display: none | inline | block | list-item | inline-list-item | inline-block | inline-table | table | table-cell | table-column | table-column-group | table-footer-group | table-header-group | table-row | table-row-group | flex | inline-flex | grid | inline-grid | run-in | ruby | ruby-base | ruby-text | ruby-base-container | ruby-text-container | contents

```CSS
body{
  display: none;

  display: inline;
  display: block;
  display: contents;
  display: list-item;
  display: inline-block;
  display: inline-table;
  display: table;
  display: table-cell;
  display: table-column;
  display: table-column-group;
  display: table-footer-group;
  display: table-header-group;
  display: table-row;
  display: table-row-group;
  display: flex;
  display: inline-flex;
  display: grid;
  display: inline-grid;
  display: ruby;
  display: ruby-base;
  display: ruby-text;
  display: ruby-base-container;
  display: ruby-text-container;
  display: run-in;

  display: inherit;
  display: initial;
  display: unset;
}
```

## 01-06-01-01
# display:block

<p align="center"><img src="https://github.com/TYRMars/CSSLearn/blob/master/01-06/display/display_block.png" /></p>

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

## 01-06-01-02
# display:inline

<p align="center"><img src="https://github.com/TYRMars/CSSLearn/blob/master/01-06/display/display_inline.png" /></p>

* 默认宽度是内容宽度
* 不可设置宽高度
* 同行显示
* 默认`display:inline`元素
  - span|a|label|cite|em

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
    <span>inline之前的元素</span>
    <span class="sample">display:inline;</span>
    <em>inline之后的元素</em>
  </body>
</html>
```
## 01-06-01-03
# display:inline-block

<p align="center"><img src="https://github.com/TYRMars/CSSLearn/blob/master/01-06/display/display_inline-block.png" /></p>

* 默认宽度为内容宽度
* 可设置宽高
* 同行显示
* 整块换行
* 默认`display:inline`元素
  - input|textarea|select|button

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>dispay inline-block</title>
    <style media="screen">
    .samlpe{background-color:pink}
    .sample{display: inline-block}
    </style>
  </head>
  <body>
    <span>inline-block之前的元素</span>
    <span class="sample"></span>
    <em>inline-block之后的元素</em>
  </body>
</html>
```

# block VS inline VS inline-block

| display | 默认宽度 | 可设置宽高 | 起始位置 |
| :------------- | :------------- | :------------- | :------------- |
| block   | 父级元素宽度  | 是  |  换行 |
|inline   | 内容宽度  | 否  | 同行  |
|inline-block   | 内容宽度  | 是  | 同行 |

## 01-06-01-04
# display:none

<p align="center"><img src="https://github.com/TYRMars/CSSLearn/blob/master/01-06/display/display_none.png" /></p>

* 设置元素不显示
* display:none VS visibility:hidden

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>display none demo</title>
    <style media="screen">
      .parent{margin: 30px;border: 1px solid pink}
      .dn{display: none;}
      .vn{visibility: hidden;}
    </style>
  </head>
  <body>
    <div class="parent">
      <div class="dn">
        display:none
      </div>
    </div>
    <div class="parent">
      <div class="vn">
        visibility:hidden
      </div>
    </div>
  </body>
</html>
```

# 布局-块级元素水平居中

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>布局-块级元素水平居中</title>
    <style media="screen">
    .content{margin:0 auto;}
    .content{width: 300px;height: 300px;background-color: pink}
    </style>
  </head>
  <body>
    <div>
      <div class="content">
        content区域
      </div>
    </div>
  </body>
</html>
```

# 布局-居中导航

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>布局-居中导航</title>
    <style media="screen">
      ul{text-align: center;height: 30px;line-height: 30px;background-color: #f00;}
      li,a{display: inline-block;width: 80px;height: 100%;}
      li{margin: 0 5px;list-style: none;}
      a, a:hover, li.cur a{
        color: #fff;
        text-decoration: none;
      }
      a:hover, li.cur a{
        background-color: #c00;
      }
    </style>
  </head>
  <body>
    <ul class="m-nav">
      <li><a href="#">首页</a></li>
      <li class="cur"><a href="#">页面一</a></li>
      <li><a href="#">页面二</a></li>
      <li><a href="#">页面三</a></li>
      <li><a href="#">页面四</a></li>
    </ul>
  </body>
</html>
```

## 01-06-02
### position 定位

* position - 设置定位方式
* top、right、bottom、left、z-index -设置位置

# top/right/bottom/left

<p align="center"><img src="https://github.com/TYRMars/CSSLearn/blob/master/01-06/position/top_right_bottom_left.png" /></p>

* top是上边缘与参照物的距离
* right是右边缘与参照物的距离
* bottom是下边缘与参照物的距离
* left是左边缘与参照物的距离

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>位置</title>
    <style media="screen">
      .sample{background-color: pink;}
      .sample{position: absolute;}
      .sample{top: 30px;left: 30px;}
    </style>
  </head>
  <body>
    <div class="sample">
      sample
    </div>
  </body>
</html>
```

# z-index

<p align="center"><img src="https://github.com/TYRMars/CSSLearn/blob/master/01-06/position/z-index.png" /></p>

* Z轴上下排序，父级元素相同的情况下，值越大越在上面👆

## z-index 栈

<p align="center"><img src="https://github.com/TYRMars/CSSLearn/blob/master/01-06/position/z-index2.png" /></p>

* Z轴上下排序，不同父级元素相同的情况下，要根据父级情况而定

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>z-index</title>
    <style media="screen">
      .sample0, .sample1{
        position: absolute;
        width: 200px;
        line-height: 150px;
        text-align: center;
      }
      .sample0{
        background-color: #ff0;
      }
      .sample1{
        background-color: pink;
      }
      .sample1{
        top: 100px;
        left: 100px;
      }
      /*
      .container0,.container1{
      position:relative
      }
      .container1{
      z-index:99;
      }
      */
    </style>
  </head>
  <body>
    <div class="container0">
      <div class="sample0">
        sample0
      </div>
    </div>
    <div class="container1">
      <div class="sample1">
        sample1
      </div>
    </div>
  </body>
</html>
```

# position:relative
## 相对定位

<p align="center"><img src="https://github.com/TYRMars/CSSLearn/blob/master/01-06/position/position_absolute_relative.png" /></p>

<p align="center"><img src="https://github.com/TYRMars/CSSLearn/blob/master/01-06/position/position_relative2.png" /></p>

* 仍在文档流中
* 参照物为元素本身

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>相对定位</title>
    <style media="screen">
      .container{
        width: 400px;
        line-height: 2;
        border: 1px dashed #aaa;
      }
      .sample{
        background-color: pink;
        position: relative;
        top: 20px;
        left: -30px;
      }
    </style>
  </head>
  <body>
    <div class="container">
      <div>相对定位元素的前序元素</div>
      <div class="sample">
        sample
      </div>
      <div>相对定位元素的后序元素</div>
    </div>
  </body>
</html>
```

* 使用场景：绝对定位元素的参照物

# position:absolute
## 绝对定位


<p align="center"><img src="https://github.com/TYRMars/CSSLearn/blob/master/01-06/position/position_absolute_relative.png" /></p>

<p align="center"><img src="https://github.com/TYRMars/CSSLearn/blob/master/01-06/position/position_absolute2.png" /></p>

<p align="center"><img src="https://github.com/TYRMars/CSSLearn/blob/master/01-06/position/position_absolute3.png" /></p>

* 默认宽度为内容宽度
* 默认脱离文档流
* 参照物为第一个定位祖先/根元素

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>绝对定位</title>
    <style media="screen">
    .container{
      width: 400px;
      margin: 200px;
      line-height: 2;
      border: 1px dashed #aaa;
    }
    .sample{
      background-color: pink;
    }
    .sample{
      position: absolute;
    }
    /*.sample{
      bottom: 10px;
      left: -30px;
    }
    .container{
      position: relative;
    }*/
    </style>
  </head>
  <body>
    <div class="container">
      <div>绝对定位元素的前序元素</div>
      <div class="sample">
        sample
      </div>
      <div>绝对定位元素的后序元素</div>
    </div>
  </body>
</html>
```

## 绝对定位应用场景

* 轮播头图

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>轮播头图</title>
    <style media="screen">
      .is{
        position: relative;
        width: 480px;
      }
      .is img{
        display: block;
      }
      .is .title{
        position: absolute;
        bottom: 0;
        margin: 0;
        width: 100%;
        line-height: 45px;
        background-color: #000;
        opacity: 0.7;
      }
      .is .title a{
        margin-left: 20px;
        color: #fff;
        text-decoration: none;
      }
      .is .controls{
        position: absolute;
        bottom: 18px;
        right: 10px;
        line-height: 10px;
      }
      .is .controls span{
        display: inline-block;
        width: 10px;
        margin: auto 1px;
        height: 10px;
        border-radius: 10px;
        background-color: gray;
      }
      .is .controls span.cur{
        background-color: #fff;
      }
    </style>
  </head>
  <body>
    <div class="is">
      <img src="./time1.jpg" alt="img">
      <p class="title">
        <a href="#">Mac stay hungry stay foolish</a>
      </p>
      <div class="controls">
        <span></span>
        <span class="cur"></span>
        <span></span>
        <span></span>
        <span></span>
      </div>
    </div>
  </body>
</html>
```

# position:fixed
## 固定定位

<p align="center"><img src="https://github.com/TYRMars/CSSLearn/blob/master/01-06/position/position_fixed.png" /></p>

<p align="center"><img src="https://github.com/TYRMars/CSSLearn/blob/master/01-06/position/position_fixed2.png" /></p>


* 默认宽度为内容宽度
* 脱离文档流
* 参照物为视窗

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>fixed定位</title>
    <style media="screen">
      .container{
        width: 400px;
        margin: 200px;
        line-height: 2;
        border: 1px dashed #aaa;
      }
      .sample{
        background-color: pink;
      }
      .sample{
        position: fixed;
      }
      .sample{
        bottom: 0;
        left: 10px;
      }
      .container{
        height: 1000px;
      }
    </style>
  </head>
  <body>
    <div class="container">
        <div>----------------</div>
        <div class="sample">
          sample
        </div>
        <div>----------------</div>
    </div>
  </body>
</html>
```

## 固定定位应用场景

* 布局-固定顶栏

```html
<!DOCTYPE html>
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>固定顶栏</title>
    <style media="screen">
      body{
        margin: 0;
        line-height: 1.8;
      }
      .top{
        background-color: pink;
        color: #fff;
      }
      .main{
        height: 3000px;
        background-color: #eee;
      }
      body{
        padding-top: 50px;
      }
      .top{
        position: fixed;
        top: 0px;
        width: 100%;
        height: 50px;
      }
    </style>
  </head>
  <body>
    <div class="top">
      top bar
    </div>
    <div class="main">
      main content area
    </div>
  </body>
</html>
```

* 布局-遮罩

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>遮罩</title>
    <style media="screen">
      .mask{
        position: fixed;
        top: 0;
        left: 0;
        z-index: 999;
        width: 100%;
        height: 100%;
        background-color: #000;
        opacity: 0.3;
      }
      .content{
        height: 3000px;
      }
    </style>
  </head>
  <body>
    <div class="mask">

    </div>
    <div class="content">
      content area
    </div>
  </body>
</html>
```

* 布局-三行中间自适应布局

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>三行自适应布局布局</title>
    <style media="screen">
      .head{
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100px;
        background-color: #ccc;
      }
      .body{
        position: absolute;
        top: 100px;
        left: 0;
        bottom: 100px;
        right: 0;
        overflow: auto;
      }
      .content{
        height: 2000px;
      }
      .foot{
        position: absolute;
        bottom: 0;
        left: 0;
        width: 100%;
        height: 100px;
        background-color: #ccc;
      }
    </style>
  </head>
  <body>
    <div class="head">
      head
    </div>
    <div class="content">
      content area
    </div>
    <div class="foot">
      foot
    </div>
  </body>
</html>
```
## 01-06-03
# float

<p align="center"><img src="https://github.com/TYRMars/CSSLearn/blob/master/01-06/float/float.png" /></p>

<<<<<<< HEAD


## 01-06-04

* 元素为`flex container`flex容器
* `flex item`弹性元素
* `main axis `主轴
* `cross axis`副轴

### 创建flex container

* `display:flex`
* `flex item`
  - 只有在文档流中的子元素是flex item

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>flex</title>
  </head>
  <body>
    <div style="display:flex">
      <div>block</div>
      <div style="flout:left;">float</div>
      <span>inline</span>
      <div style="position:absolute;"></div>
      <div>
        <div>grandson</div>
      </div>
    </div>
  </body>
</html>
```

# flex

* 方向
* 弹性
* 对齐

## 方向

| flex-direction | 弹性方向 |
| :------------- | :------------- |
| flex-warp  | 弹性换行    |
| flex-flow   | 弹性的流  |
| order  | 弹性的顺序  |
=======
* float:left|right|none
* 默认宽度为内容宽度
* 脱离文档流
* 向指定方向一直移动

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>float</title>
    <style>
        div{line-height: 50px;}
        .sample{
            background-color: yellow;
            float:left;
        }
        .sb0{background-color: red}
        .sb1{background-color: blue}
        .div1{background-color: yellow;
            float:left;}
        .div2{background-color: red;
            float:left;}
        .div3{background-color: blue;}
    </style>
</head>
<body>
<div class="sb0">&nbsp;</div>
<div class="sample">sample</div>
<div class="sb1">&nbsp;</div>
<HR>
<div class="divs">
    <div class="div1">123</div>
    <div class="div2">123</div>
    <div class="div3">123</div>
</div>
<div style="clear: both"></div>
<HR>
</body>
</html>
```

* float元素半脱离文档流

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>float</title>
    <style>
        div{line-height: 50px;}
        .sample{
            background-color: yellow;
            float:left;
        }
        .sb0{background-color: red}
        .sb1{background-color: blue}
        .div1{background-color: yellow;
            float:left;}
        .div2{background-color: red;
            float:left;}
        .div3{background-color: blue;}
    </style>
</head>
<body>
<div class="sb0">&nbsp;</div>
<div class="sample">sample</div>
<div class="sb1">&nbsp;</div>
<HR>
<div class="divs">
    <div class="div1">123</div>
    <div class="div2">123</div>
    <div class="div3">123</div>
</div>
<div style="clear: both"></div>
<HR>

</body>
</html>
```
>>>>>>> 62b81632133c2373069bdd4f42ef832dafc6de54
