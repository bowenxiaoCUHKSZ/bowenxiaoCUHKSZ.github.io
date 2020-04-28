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



