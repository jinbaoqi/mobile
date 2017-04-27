## ios tap highlight issue
```css
*{
    -webkit-tap-highlight-color:rgba(0,0,0,0);
    -webkit-tap-highlight-color:transparent;
}
```
## ios/andoid when overflow animation will disappear
```css
*{
    -webkit-overflow-scrolling:touch;
}
```

## css reset
```css
html{
    -webkit-tap-highlight-color:rgba(0,0,0,0);
    -webkit-user-modify:read-write-plaintext-only;
    -webkit-user-select:none;
}
*,
*:before,
*:after{
    box-sizing:border-box;
}
input,textarea,select{
    -webkit-appearance:none;/*去掉webkit默认的表单样式*/
    appearance:none;
    outline:none;
    border:none;
}
```

## font setting
```css
body{
    font-family:"Helvetica Neue", Helvetica, STHeiTi, sans-serif;
    /*
    ios 4.0+ Helvetica Neue
    ios 4.0- Helvetica
    chinese STHeiTi
    */
}
```

## :active 效果不兼容
在安卓4.0以下版本：active为状态无法兼容，需要给该元素绑定touch事件
```javascript
var ele = document.getElementById('btnShare')
ele.addEventListener('touchstart',function(){})
```
