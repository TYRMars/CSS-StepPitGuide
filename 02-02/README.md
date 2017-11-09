# 02-02
## 多列布局

* [02-02-01](https://github.com/TYRMars/CSSLearn/tree/master/02-02#02-02-01) `定宽与自适应`
* [02-02-02](https://github.com/TYRMars/CSSLearn/tree/master/02-02#02-02-02) `不定宽与自适应`
* [02-02-03](https://github.com/TYRMars/CSSLearn/tree/master/02-02#02-02-03) `等分`
* [02-02-04](https://github.com/TYRMars/CSSLearn/tree/master/02-02#02-02-04) `等高`

# 02-02-01
## 定宽与自适应

* float+margin

### float+margin

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title></title>
    <style>
    .left{
        float: left;
        width: 100px;
    }
    .right{
        margin-left: 120px;
    }
    </style>
  </head>
  <body>
    <div class="parent">
        <div class="left">
            <p>left</p>
        </div>
        <div class="right">
            <p>right</p>
            <p>right</p>
        </div>
    </div>
  </body>
</html>
```
