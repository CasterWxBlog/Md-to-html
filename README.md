# Md-to-html

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
