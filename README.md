# Md-to-html

## 赞助

| 支付宝 | 微信 |
| ------------ | ------------ | 
| <img width="250" src="https://www.cnblogs.com/images/cnblogs_com/LexMoon/1246510/o_pay.png"/> |<img width="250" src="https://www.cnblogs.com/images/cnblogs_com/LexMoon/1246510/o_wx.png"/> |

所有项目都是完全开源的，使用完全免费。 但是随着项目规模的增长，也需要有相应的资金支持才能持续项目的维护与开发。你可以通过下列的方法来赞助开发。你的名字会出现在我的GitHub 仓库和博客文档中。


### 对markdown格式文档进行转换。

>   markdown -> html

### 第一步,引入showdown.js

```
    <script src="markdown/dist/showdown.js"></script>
```

### 第二步，转换方法

```
<script type="text/javascript">
    $(function () {
        var converter = new showdown.Converter(),
            text = "## Markdown文档",
            html = converter.makeHtml(text);
</script>

```
这里html的返回值就是转换之后的html格式了。

### 第三步，嵌入html
html中
```html
<div id="result">
</div>
```
js中
```
    document.getElementById("result").innerHTML = html;
```

### 效果

![mdtohtml](https://www.cnblogs.com/images/cnblogs_com/LexMoon/1246510/o_mark.jpg)
