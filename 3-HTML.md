#### https://github.com/markyun/My-blog/tree/master/Front-end-Developer-Questions/Questions-and-Answers

#### 1. DOCTYPE的标准模式&怪异模式
 http://www.cnblogs.com/imxiu/p/3541932.html
 http://www.w3school.com.cn/tags/tag_doctype.asp
html5后严格按w3c标准执行，html4是DOCTYPE有三种声明：严格模式，过渡模式，框架模式

#### 2. DTD是什么？
 Document Type Declaration（文档类型声明，缩写 DTD）
 DTD  文档类型定义  (Document Type Definition)  DTD 是一套关于标记符的语法规则。它是XML1.0版规格的一部分,是XML文件的验证机制,属于XML文件组成的一部分。  DTD 是一种保证XML文档格式正确的有效方法，可以通过比较XML文档和DTD文件来看文档是否符合规范，元素和标签使用是否正确。一个DTD文档包含：元素的定义规则，元素间关系的定义规则，元素可使用的属性，可使用的实体或符号规则。  XML文件提供应用程序一个数据交换的格式,DTD正是让XML文件能够成为数据交换的标准,因为不同的公司只需定义好标准的DTD,各公司都能够依照DTD建立XML文件,并且进行验证,如此就可以轻易的建立标准和交换数据，这样满足了网络共享和数据交互。  DTD文件是一个ASCII的文本文件，后缀名为.dtd。
 
#### 2.块级元素&行级元素&空元素
 规定每个元素都有display属性，确定该元素的类型，每个元素都有默认的display值，如div的display默认值为“block”，则为“块级”元素；span默认display属性值为“inline”，是“行内”元素。
行级元素有：```<span>,<a>,<img>,<input>,<textarea>,<label>``` . 块级元素有：```<div>,<p>,<h1>,<ol>,<table>,<ul>,<pre>```
  http://www.jianshu.com/p/50e6ef5112a6
  http://www.jianshu.com/p/2e1e6a4bee8e

#### 3.浏览器内核（渲染引擎）和JS引擎
 http://www.jianshu.com/p/e22cbcc357c2
 渲染引擎决定了浏览器如何显示网页的内容以及页面的格式信息。不同的浏览器内核对网页编写语法的解释也有不同，因此同一网页在不同的内核的浏览器里的渲染（显示）效果也可能不同，这也是网页编写者需要在不同内核的浏览器中测试网页显示效果的原因。
JavaScript引擎是一个专门处理JavaScript脚本的虚拟机，一般会附带在网页浏览器之中。

#### 4.SGML是什么？
标准通用标记语言（Standard Generalized Markup Language，SGML）是现时常用的超文本格式的最高层次标准，是可以定义标记语言的元语言
HTML和XML同样衍生于它：XML可以被认为是它的一个子集，而HTML是它的一个应用(html5已经独立于SGML之外了)
https://zh.wikipedia.org/wiki/SGML

#### 5 . html5有哪些新特性、移除了那些元素？
HTML5 现在已经不是 SGML 的子集主要是关于图像，位置，存储，多任务等功能的增加。
绘画 canvas;
用于媒介回放的 video 和 audio 元素;
本地离线存储 localStorage 长期存储数据，浏览器关闭后数据不丢失; 
sessionStorage 的数据在浏览器关闭后自动删除;      
语意化更好的内容元素，比如 article、footer、header、nav、section;      
表单控件，calendar、date、time、email、url、search;    
新的技术webworker, websocket, Geolocation; 
http://www.html5tutorial.info/（HTML5新特性详解）
http://www.bbsmax.com/A/GBJrZj39J0/
移除的元素：     
纯表现的元素：basefont，big，center，font, s，strike，tt，u;     
对可用性产生负面影响的元素：frame，frameset，noframes；

#### 6 .HTML5的历史及各大浏览器支持情况
https://zh.wikipedia.org/zh-cn/HTML5
IE8/IE7/IE6支持通过document.createElement方法产生的标签，可以利用这一特性让这些浏览器支持HTML5新标签，浏览器支持新标签后，还需要添加标签默认的样式。
当然也可以直接使用成熟的框架、比如html5shim;
<!--[if lt IE 9]>
         <script> src="http://html5shim.googlecode.com/svn/trunk/html5.js"</script>   
<![endif]-->

#### 7.如何区分HTML5
DOCTYPE声明
新增的结构元素
功能元素

#### 8.canvas是如何使用以及原理
之前使用canvas写小游戏学习资料：
https://shimo.im/doc/bDXeI3fHAosoBXQP
https://shimo.im/doc/zsFUpJD8rQovpjLc


#### 9.localStorage是如何使用以及原理
http://www.w3school.com.cn/html5/html_5_webstorage.asp
http://www.cnblogs.com/xiaowei0705/archive/2011/04/19/2021372.html
在HTML5中，本地存储是一个window的属性，包括localStorage和sessionStorage，从名字应该可以很清楚的辨认二者的区别，前者是一直存在本地的，后者只是伴随着session，窗口一旦关闭就没了。

