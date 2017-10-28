# scss skills
## 设备像素密度测试，不同手机不同数值
[http://www.gbtags.com/gb/share/5307.htm](http://www.gbtags.com/gb/share/5307.htm)
```
@media (-webkit-min-device-pixel-ratio: 2) {
  body:before {
    line-height: 2.025em;
  }
}
```

---

## 添加一个闪光效果
```
@include keyframes('overlay-hide') {
  0% {
    opacity: 1;
    z-index: 100000;
  }
  15% {
    opacity: 1;
    z-index: 100000;
  }
  99% {
    opacity: 0;
    z-index: 100000;
  }
  100% {
    opacity: 0;
    z-index: -1;
  }
}

body {
  &:after {
    @include vendor('animation', 'overlay-hide 1.5s ease-in forwards !important');
    display: block;
    position: fixed;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    z-index: -1;
    background: #fff;
    opacity: 0;
    content: '';
  }
}
```

---

## animation
```
    // animation-name	指定要绑定到选择器的关键帧的名称(spinner-show)
    // animation-duration	动画指定需要多少秒或毫秒完成(1.5s)
    // animation-iteration-count	定义动画的播放次数。(1)
    // animation-delay	设置动画在启动前的延迟间隔。(0.25s)
    // animation-timing-function	设置动画将如何完成一个周期(ease)
    // animation-direction	指定是否应该轮流反向播放动画。(forwards)
    @include vendor('animation', ('spinner-show 1.5s 1 0.25s ease forwards', 'spinner-hide 0.25s ease-in-out forwards !important'));

    // transform-origin 属性允许您改变被转换元素的位置。旋转轴点(x,y)
    @include vendor('transform-origin', '50% 50%');
```

---

## 使页面上的字体抗锯齿,
```
    -moz-osx-font-smoothing: grayscale;
    -webkit-font-smoothing: antialiased;
```