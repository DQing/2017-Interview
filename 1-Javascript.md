####什么是js跨域？
http://www.cnblogs.com/hustskyking/archive/2013/03/31/CDS-introduce.html
http://www.ruanyifeng.com/blog/2016/04/cors.html
http://www.cnblogs.com/rainman/archive/2011/02/20/1959325.html#m0
http://www.jianshu.com/p/63bb7b8f53ad

####2.怎么解决跨域问题？
https://segmentfault.com/a/1190000000718840
http://www.cnblogs.com/hustskyking/articles/ten-methods-cross-domain.html

####3.什么是闭包？
闭包是指有权访问另一个函数作用域中的变量的函数。
http://www.jianshu.com/p/d43df0e00bae
http://www.ruanyifeng.com/blog/2009/08/learning_javascript_closures.html
首先先要明白闭包出现的原因是什么，闭包是为了突破js的作用链，简单来说就是想要在外部访问函数内部变量。

####4.使用闭包的常用场景？
　　1.使用闭包代替全局变量
　　2.函数外或在其他函数中访问某一函数内部的参数
　　3.在函数执行之前为要执行的函数提供具体参数
　　4.在函数执行之前为函数提供只有在函数执行或引用时才能知道的具体参数
       5.为节点循环绑定click事件，在事件函数中使用当次循环的值或节点，而不是最后一次循环的值或节点
       6.暂停执行
       7.包装相关功能
http://blog.csdn.net/yanghua_kobe/article/details/6780181

####5.介绍js有哪些内置对象？js的基本数据类型？
内置对象：Function、Arguments、Math、Date、RegExp、Error
    Object、Array、Boolean、Number 和 String
数据类型：undefined，null，boolean，number，string， Object

####6.undefined和null的区别？
let x;
let y = null;
console.log(x);//undefined
console.log(y);//null
undefined表示你定义了一个名字‘x’，但是它没有指向任何东西。它时一个孤零零的名字，我们没法推断它到底是什么。
null表示你定义了一个名字‘y’，并且它指向了一个‘null’，代表空对象，它不是孤单的。

http://www.ruanyifeng.com/blog/2014/03/undefined-vs-null.html

####7.JavaScript原型，原型链 ? 有什么特点？
https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Inheritance_and_the_prototype_chain
http://www.jianshu.com/p/0178771710e3
http://www.jianshu.com/p/d18c55fac766
http://www.jianshu.com/p/76c4de1a44f3
https://segmentfault.com/a/1190000008739672（极力推荐）
https://segmentfault.com/a/1190000008754962（极力推荐）

####8.如何实现数组的随机排序？
http://codepen.io/douqing/pen/wJgrLL?editors=1112

####9.事件捕获与冒泡
https://segmentfault.com/a/1190000000749838
分别由微软和网景提出的对于事件的不同响应，微软提出了事件冒泡，事件由内向外响应
而网景提出的事件捕获刚好相反，是由外向内。而浏览器默认使用事件冒泡，但是我们可以使用addEventListener()方法控制事件。
冒泡Demo：http://codepen.io/douqing/pen/XMMNab?editors=1111
捕获Demo：http://codepen.io/douqing/pen/wJJoER?editors=1011
取消事件
标准是e.preventDefault()
IE 则是使用 e.returnValue = false;
怎么阻止事件冒泡
标准是e.stopPropagation()
IE 则是使用 e.cancelBubble = true

####10.JavaScript不用new怎么实现继承？
http://www.infoq.com/cn/articles/javascript-instantiation-and-inheritance

####11.webpack 打包文件体积过大
http://www.jianshu.com/p/a64735eb0e2b

####12.webpack如何打包？
Webpack 会分析入口文件，解析包含依赖关系的各个文件。这些文件（模块）都打包到 bundle.js 。Webpack 会给每个模块分配一个唯一的 id 并通过这个 id 索引和访问模块。在页面启动时，会先执行 entry.js 中的代码，其它模块会在运行 require 的时候再执行。
http://zhaoda.net/webpack-handbook/usage.html

####JS异步
http://javascript.ruanyifeng.com/advanced/promise.html
promise的三种状态：
异步操作“未完成”（pending）
异步操作“已完成”（resolved，又称fulfilled）
异步操作“失败”（rejected）


####在线promise书
http://liubin.org/promises-book/




