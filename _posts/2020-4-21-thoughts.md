---
layout: post
title: thoughts
---
* 1
如何检查当前本地版本与云端版本是否匹配 github : git log 查看提交记录
git fetch， reset : fetch 得到最新的版本号，reset返回origin/master
git checkout妙用 : checkout -> fetch -> merge
sudo fuser -k -n tcp 81 : 杀死端口tcp 81
Socket编程 (使用TCP, UDP) : 自己写一个基于TCP的传输 


* 2
curl, wget: wget轻便简单，curl可支持操作更多，类似于浏览器，不过不渲染
VPN 上网原理：通过vps配置iptables实现路由转发的目的，封装新的ip头，同时VPN协议会加密以绕过GFW.
~~移动网络~~
跳板机：集群权限控制，访问数据中心
内网穿透：外部的包发往内网主机，防止被NAT接受并转发的机制。

* 3
SDN, VPC:
虚拟化
Conda install 和 Pip Install的区别: 差不多，windows用conda
bashrc 和 export那个到底是啥意思，为什么source: $PATH 调用原来的变量
SIGPIPE: Broken Pipe
查IP：ifconfig -a 
什么是loop back?:
Linux开机启动详解：http://linux.chinaitlab.com/set/894157.html

* 4
Telnet关闭连接如何操作

* 5
Linux 描述字？
Linux connect会不会阻塞
telnet 底层是socket?
poller dispatch 是不是阻塞的？
go: k8s, TiDB, etcd, containered
go并发编程模式: 生产者消费者
ls -l: use a long listing format
mkfifo, ftok: mkfifo 建一个管道，跟channel很像 || ftok file to key (标识文件，具有幂等性)
inode
System V IPC： Linux IPC 机制
strace 系统调用

* 
ipcs
inode 转 key
JS .装箱操作
Symbol.iterator 
/etc/init.d/

* 
SGML
CDATA
await 一个非Promise值 直接返回

* 
学习的一种方式: 搜集所有API/归纳整理（从winter那里学的）, 可以先整理所有DOM的API
ES Modules 
Common JS
AMD

* 
QUIC: 多路复用，减少重新建立连接，滑动窗口应答机制offset,
TCP/IP 协议: 应用层HTTP,HTTPS,FTP,SMTP,TELNET,DNS,SSH; 传输层TCP,UDP,QUIC；网络层 IP, ICMP,ARP,RARP; 链路层Ethernet;
HTTP 1.1/2的进化: HTTP1.x是严格串行；多路复用，乱序响应（Stream,一个连接多个请求,避免队首阻塞），头部压缩
队首阻塞：HTTP(多个请求到达，必须先对前面的ACK)；
数据库怎么读写分离: 中间代理层 + or 自己封装操作对象（select从库，insert主库）。主从分离。
分布式事物，分布式锁: 事务分布在不同服务器上；分布式锁就是不同服务器要操作相同资源 -> 解决方案
为什么分页: 历史上之前是连续的。分页，分段都有虚拟内存的影子，分段解决的是整段程序的隔离性（防止内存操作失误），分页更细化，解决的是程序进出内存的粗细度。
解释从网页下载文件忽快忽慢: 多线程分布式下载，多个链接
内存碎片:（内存池）
头插法 反转链表： 遇到一个元素就插到前面去
Golang 社招: https://www.nowcoder.com/discuss/412272?type=post&order=time&pos=&page=0&channel=


* 
怎么查看内存，IO，CPU使用情况: top free uptime vmstat(上下文切换) pidstat df
TIME_WAIT连接太多怎么办: (端口占用：sa内核新机制，SO_REUSEADDR)
sysctl: 改参数
调度算法：实时进程(FIFO,RR,DDL)，普通进程(NORMAL,BATCH,IDLE),标记在task_struct上
golang的GC过程：mark and sweep; 写屏障；支持并发
go map底层：前8后8
channel异常
MTU
MSL

* 
快排
三数之和
股票
Linux profile 和 bashrc


* 
less, size
Canvas, WebGL, SVG
Bootstrap


