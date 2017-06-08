在Safari浏览器中如果想对select控件进行高度设置，最常用的方法是下面几个：
- ```-webkit-appearance: menulist-button;```
- ```-webkit-appearance: none;```
- 设置```border```
- 设置```background```

如果从设计思想出发的话，这个并不算是bug，控件是由引擎来实现行为和逻辑，再由主题API来进行绘制完成(mac上的主题是Aqua)。外观样式通过-webkit-appearance进行控制，如果不需要默认的外观，只需要将-webkit-appearance设置为none，然后就可以在上面为所欲为了😏。

想要删除select元素上的Aqua样式，设置-webkit-appearance只是其中的一种，另外两种分别是：
- 指定元素的边框```border```
- 指定元素的背景```background```

通过上面任意一种方式去除select元素的Aqua样式后，我们就可以通过属性修改：
- ```font-family```
- ```font-size```
- ```height```和```line-height```
- ```padding``` (只有修改-webkit-appearance才可以设置)

> 资料来源于 [Permanent Link: Design Friendly Select Elements in Safari 3](http://particletree.com/notebook/design-friendly-select-elements-in-safari-3/)，通过实验并对其中部分进行了修改。