localStorage将数据保存在客户端硬件设备上

#### 10.sessionStorage是如何使用以及原理
sessionStorage 方法针对一个 session 进行数据存储。当用户关闭浏览器窗口后，数据会被删除。

#### 11.浏览器是怎么对HTML5的离线储存资源进行管理和加载的呢？

#### 11.HTML5的离线储存怎么使用，工作原理能不能解释一下？
在用户没有与因特网连接时，可以正常访问站点或应用，在用户与因特网连接时，更新用户机器上的缓存文件。 原理：HTML5的离线存储是基于一个新建的.appcache文件的缓存机制(不是存储技术)，通过这个文件上的解析清单离线存储资源，这些资源就会像cookie一样被存储了下来。之后当网络在处于离线状态下时，浏览器会通过被离线存储的数据进行页面展示。  
如何使用：
1、页面头部像下面一样加入一个manifest的属性；
2、在cache.manifest文件的编写离线存储的资源；
   
   CACHE MANIFEST
   #v0.11 
   CACHE:     
   js/app.js
   css/style.css
   NETWORK:
   resourse/logo.png
   FALLBACK:
   / /offline.html 
 3、在离线状态时，操作window.applicationCache进行需求实现。
概念学习：http://www.cnblogs.com/chyingp/archive/2012/12/01/explore_html5_cache.html
实例：http://www.w3school.com.cn/tiy/t.asp?f=html5_html_manifest
HTML5 离线缓存-manifest简介有趣的HTML5
离线存储

#### 11 .离线储存（manifest）和本地存储(localStorage)时两个不同的方式，有什么区别，分别怎么应用？
http://www.jianshu.com/p/fff9e5c46b9e
html5的manifest 和 使用localStorage 那种方式好
https://www.pureweber.com/article/html5/

#### 12.请描述一下 cookies，sessionStorage 和 localStorage 的区别？
cookie是网站为了标示用户身份而储存在用户本地终端（Client Side）上的数据（通常经过加密）。 
cookie数据始终在同源的http请求中携带（即使不需要），记会在浏览器和服务器间来回传递。 
sessionStorage和localStorage不会自动把数据发给服务器，仅在本地保存。
存储大小：
     cookie数据大小不能超过4k。  
    sessionStorage和localStorage 虽然也有存储大小的限制，但比cookie大得多，可以达到  
    5M或更大。
有期时间： 
     localStorage：存储持久数据，浏览器关闭后数据不丢失除非主动删除据；                        
    sessionStorage：数据在当前浏览器窗口关闭后自动删除。   
    cookie ： 设置的cookie过期时间之前一直有效，即使窗口或浏览器关闭
http://jerryzou.com/posts/cookie-and-web-storage/
1. cookie由服务端生成，用于标识用户身份；而两个storage用于浏览器端缓存数据
2. 三者都是键值对的集合
3. 一般情况下浏览器端不会修改cookie，但会频繁操作两个storage
4. 如果保存了cookie的话，http请求中一定会带上；而两个storage可以由脚本选择性的提交
5. 会话的storage会在会话结束后销毁；而local的那个会永久保存直到覆盖。cookie会在过期时间之后销毁。
6. 安全性方面，cookie中最好不要放置任何明文的东西。两个storage的数据提交后在服务端一定要校验（其实任何payload和qs里的参数都要校验）。

#### 13.简述一下你对HTML语义化的理解
    使用一些符合人们认知的标签，比如使用<nav>标签表示导航栏
    使得html语义化让页面的内容结构化，结构更清晰，便于对浏览器、搜索引擎解析;
    即使在没有样式CSS情况下也以一种文档格式显示，并且是容易阅读的;
    搜索引擎的爬虫也依赖于HTML标记来确定上下文和各个关键字的权重，利于SEO;
    使阅读源代码的人对网站更容易将网站分块，便于阅读维护理解。

#### 14.iframe是什么？怎么用？有那些缺点？
Iframes是页面框架，将页面放入另一个页面。
优点：
1. 解决加载缓慢的第三方内容如图标和广告等的加载问题
2. Security sandbox
3. 并行加载脚本
缺点：
1. iframe会阻塞主页面的Onload事件
2. 即时内容为空，加载也需要时间
3. 没有语意
使用iframe之前需要考虑这两个缺点。如果需要使用iframe，最好是通过javascript
动态给iframe添加src属性值，这样可以绕开以上两个问题。

#### 15.Label的作用是什么？是怎么用的？
label标签来定义表单控制间的关系,当用户选择该标签时，浏览器会自动将焦点转到和标签相关的表单控件上。
<label for="Name">Number:</label>
<input type=“text“name="Name" id="Name"/>
<label>Date:<input type="text" name="B"/></label>

#### 16.如何实现浏览器内多个标签页之间的通信? (阿里)
localstorage和cookie
17.webSocket如何兼容低浏览器？(阿里)
Adobe Flash Socket 、   ActiveX HTMLFile (IE) 、   基于 multipart 编码发送 XHR 、   基于长轮询的 XHR

