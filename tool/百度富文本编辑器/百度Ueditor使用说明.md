

1.在页面中引入ueditor插件



```javascript
<!--引入富文本编辑器的3个js文件-->
  <script type="text/javascript" src="../static/assets/vendors/ueditor/ueditor.config.js"></script>
  <script type="text/javascript" src="../static/assets/vendors/ueditor/ueditor.all.min.js"> </script>
  <script type="text/javascript" src="../static/assets/vendors/ueditor/lang/zh-cn/zh-cn.js"></script>
```
2.`在表单的textarea中设置`id属性

```html
<textarea id="content"  name="content" placeholder="内容"></textarea>
```



3.在页面中写入如下js代码

```javascript
<script>
var ue = UE.getEditor('content',{ toolbars: [[
            'fullscreen', 'source', '|', 'undo', 'redo', '|',
            'bold', 'italic', 'underline', 'fontborder', 'strikethrough', 'superscript', 'subscript', 'removeformat', 'formatmatch', 'autotypeset', 'blockquote', 'pasteplain', '|', 'forecolor', 'backcolor', 'insertorderedlist', 'insertunorderedlist', 'selectall', 'cleardoc', '|',
            'rowspacingtop', 'rowspacingbottom', 'lineheight', '|',
            'customstyle', 'paragraph', 'fontfamily', 'fontsize', '|',
            'directionalityltr', 'directionalityrtl', 'indent', '|',
            'justifyleft', 'justifycenter', 'justifyright', 'justifyjustify', '|', 'touppercase', 'tolowercase', '|',
            'link', 'unlink', 'anchor', '|', 'imagenone', 'imageleft', 'imageright', 'imagecenter', '|',
            'simpleupload', 'insertimage', 'emotion', 'scrawl', 'insertvideo', 'music', 'attachment', 'map', 'gmap', 'insertframe', 'insertcode', 'webapp', 'pagebreak', 'template', 'background', '|',
            'horizontal'
        ]] });
</script>
```



