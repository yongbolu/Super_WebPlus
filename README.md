# Super_WebPlus
This is a project for web of forhead
META常识
一、什么是Viewport
手机浏览器是把页面放在一个虚拟的“窗口”（viewport）中，通常这个虚拟的“窗口”（viewport）比屏幕宽，这样就不用把每个网页挤到很小的窗口中（这样会破坏没有针对手机浏览器优化的网页的布局），用户可以通过平移和缩放来看网页的不同部分。移动版的 Safari 浏览器最新引进了 viewport 这个 meta tag，让网页开发者来控制 viewport 的大小和缩放，其他手机浏览器也基本支持。
1、H5页面窗口自动调整到设备宽度，并禁止用户缩放页面
<meta name="viewport" content="width=device-width,initial-scale=1.0,minimum-scale=1.0,maximum-scale=1.0,user-scalable=no>
说明：
	width - viewport的宽度 height - viewport的高度
	initial-scale - 初始的缩放比例
	minimum-scale - 允许用户缩放到的最小比例
	maximum-scale - 允许用户缩放到的最大比例
	user-scalable - 用户是否可以手动缩放
2、忽略将页面中的数字识别为电话号码
<meta name="format-detection" content="telephone=no" />
3、忽略Android平台中对邮箱地址的识别
<meta name="format-detection" content="email=no" />
4、当网站添加到主屏幕快速启动方式，可隐藏地址栏，仅针对ios的safari
<meta name="apple-mobile-web-app-capable" content="yes" />
<!-- ios7.0版本以后，safari上已看不到效果 -->
5、将网站添加到主屏幕快速启动方式，仅针对ios的safari顶端状态条的样式
<meta name="apple-mobile-web-app-status-bar-style" content="black" />
<!-- 可选default、black、black-translucent -->
6、viewport模板
<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<meta content="width=device-width,initial-scale=1.0,maximum-scale=1.0,user-scalable=no" name="viewport">
<meta content="yes" name="apple-mobile-web-app-capable">
<meta content="black" name="apple-mobile-web-app-status-bar-style">
<meta content="telephone=no" name="format-detection">
<meta content="email=no" name="format-detection">
<title>标题</title>
<link rel="stylesheet" href="index.css">
</head>

<body>
</body>

</html>
7、viewport模板 – target-densitydpi=device-dpi，android 2.3.5以下版本不支持
<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=750, user-scalable=no, target-densitydpi=device-dpi"><!-- width取值与页面定义的宽度一致 -->
<meta content="yes" name="apple-mobile-web-app-capable">
<meta content="black" name="apple-mobile-web-app-status-bar-style">
<meta content="telephone=no" name="format-detection">
<meta content="email=no" name="format-detection">
<title>标题</title>
<link rel="stylesheet" href="index.css">
</head>

<body>

</body>

</html>