#### 18.页面可见性（Page Visibility API） 可以有哪些用途？

#### 19.如何在页面上实现一个圆形的可点击区域？
1、map+area或者svg   
2、border-radius  
3.canvas

#### 20.实现不使用 border 画出1px高的线，在不同浏览器的标准模式与怪异模式下都能保持一致的效果。
  <div style="height:1px;overflow:hidden;background:red"></div> 

#### 21.网页验证码是干嘛的，是为了解决什么安全问题。

#### 22.title与h1的区别、b与strong的区别、i与em的区别？
http://www.cnblogs.com/SeeYouBug/p/6188583.html#_lab2_0_1

#### 23.关于Web语义化
What？
Web语义化，使用语义恰当的标签，可以让页面具有良好的结构，页面元素具有良好的含义，从而让人和机器人都能快速理解。语义化Web的Web页面一方面可以让机器在更少的人类干预情况下收集并研究网页信息，从而可以读懂网页的内容，然后将收集汇总的信息进行分析，结果为人类所用；另一方面它可以让开发人员读懂结构和用户以及屏幕阅读器（如果访客有视障）能够读懂内容。
Why？
1.有利于SEO（SEO也就是Search Engine Optimization，搜索引擎优化。指通过站内优化比如网站结构调整、网站内容建设、网站代码优化等以及站外优化，比如网站站外推广、网站品牌建设等，使网站满足搜索引擎收录排名需求，在搜索引擎中提高关键词排名，从而吸引精准用户进入网站，获得免费流量，产生直接销售或品牌推广。）
     人可以通过视觉的划分判断内容的语义,而搜索引擎只能通过爬取网页标签等代码来判断内容的语义。得到搜索引擎的有效爬取，是提高网站流量的有效方法之一。要使页面尽可能地对搜索引擎友好，所以就要尽可能地使标签和内容语义化。
在页面去掉或样式丢失的时候，能让页面呈现清晰的结构。html的一些标签，例如h1（粗体）,strong（加粗）,em（斜体）,通过一些默认的样式，可以使页面即使在缺失CSS样式修饰时也能呈现清晰的结构。
屏幕阅读器（如果访客有视障）会完全根据你的标记来“读”你的网页。
团队开发中，良好的语义化标签，可以减少很多差异化，减少成员间沟通成本，方便开发和后期维护，利于实现模块化开发。 
Web语义化的分类
       web语义化应该是样式与结构分离的结果，重构中的语义化包含：
HTML标签语义化，HTTP的语义化是针对HTTP协议来说。
CSS命名语义化
How？
HTML标签语义化 
HTML为网页文档内容提供上下文结构和含义。对于HTML体系而言，Web语义化是指使用语义恰当的标签，使页面有良好的结构，让页面元素有含义，便于被浏览器、搜索引擎解析。通常我们所说的HTML应该是完全脱离表现信息的，其中的标签应该都是语义化地定义了文档的结构。

一些常用的标签元素有：
本身无实在意义，组合其他HTML元素，常用于页面布局:div
设置文本，填充段落:h1~h6, p, span, strong, em…
表现列表：ul, li, ol, dl, dt, dd
表单相关：form,input,select,button
表格相关：table,thead,tbody,tfoot,th,tr,td
用于图像显示：img, canvas
打开链接，发送邮件，段落跳转：a 
此外，meta Description/meta keywords等针对搜索引擎和更新频度的描述和关键词的meta标签也会用来实现网页的SEO。 

HTML 规范其实一直在往语义化的方向上努力，许多元素、属性在设计的时候，就已经考虑了如何让各种用户代理甚至网络爬虫更好地理解 HTML 文档。HTML5 更是在之前规范的基础上，将所有表现层的语义描述都进行了修改或者删除，增加了不少可以表达更丰富语义的元素，也出现很多可以提到DIV元素的更具象的标签。

一个经典的页面结构如图：

     总之，HTML语义化是反对大篇幅使用无语义化的div+span+class,而鼓励使用HTML定义好的语义化标签。当然，如果需要兼容低版本的IE浏览器，比如说IE8以及以下，那就需要选择合适的兼容性的标签了。

CSS标签语义化
     CSS语义就是class和ID命名的语义。class属性作为HTML与CSS衔接的纽带，其本意是用来描述元素内容的。指用易于理解的名称对html标签附加的class或id命名。如果说HTML语义化标签是给机器看的，那么CSS命名的语义化就是给人看的。良好的CSS命名方式减少沟通调试成本，易于理解。 
    CSS命名首先要满足W3C的命名规范和团队的命名规范。其次是高效和可重用性。 就好像.main/.sidebar会比.left_content/.right_content的class命名灵活性更好。
     https://wiki.jenkins-ci.org/display/JENKINS/Installing+Jenkins+on+Ubuntu

#### web标准
web标准不是一个标准，而是一系列标准的集合。
网页主要有三部分组成：结构，表现和行为
对应的标准也分三方面：结构化标准语言主要包括XHTML和XML，表现标准语言主要包括CSS，行为标准主要包括对象模型、ECMAScript等。

