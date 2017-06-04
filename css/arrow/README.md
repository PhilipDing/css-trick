## CSS3箭头

#### 90°直角箭头
原理： 看做只有两个边框的元素，再旋转45°
![](./arrow-90.png)

``` css
.arrow-90 {
    width: 20px;
    height: 20px;
    border-top: 2px solid #000;
    border-right: 2px solid #000;
    transform: rotate(45deg);
}
```

### 非90°箭头
在90°箭头的基础上，利用skew在X轴或者Y轴进行扭曲变形。
``` css
.arrow {
    width: 20px;
    height: 20px;
    border-top: 2px solid #000;
    border-right: 2px solid #000;
    transform: rotate(55deg) skewX(30deg);
}
```

![](./show.png)