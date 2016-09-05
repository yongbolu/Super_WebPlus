# META常识
一、什么是Viewport    
手机浏览器是把页面放在一个虚拟的“窗口”（viewport）中，通常这个虚拟的“窗口”（viewport）比屏幕宽，这样就不用把每个网页挤到很小的窗口中（这样会破坏没有针对手机浏览器优化的网页的布局），用户可以通过平移和缩放来看网页的不同部分。移动版的 Safari 浏览器最新引进了 viewport 这个 meta tag，让网页开发者来控制 viewport 的大小和缩放，其他手机浏览器也基本支持。  

1. H5页面窗口自动调整到设备宽度，并禁止用户缩放页面    
`<meta name="viewport" content="width=device-width,initial-scale=1.0,minimum-scale=1.0,maximum-scale=1.0,user-scalable=no>`   
>说明：    
	width - viewport的宽度 height - viewport的高度  
	initial-scale - 初始的缩放比例  
	minimum-scale - 允许用户缩放到的最小比例  
	maximum-scale - 允许用户缩放到的最大比例  
	user-scalable - 用户是否可以手动缩放  

2. 忽略将页面中的数字识别为电话号码    
`<meta name="format-detection" content="telephone=no" />`
3. 忽略Android平台中对邮箱地址的识别    
`<meta name="format-detection" content="email=no" />`    

4. 当网站添加到主屏幕快速启动方式，可隐藏地址栏，仅针对ios的safari    
`<meta name="apple-mobile-web-app-capable" content="yes" />`    
`<!-- ios7.0版本以后，safari上已看不到效果 -->`
5. 将网站添加到主屏幕快速启动方式，仅针对ios的safari顶端状态条的样式      
`<meta name="apple-mobile-web-app-status-bar-style" content="black" />
<!-- 可选default、black、black-translucent -->`
6. viewport模板    

    `<!DOCTYPE html>`    
    `<html>`    
    `<head>`    
    `<meta charset="utf-8">`    
    `<meta content="width=device-width,initial-scale=1.0,maximum-scale=1.0,user-scalable=no"    name="viewport">`    
    `<meta content="yes" name="apple-mobile-web-app-capable">`    
    `<meta content="black" name="apple-mobile-web-app-status-bar-style">`    
    `<meta content="telephone=no" name="format-detection">`    
    `<meta content="email=no" name="format-detection">`    
    `<title>标题</title>`    
    `<link rel="stylesheet" href="index.css">`    
    `</head>`    
    `<body>`    
    `</body>`    
    `</html>`  

7. viewport模板 – target-densitydpi=device-dpi，android 2.3.5以下版本不支持    

    `<!DOCTYPE html>`    
    `<html>`    
    `<head>`    
    `<meta charset="utf-8">`    
    `<meta name="viewport" content="width=750, user-scalable=no`    
    `target-densitydpi=device-dpi"><!-- width取值与页面定义的宽度一致 -->`    
    `<meta content="yes" name="apple-mobile-web-app-capable">`    
    `<meta content="black" name="apple-mobile-web-app-status-bar-style">`    
    `<meta content="telephone=no" name="format-detection">`    
    `<meta content="email=no" name="format-detection">`    
    `<title>标题</title>`    
    `<link rel="stylesheet" href="index.css">`    
    `</head>`    
    `<body>`    
    `</body>`    
    `</html>`
# 面试前端176问

1．html5有哪些新标签？
2．header、footer标签在什么时候使用？
3．怎么把一个nav标签固定到底部？
4．fixed和absolute有什么区别？
5．怎样得到浏览器窗口的宽度和高度？
6．用div模拟按扭，当鼠标移上去的时候放大一些，怎么实现？按下缩小呢？
7．jQuery支持哪些动画效果？
8．点击显示和隐藏怎么实现？
9．动画执行完毕之后需要执行一段代码该怎么做？
10．jQuery Deferred都有哪些常用的方法？分别是什么作用？
11．对Deferred的then进行链式调用时有什么要求，有什么作用？
12．Deferred的then链式调用和非链式调用有什么区别？
13．使用Deferred或Promise的好处是什么？
14．jQuery3.0有什么新变化？
15．js中的this有什么特点？jQuery('li').each(function)中，function中的this指向什么？
16．怎么改变this指向？call和apply的区别是什么？call和bind的区别是什么？
17．jQuery怎样添加和移除事件监听函数？
18．JQuery中如果某事件只需处理一次怎样添加监听函数？
19．如果希望事件监听对以后添加到页面上的新标签也有效，应该怎么做？
20．JS中事件传播过程是什么？怎么阻止事件传播？
21．document的DOMContentLoaded事件什么时候发生？window的load事件什么时候发生？
22．文件框中输入的内容变化时立即获得事件通知应该监听什么事件？
23．表单中进行什么样的操作会导致表单提交？如果希望阻止表单提交怎么办？
24．typeof(function(){})返回什么？typeof([])返回什么？
25．怎么判断一个变量是否是数组？
26．alert(‘3’- 1)弹出什么？
27．从文本框是得到value，怎么转换成整数？怎么转换成小数？
28．整数怎么保留2位小数？保留2位小数后是什么类型


