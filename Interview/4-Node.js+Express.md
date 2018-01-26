####什么是node.js？
Node.js不是JS应用、而是JS运行平台。Node.js是一个后端的Javascript运行环境（支持的系统包括*nux、Windows），这意味着你可以编写系统级或者服务器端的Javascript代码，交给Node.js来解释执行。
http://www.infoq.com/cn/articles/what-is-nodejs
 ####1。module.exports与exports？？关于exports的总结
https://cnodejs.org/topic/52308842101e574521c16e06

####import和require的区别
http://www.jianshu.com/p/85f4dde573c0
####2.CommonJS
CommonJS 是一套规范，它的创建和核准是开放的。
CommonJS 规范是为了解决 JavaScript 的作用域问题而定义的模块形式，可以使每个模块它自身的命名空间中执行。该规范的主要内容是，模块必须通过 module.exports 导出对外的变量或接口，通过require() 来导入其他模块的输出到当前模块作用域中。
CommonJS 是同步加载模块，但其实也有浏览器端的实现，其原理是现将所有模块都定义好并通过 id 索引，这样就可以方便的在浏览器环境中解析了，

####2 。AMD 规范
AMD（异步模块定义）是为浏览器环境设计的，因为 CommonJS 模块系统是同步加载的，当前浏览器环境还没有准备好同步加载模块的条件。
AMD 定义了一套 JavaScript 模块依赖异步加载标准，来解决同步加载的问题。

####什么是express
http://javascript.ruanyifeng.com/nodejs/express.html#toc1
