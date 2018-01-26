####1 介绍一下标准的CSS的盒子模型？低版本IE的盒子模型有什么不同的
      http://blog.csdn.net/wzqnls/article/details/38109745
      http://www.jianshu.com/p/18c691450e87

####2. CSS选择符（选择器）有哪些？哪些属性可以继承？
    不可继承：也就是指子节点不能继承父节点的属性
    可继承：可继承就是父节点设置了这个属性后，子节点就可以继承他的属性
    http://www.dongcoder.com/detail-111410.html
http://www.jianshu.com/p/34b49f9ba3ac
css 选择符的优先级：
http://justcoding.iteye.com/blog/2312385

####3. CSS3新增伪类有那些
伪元素和伪类：http://kb.cnblogs.com/page/545911/ 
http://www.jianshu.com/p/09193034841b
CSS3新增特性：
     http://www.cnblogs.com/SKLthegoodman/p/css3.html
     https://www.ibm.com/developerworks/cn/web/1202_zhouxiang_css3/  
伪类和伪元素作用：
 css引入伪类和伪元素概念是为了格式化文档树以外的信息。也就是说，伪类和伪元素是用来修饰不在文档树中的部分，比如，一句话中的第一个字母，或者是列表中的第一个元素。
伪类和伪元素的区别：
伪类的操作对象是文档树中已有的元素，而伪元素则创建了一个文档数外的元素。因此，伪类与伪元素的区别在于：有没有创建一个文档树之外的元素。

####4.如何水平居中div？
    div{
     width:200px;   
    margin:0 auto;
     }
div{
   display:flex;
   justify-content：center;
}
使用flex：https://jsbin.thoughtworks.school/but/2/edit?html,css,output

####怎么垂直居中div？
http://www.jianshu.com/p/15ba8f6afec0

####5.display有哪些值？说明他们的作用。
     block           块类型。默认宽度为父元素宽度，可设置宽高，换行显示。
     none            此元素不会被显示
     inline           行内元素类型。默认宽度为内容宽度，不可设置宽高，同行显示。   
     inline-block  默认宽度为内容宽度，可以设置宽高，同行显示。
     list-item       象块类型元素一样显示，并添加样式列表标记。 
     table           此元素会作为块级表格来显示。
     inherit         规定应该从父元素继承 display 属性的值。

####display:inline-block会带来什么问题：
http://luopq.com/2015/11/01/display-inline-block/
####6.position的值relative和absolute定位原点是？
http://zh.learnlayout.com/position.html
http://www.jianshu.com/p/6dc704ac8c24

####7.CSS3有哪些新特性？
     新增各种CSS选择器  （: not(.input)：所有 class 不是“input”的节点）
     圆角            （border-radius:8px） 
     多列布局      （multi-column layout） 
     阴影和反射   （Shadow\Reflect）
     文字特效      （text-shadow、）
     文字渲染      （Text-decoration） 
     线性渐变      （gradient） 
     旋转            （transform） 
     缩放,定位,倾斜,动画,多背景 
           例如:transform:\scale(0.85,0.90)\ translate(0px,-30px)\ skew(-9deg,0deg)\Animation:
https://www.ibm.com/developerworks/cn/web/1202_zhouxiang_css3/

####8.请解释一下CSS3的Flexbox（弹性盒布局模型）,以及适用场景？
2009年，W3C提出了一种新的方案----Flex布局，可以简便、完整、响应式地实现各种页面布局。目前，它已经得到了所有浏览器的支持，这意味着，现在就能很安全地使用这项功能。
http://www.ruanyifeng.com/blog/2015/07/flex-grammar.html
采用Flex布局的元素，称为Flex容器（flex container），简称"容器"。  它的所有子元素自动成为容器成员，称为Flex项目（flex item），简称"项目"。  常规布局是基于块和内联流方向，而Flex布局是基于flex-flow流可以很方便的用来做局中，能对不同屏幕大小自适应。  在布局上有了比以前更加灵活的空间。

####9.怎么清除浮动
1.clear：both；
http://www.jianshu.com/p/18c691450e87
2.父级div定义 overflow: auto
3.:after 方法
先说原理：这种方法清除浮动是现在网上最拉风的一种清除浮动，他就是利用:after和:before来在元素内部插入两个元素块，从面达到清除浮动的效果。其实现原理类似于clear:both方法，只是区别在于:clear在html插入一个div.clear标签，而outer利用其伪类clear:after在元素内部增加一个类似于div.clear的效果。
https://codepen.io/yhl221/pen/wJgKLg

####10. 用纯CSS创建一个三角形的原理是什么？
http://codepen.io/douqing/pen/aJBeEo


####10. 一个满屏 品 字布局 如何设计?
http://www.itdadao.com/articles/c15a732729p0.html
代码实现：http://codepen.io/douqing/pen/OpWJyL

####11.inline-block和inline、block的区别
http://www.cnblogs.com/jdonson/archive/2011/06/10/2077932.html

####12.为什么要清除浮动？
https://www.zhihu.com/question/20063303
没看懂：http://codepen.io/douqing/pen/XMpWMV

http://snailsky.me/2014/08/20/%E6%B5%AE%E5%8A%A8%E5%92%8C%E5%AE%83%E7%9A%84%E5%B7%A5%E4%BD%9C%E5%8E%9F%E7%90%86%EF%BC%9F%E6%B8%85%E9%99%A4%E6%B5%AE%E5%8A%A8%E7%9A%84%E6%8A%80%E5%B7%A7%EF%BC%9F/

####13.::before 和 :after中双冒号和单冒号 有什么区别？解释一下这2个伪元素的作用。
单冒号(:)用于CSS3伪类，双冒号(::)用于CSS3伪元素。（伪元素由双冒号和伪元素名称组成） 双冒号是在当前规范中引入的，用于区分伪类和伪元素。不过浏览器需要同时支持旧的已经存在的伪元素写法， 比如:first-line、:first-letter、:before、:after等， 而新的在CSS3中引入的伪元素则不允许再支持旧的单冒号的写法。  想让插入的内容出现在其它内容前，使用::before，否者，使用::after； 在代码顺序上，::after生成的内容也比::before生成的内容靠后。 如果按堆栈视角，::after生成的内容会在::before生成的内容之上

####14.png、jpg、gif 这些图片格式解释一下，分别什么时候用。有没有了解过webp
https://www.zhihu.com/question/20028452

####15.CSS选择器权重及样式
http://wentaoma.com/2016/08/19/CSS-selector-weight/
浏览器的兼容性问题
http://developer.51cto.com/art/201008/218335.htm

####16. box-sizing用法
http://www.jianshu.com/p/f4f35684970e
http://zh.learnlayout.com/box-sizing.html

####17.css中px rem em之间的区别?
https://segmentfault.com/a/1190000005936910

####18.CSS LESS官方文档
http://less.bootcss.com/

####19.CSS SASS教程
https://www.w3cplus.com/sassguide/syntax.html

####BFC
http://www.html-js.com/article/1866
https://www.w3ctech.com/topic/865






