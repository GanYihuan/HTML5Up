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