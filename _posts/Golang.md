Golang 分布式缓存项目
[Golang 项目](https://www.cnblogs.com/Jun10ng/p/12628081.html)
[Go 底层](https://halfrost.com/go_slice/)
## Go 语言常问
* 协程，进程，线程
* docker 网络端口，文件隔离
* make的底层,len,cap,slice,数组初始化，扩容机制等等
扩容机制：如果无长度的切片，容量从1开始翻倍。有长度的切片，容量=长度*2。每次长度到达容量，翻倍。
如果容量超过1024，不翻倍了，增加25%。



* new 和 make 的区别
new: 仅仅分配0值的内存+不初始化，少用，返回值为指针
make: 分配内存+初始化，多用于slice, map, channel。返回值为引用类型。

  
* map底层实现, sync.Map 原理实现
* channel底层实现，异常处理
* Go并发模型
* 接口
* golang gc介绍
三色标记法介绍
甚至扯到了内存屏障
标记清扫法相比其他gc算法的好处在哪
* go的new make区别
* go的slice和array区别
  
Go 如何查看性能：pprof
Go 如何进行调试：gdb/delve
Go 如何打印堆栈：runtime.Caller

Golang生产者消费者模式， 写代码



go的调度
go struct能不能比较
go defer（for defer）
select可以用于什么
context包的用途
client如何实现长连接
主协程如何等其余协程完再操作
slice，len，cap，共享，扩容
map如何顺序读取
实现set
实现消息队列（多生产者，多消费者）
大文件排序

Go的反射包怎么找到对应的方法（这里忘记怎么问的，直接说不会，只用了DeepEqual，简单讲了DeepEqual）

Go的channel（有缓冲和无缓冲）

topk问题，海量数据topk

io模型，同步阻塞，同步非阻塞，异步

go的值传递和引用

go的new和make区别
go怎么从源码编译到二进制文件
go的调度模型
go的锁如何实现，用了什么cpu指令
go的runtime如何实现

c++的map和go的map的区别（红黑树和hashtable）
ctx包了解吗？有什么用？
go什么情况下会发生内存泄漏？（他说ctx没有cancel的时候，这个真不知道）
怎么实现协程完美退出？

实现一个hashmap，解决hash冲突的方法，解决hash倾斜的方法
c++的模板跟go的interface的区别
怎么理解go的interface
100亿个数选top5，小根堆

go并发网络编程（Go语言圣经）


生产者消费者模式，手写代码（Go直接使用channel实现很简单，还想着面试官会不会不让用channel实现，不用channel的可以使用数组加条件变量），channel缓冲长度怎么决定，怎么控制上游生产速度过快，这里没说出解决方案，只是简单说了channel长度可以与上下游的速度比例成线性关系，面试官说这是一种解决方案
手写循环队列
写的循环队列是不是线程安全，不是，怎么保证线程安全，加锁，效率有点低啊，然后面试官就提醒Go推崇原子操作和channel

select, epoll, poll 区别，原理
连接建立sockt()



