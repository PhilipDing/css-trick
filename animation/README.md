## Animation

animation可以使一个CSS样式转换成另一个CSS样式。

动画由两部分组成：
1. 描述动画的样式规则 (animation)
2. 用于指定动画的开始、结束及中间点样式的关键帧 (@keyframes)

使用CSS动画的优点：
1. 创建起来比较简单，不需要了解任何的JavaScript的知识。
2. 运行效果较好，甚至是在低性能的系统上。渲染引擎会使用跳帧或者其他技术保证动画表现尽可能的流畅。
3. 让浏览器控制动画序列，允许浏览器优化性能和效果，如降低位于隐藏选项卡中的动画更新频率。

### 配置动画
使用```animation```属性配置动画时间、时长以及一些其他的动画细节，但该属性不能配置动画的实际表现，动画的实际表现由```@keyframes```规则实现。

通过使用```@keyframes```建立两个或两个以上关键帧来配置动画的实际表现，每一个关键帧都描述了动画元素在给定的时间上应该如何渲染。

关键帧使用percentage来指定动画发生的时间点，0%(from)表示动画第一时刻，100%(to)表示动画最终时刻。

### 语法
``` css
animation: name duration timing-function delay iteration-count direction.
```
默认值: ``` none 0 ease 0 1 normal ```

值 | 描述
--  | --
animation-name | 规定需要绑定到选择器的 keyframe 名称。
animation-duration | 规定完成动画所花费的时间，以秒或毫秒计。
animation-timing-function | 规定动画的速度曲线。
animation-delay | 规定在动画开始之前的延迟。
animation-iteration-count | 规定动画应该播放的次数。(n或infinite)
animation-direction | 规定是否应该轮流反向播放动画。
animation-fill-mode | 指定动画执行前后如何为目标元素应用样式。
animation-play-state |

### 资源
* [深入理解CSS3 Animation 帧动画](http://www.cnblogs.com/aaronjs/p/4642015.html "animation-timing-fucntion steps")

* [MDN](https://developer.mozilla.org/zh-CN/docs/Web/CSS/CSS_Animations)