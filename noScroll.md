# 禁止页面滚动
1. js控制页面禁止滚动。

```
禁止页面滚动
function addListener(){
    $('body').on('touchmove',function(e){
        e = e || window.e;
        e.preventDefault();
        e.stopPropagation();
    })
 }
解除页面禁止滚动效果
function removeListener(){
    $('body').off('touchmove');
}
```
2. css控制页面禁止滚动。
```
body的禁用滚动
.noscroll{
  position: fixed;
  overflow-y: hidden;
  width: 100%;
}
```