29．CSS3有哪些新样式？
30．怎样实现类似报纸的多列分栏效果？
31．CSS3中新增了什么布局方式？
32．除了上述布局方式外还有什么常用的布局方式？
33．什么时候使用浮动？如果后面的元素受到影响怎么解决？
34．不添加新标签清除浮动能不能做到？
35．CSS中的calc()有什么作用？
36．什么时候使用mm、cm？
37．如果一个页面即要在屏幕上显示，又要打印，怎么将这2种样式定义在一起？
38．如果分别定义成2个样式文件该怎样导入页面？
39．媒体查询除了在打印时使用还在什么情况下使用？
40．在手机页面上使用图片，宽度为80%，怎么让图片居中？
41．手机页面底部工具条中4个图标，怎么均分空间？设边框后最后一个掉下去怎么办？
42．viewport是什么？什么时候使用？有什么作用？
43．box-sizing什么时候用？常用的值都有什么？
44．vertical-align什么时候使用？常用的值分别有什么作用？
45．CSS Sprite图片精灵都涉及哪些样式？
46．CSS3中的transform都支持哪些变换效果？
47．CSS3中的动画能否暂停和继续执行？
48．CSS3中的transition能否过渡opacity?能否过渡display？
49．什么时候使用transition?什么时候使用animation？
50．animation怎样能够被触发?
51．简述bootstrap的栅格系统的特点，
52．怎么实现桌面4列、平板2列、手机1列？
53．页面上有一个aside标签，在桌面上是显示的，但平板和手机是隐藏的，怎么实现？
54．.container、.container-fluid和.row有什么作用，有什么不同？
55．什么是原型和原型链？
56．js中的this指向有什么特点？怎么改变this指向，它们有什么区别？
57．怎样将两个对象混合在一起？
58．怎样建立原型链？
59．什么是闭包？闭包有什性质？
60．ES6有什么新特性？
61．jQuery中的proxy方法有什么作用？
62．jQuery中执行一个动画后，隔2s后再执行一个动画应该怎么写？
63．jQuery中怎么停止动画？停止后参与动画的标签元素会处于什么状态？
64．jQuery中能不能改变动画频率？
65．jQuery中能否在color或background-color等颜色值上实施动画？
66．jQuery插件有2种类型，分别是哪2种？
67．你用过哪些jQuery插件？
68．jQuery中的Callbacks是什么？有什么用？有哪些常用方法？
69．使用jQuery在同一个页面发起多个Ajax请求时能否将共同的请求设置一次性设置好？能否用一个函数处理所有请求的失败？
70．JSONP是什么？jQuery是否支持JSONP？怎么支持的？
71．你还知道其他的跨域请求文案吗？
72．jQuery Ajax怎么设置请求头？怎么获取响应头？怎么设置请求超时时间？
73．jQuery Ajax发起POST请求时，如果数据需要以JSON格式发送到服务端该怎su？
74．怎样通过jQuery Ajax请求上传文件？
75．怎样实现将图片从文件夹拖拽到页面时将图片显示到页面上？如果拖拽到页面上就直接通过Ajax上传到服务器呢？
76．input[type=file]能否设置一次选择多个文件？能够限制上传文件的类型？
77．通过jQuery能否向页面导入新的js脚本文件（用哪个方法），如果希望在加载的js脚本执行后运行一段代码该怎么办？
78．RequireJs与jQuery的getScript()方法有什么不同？
79．RequireJs中怎么指定页面的主js脚本文件？
80．RequireJs中怎么定义模块？怎么指定模块依赖项？
81．RequireJs中怎么将数据或功能导出模块？
82．RequireJs中怎么加载模块，并在模块加载完成后执行代码？
83．RequireJs中如果要加载jQuery应该怎么做？
84．RequireJs中如果要加载jQuery插件应该怎么做？
85．RequireJs除了能加载js脚本文件外，能否加载其它文件？怎么做？
86．ArtTemplate支持if/else吗？除了if/else之外还有什么方法能实现条件判断？
87．ArtTemplate支持循环处理数据（如数组）吗？
88．ArtTemplate支持引用子模板吗？
89．ArtTemplate支持将模板字符串编译成函数吗？
90．ArtTemplate支持Express吗？
91．Express怎么处理静态文件请求？
92．Express路由怎么定义，怎么使用？
93．Express请求处理管线怎么使用？
94．Express中使用什么模块可以获得POST数据？
95．Express中使用什么模块可以获得上传的文件？
96．Express中怎么从URL的path中获得参数？
97．Express中怎么从URL的QueryString中获得参数？
98．npm是什么？
99．npm init命令的作用是什么？
100．Node.js中导入模块和导入js文件写法上有什么区别？
101．Grunt是什么？有哪些常用的插件？
102．知道Gulp吗？
103．用过Less吗？它与CSS有什么不同？
104．知道SASS/SCSS吗？它与Less有什么不同？


