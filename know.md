## 03 
main.scss 需要搞懂其参数
```scss
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
```scss
@include skel-layout((
        reset: 'full',
        boxModel: 'border',
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