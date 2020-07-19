# Bootstrap


## ***** Bootstrap 是移动设备优先 *****

```html
1、<meta http-equiv="X-UA-Compatible" content="IE=edge">//开启IE8标准模式
2、<meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no">配置视窗（设备窗口，设备窗口宽度，初始等比例缩放，用户是否可以手动缩放）
3、引入Jquery，
4、引入Bootstrap CSS文件和JS文件
```

Bootstrap容器：container的orw行里的12col，在12col里的其中1个里可以再嵌套，如果大于12个，那么它会自动换行到下面去，因它是：float：left //向左浮动的
-------------------------------------------------------------------------------------------------------------
1、.container //定义容器宽度（固定宽度值）
.orw //1行
.col-md-1 //1列

col-[单位如下：]-
.col-xs-{【超小屏幕 手机】小于768px}【兼容大分辨率：就是小的，兼容大的】
.col-sm-{【小屏幕 平板】大于或等于768px}
.col-md-{【中等屏幕，显示器】大于或等于992px}
.col-lg-{【大屏幕，大显示器】大于或等于1200px}

2、.container-fluid //定义容器宽度（container-fluid 是在任可屏幕宽度下都是：百分之百的）

### bootstrap媒体查询：*****【是Bootstrap核心要素】*****用于在不同的分辨率下，设置不同的样式
-------------------------------------------------------------------------------------------------------------
```css
/* 超小屏幕（手机，小于 768px） */
/* 没有任何媒体查询相关的代码，因为这在 Bootstrap 中是默认的（还记得 Bootstrap 是移动设备优先的吗？） */

/* 小屏幕（平板，大于等于 768px） */
@media (min-width: @screen-sm-min) { ... }

/* 中等屏幕（桌面显示器，大于等于 992px） */
@media (min-width: @screen-md-min) { ... }

/* 大屏幕（大桌面显示器，大于等于 1200px） */
@media (min-width: @screen-lg-min) { ... }

实 例：

@media(max-width:768px)/*当屏幕大小，max小于768px时候*/
	{
		div{ background: red;}
	}

@media only screen and (min-width: 768px) and (max-width: 992px)/*当屏幕大小在min：768px -到- max：992px之间时候*/
	{
		div{ background: blue;}
	}
			
@media(min-width:1200px)/*当屏大小，大于min：1200px时候*/
	{
		div{ background: green;}
	}

```
-------------------------------------------------------------------------------------------------------------

## 常用样式
``` css
.h1-h6
p==.lead

div.form-group //（栅格系统中的【row】1行）把表单项下边距设为15px
input.form-control //input框宽度度100%

form>.form-inline //内联表单
form>.form-horizontal //水平排列的表单

.img-responsive //响应式图片

.navbar  //导航
.navbar  //导航默认样式
.navbar-fixed-top //将导航固定定位到顶部


.container-fluid // 定义容器宽度（宽度百分百【%】）

.navbar-toggle //导航缩小时按扭
.icon-bar导航缩小时按扭里面的横线

.navbar-brand//导航logo
.navbar-collapse导航
.collaps导航

ul .navbar-nav //导航菜单
ul .navbar-right//导航菜单居右显示

```