# 01-04
## CSS盒模型

## 目录
* [01-04-01](https://github.com/TYRMars/CSSLearn/tree/master/01-04#01-04-01)`CSS盒模型基本特征`
* [01-04-02](https://github.com/TYRMars/CSSLearn/tree/master/01-04#01-04-02)``
* [01-04-03](https://github.com/TYRMars/CSSLearn/tree/master/01-04#01-04-03)``


## 01-04-01
### CSS盒模型的特征

* `box-sizing:content-box;`标准盒模型
* `box-sizing:border-box;`IE盒模型

### 基本属性

* content = width * height
* padding
* border
* margin

## width

* `width:<length>|<percentage>|auto|inherit`
* 只对块级元素设置宽度
* `max-width,min-width`

## heigth

* `height:<length>|<percentage>|auto|inherit`
* 只对块级元素设置宽度
* `max-height,min-height`

---

### JS设置盒模型宽高
* `dom.style.width/height`
* `dom.currentStyle.width/height`(only IE)
* `window.getComputedStyle(dom).width/height`
* `dom.getBoundingClientRect().width/height`(根据视窗view的左顶点，对元素位置进行判断)

---

## padding

* `padding:[<length>|<percentage>]{1,4}|inherit`

### top_right_bottom_left

* 顺时针方向设置
* `-----------------------`
* padding: 40px 30px 20px 10px;
* ||
* padding-top: 40px;
* padding-right: 30px;
* padding-bottom: 20px;
* padding-left: 10px;
* `-----------------------`
* padding:20px; == padding: 20px 20px 20px 20px;
* padding:20px 10px; == padding: 20px 10px 20px 10px;
* padding:20px 10px 30px; == padding: 20px 10px 30px 10px;
* `-----------------------`

## margin

* `margin:[<length>|<percentage>]{1,4}|auto|inherit`

# 水平居中

* `margin: 0 auto`
* 要设置元素宽高

## border

* `border:[<border-width>]||<boder-style>||<border-color>]|inherit`
* `border-width:[<length>|thin|medium|thick]{1,4}|inherit`
* `border-style:[solid|dashed|dotted|...]{1,4}|inherit`
* `border-color:[<color>|transparent]{1,4}|inherit`

### border-radius



## overflow

* overflow:visible|hidden|scroll|auto
