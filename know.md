## 03 
main.scss 需要搞懂其参数
```
@include skel-layout((
        reset: 'full',
        boxModel: 'border',
        grid: true,
        conditionals: true,
        containers: true,
        breakpoints: (
                desktop: (
                        containers: 1200px,
                        grid: (
                                gutters: (50px, 50px)
                        ),
                ),
                tablet: (
                        containers: 960px,
                        grid: (
                                gutters: (25px, 25px)
                        ),
                ),
                mobile: (
                        containers: (100%, true),
                        grid: (
                                gutters: (20px, 20px)
                        ),
                )
        )
));
```


## 08
```
@include skel-layout((
  // css reset
  reset: 'full',
  // apply a box model
  boxModel: 'border',
  // Use [column, row] to set both column and row gutters.
  grid: (gutters: (40px, 40px)),
  conditionals: true,
  containers: 1400px,
  breakpoints: (
    xlarge: (
      containers: 1200px
    ),
    large: (
      containers: 960px,
      grid: (gutters: (25px, 25px))
    ),
    medium: (
      containers: (90%, true)
    ),
    small: (
      containers: (100%, true),
      grid: (gutters: (20px, 20px))
    )
  )
));
```


## 08
typrography 不规范



## 03
完全没有按流程



## 01
```
    // 垂直居中-父元素高度确定的单行文本
    vertical-align: middle;
```


## 01
```
        // 圆
        border: solid 1px _palette(fg);
        border-radius: 100%;
        // ----- 圆的设置start -----
        width: 2.5em;
        height: 2.5em;
        line-height: 2.5em;
        // ----- 圆的设置end -----
```



## 01
垂直居中
```
  height: 6em;
  line-height: 6em;
  text-align: center;
```



## 02
```
  // 添加一个闪光效果
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
```


## 02 _image.scss error
由于图片途径不对而造成
但是该scss是合并到main里面，不会被用到，所以不用修改
对于main来说是正确图片路径