105．Backbone中常说的MVC表示什么？
106．Backbone中怎样从Model、View等继承？initialize()方法有什么作用？
107．Backbone中Model支持数据默认值吗？
108．Backbone中怎样从Model中获取属性值和修改Model中属性的值？
109．Backbone中Model支持数据变化跟踪功能吗？怎么获得数据的当前值，之前值，从上次同步以来发生变化的值？
110．Backbone中Model怎么进行数验证？怎么获取验证结果？
111．Backbone中Model怎么向服务端进行数据增删改查？url怎么指定？Model中的id有什么作用？
112．Backbone中如果服务端返回的数据比较复杂，怎么转换成Backbone需要的数据？
113．Backbone中是否可以拦截所有的数据增删改查请求？
114．RESTful与非RESTful有什么区别？
115．Backbone中的Collection怎么向服务端进行数据增删改查？
116．Backbone中Collection怎样进行数据排序和筛选？
117．Backbone中View怎样监听事件？与jQuery有什么不同？
118．Backbone中View中的render()方法有什么作用？
119．Backbone中Router定义谁和谁的映射关系？
120．Backbone中怎样开启url变化监听？


121．Angular与Backbone理念上最大的区别是什么？
122．怎么理解Angular中的依赖注入？
123．Angular中指令为什么不叫属性？
124．Angular的ngApp指令的作用是什么？ngInit呢？Angular是否能够手动启动？
125．Angular中与ngModel有关的控制器叫什么？它的核心功能是什么？
126．Angular中与form表单有关的控制器叫什么？它的核心功能是什么？
127．Angular中表单输入状态有哪些？
128．Angular中表单验证状态有哪些？
129．Angular中支持自定义验证吗？怎么做？
130．Angular中页面上输入框中的值与作用域中对应属性的值是否永远保持一致？
131．Angular中当输入框中的值改变时要经历哪些步骤才会导致作用域中相应属性值发生变化？作用域属性值发生变化后又怎样传播到页面上的其它地方？
132．在Angular执行环境（模块）外部能否获取作用域？如果改变作用域，是否会直接同步到其它地方？如果不能，怎么解决？
133．Angular中双向绑定机制在内部是怎么实现的，涉及了哪些方法？
134．Angular中的作用域链的构成原理是什么？对于绑定有什么帮助？
135．Angular过滤器都有哪些？
136．Angular中能否自定义过滤器？怎么定义？
137．Angular中ngRepeat指令有什么作用？它的作用域有什么特点？
138．Angular中与ngRepeat指令相关的常用过滤有哪些？它们的作用是什么？
139．Angular中怎么提高ngRepeat的性能？
140．Angular中$rootscope是什么（服务service还是提供者provider）？它有什么用？
141．Angular中的$http服务是Angular中自带的还是在其它模块中？它有什么作用？支持哪些常用方法？
142．Angular中的$httpProvider有什么用？与$http的关系是什么？
143．Angular中的如何获取指定的模块？
144．Angular中定义模块时第2个参数有什么作用？
145．Angular中ngResource模块有什么用？
146．Angular中ngAnimate模块有什么用？能否与animate.css动画库配合使用？
147．Angular中ngRoute模块有什么用？怎么定义路由？ngView指令有什么用？
148．你用过uiRoute吗？与ngRoute有什么区别？
149．Angular是否支持类于SSI的功能？
150．Angular模块中都可以定义什么东西？


151．怎么实现视差滚动？
152．怎么在页面上绘制曲线图等图表？能否支持双Y轴？
153．手机页面怎么支持手势识别？
154．cookie和localstorage有什么区别？
155．JS支持多线程吗？
156．JS支持Socket双工双向通信吗？
157．JS支持GPS定位吗？
158．JS可以实现摇一摇吗？
159．微信可以实现语音识别吗？
160．什么时候使用git分支？怎么创建分支？怎么合并分支？
161．Git 合并冲突了怎么办？
162．Git第一次从远程库获取代码用什么命令？
163．Git从远程库获取更新用什么命令？
164．Git将已提交的代码发送到远程库用什么命令？
165．Git查看提交历史记录用什么命令？
166．怎么将Web页面打包成App？


167．你们之前是怎么估计项目的开发时间的？估计的偏差大吗？
168．你之前的公司都有哪些部门？都分别负责什么事？
169．你之前工作的城市有什么好吃的？有什么好玩的地方？
170．我去过你之前工作的城市，有一个xxx地方，你去过吗？
171．你怎么与你的领导相处？什么时候向他汇报工作？
172．你遇到难题时怎么解决？
173．你经常上哪些技术网站？
174．你现在在哪住？到这儿上班远不远？怎么解决？
175．你平时下班了都干什么？
176．你怎么看待公司的规章制度？