---
layout: post
title: Front End Interview
---

In this post, I will record my learning experience with front-end

## JS basics
Useful Resources:
* 廖雪峰JavaScript教程
* 《大前端吊打面试官系列》之原生 JavaScript 精华篇 (Other articles in this series are BS)
*  牛客网面经大汇总（Practice is the best!）
* [前端技术大汇总](https://fecommunity.github.io/front-end-interview/): 目前找到的最全的
* [前端复习](https://blog.nowcoder.net/yiizgo?page=2): 做成了一个系列
* [前端大宝典](http://blog.poetries.top/FE-Interview-Questions/?nsukey=Vob4o0G8K8%2FsVICltad6pncGURJVdFFUf1%2F%2Be06JHb9Vz%2BPnmwFijIjHxzbxEMQUHl3PP79bzicBUL0aX5oRvcx5D0TyHFodklAzVzXMVThfJSJdv%2FzXqs5PbNi50wDKdPn0mPpygThRidI%2FqrsjJhDURaMb62k%2FKQElLM5bzM9YrV0EexCobd2xIGs87Q3JAo9z%2FGYYeQv8nDPB1ZECDw%3D%3D)
* [深入JS系列](https://github.com/mqyqingfeng/Blog)
* 优化：雅虎36条军规

## Frequent Questions
* Implement bidirectional binding of Vue.js
* Process from input url to display
* XSS, CSRF
* 深拷贝和浅拷贝
* how to leave out duplicate elements (or find the frequency >= n)
* 继承的方式
* 原型和原型链
* 如何实现new
* 类型判断(toString等等)
* how to judge a variable is Array or Object?
* Implement Deep Copy and Shallow Copy
* Cross Site Request
* Hand written AJAX
* 对CSS实现垂直居中
* JSONP, CORS原理
* [Promise 原理 （异步）](https://juejin.im/post/5d6f7c83e51d4561c541a712)这篇文章不厉害，参考链接还可以
* cookie，浏览器储存
* 三次挥手四次握手
* apply, call, bind, new 实现
* Vue-Router 原理
* [JS 事件循环机制(Event Loop) + 阮一峰的Promise讲解等等](https://juejin.im/post/5cc64a71e51d456e51614b2f)
* JS 设计模式（练熟发布订阅即可）
* Http Headers: Cache-control, Access-Control-Allow-Origin等等



## 一些简单问题的总结
* 闭包的原理？
主要是作用域链。外部函数新建时会建立一个新的作用域链，内部函数会记住这个作用域链，所以这上面的变量不会被垃圾回收，可以被嵌套函数访问。

作用：实现私有成员；避免全局变量污染；记住变量；保护命名空间

* Vue 的 双向绑定实现原理
2.0使用Object.defineProperty（数据劫持，发布者订阅者模式），3.0使用Proxy（直接劫持整个对象，增强数据访问时的拦截）

* script标签中的async和defer
defer：等到DOM加载完成后在执行，预先下载
async: 另开一个进程去加载和执行

* Promise面试题等:
[Promise](https://juejin.im/post/5c9a43175188252d876e5903#heading-3)
[SF解答](https://segmentfault.com/q/1010000018689196?_ea=19219106) 


 
