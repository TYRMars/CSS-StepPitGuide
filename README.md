<h1 align="center">CSS学习</h1>
<p align="center"><img src="http://upload.chinaz.com/2014/0915/1410772362627.jpg" /></p>

---

# 目录
## 第一章 CSS基本知识

* [01-01](https://github.com/TYRMars/CSSdisplay#01-01) `CSS介绍`

## 第二章 CSS布局

* [02-01](https://github.com/TYRMars/CSSdisplay#02-01) `CSS布局`
* [02-02](https://github.com/TYRMars/CSSdisplay#02-02) `display`
* [02-03](https://github.com/TYRMars/CSSdisplay#02-03) `position`
* [02-04](https://github.com/TYRMars/CSSdisplay#02-04) `float`
* [02-05](https://github.com/TYRMars/CSSdisplay#02-05) `常用布局`

---

## 02-01
### CSS布局
* display(水平居中、居中导航)
* position(轮播头图、遮罩、三行自适应性布局)
* float(float),flex(三行两列自适应)

## 02-02
### display
* 设置元素显示方式
* display:block/inline/inline-block/none

### display:block
* 默认宽度为父元素宽度
* 可设置宽高
* 换行显示

## 02-03
### position
* position:static/relative/absolute/fixed/grid
* 默认为static静止

### position:relative
* 相对定位

### postion:absolute
* 绝对定位

## 02-04
### float

## 02-05
### 常用布局

#### 布局方案-剧中布局

##### 水平居中布局

* inline-block + text-align

```CSS
/*与内容同宽*/
.parent{
  text-align: center;
}
.child{
  display: inline-block;
}
```

* table+margin


---

## 日常总结
* 元素的居中利用`position:absolute`
```CSS
.style{
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  margin: auto;
}
```
