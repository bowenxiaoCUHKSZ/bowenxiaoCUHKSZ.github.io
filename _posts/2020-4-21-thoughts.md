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
QUIC
TCP/IP 协议
HTTP 1.1/2的进化
数据库怎么读写分离
分布式事物，分布式锁
为什么分页: 历史上之前是连续的。分页，分段都有虚拟内存的影子，分段解决的是整段程序的隔离性（防止内存操作失误），分页更细化，解决的是程序进出内存的粗细度。
386
amd64
快排
三数之和
股票
解释从网页下载文件忽快忽慢
内存碎片（内存池）
头插法 反转链表
Golang 社招 https://www.nowcoder.com/discuss/412272?type=post&order=time&pos=&page=0&channel=
概述
1、什么是Redis
2、Redis有哪些优缺点
3、为什么要用 Redis /为什么要用缓存
4、为什么要用 Redis 而不用 map/guava 做缓存?
5、Redis为什么这么快
数据类型
1、Redis有哪些数据类型
2、Redis的应用场景
持久化
1、什么是Redis持久化？
2、Redis 的持久化机制是什么？各自的优缺点？
3、如何选择合适的持久化方式
4、Redis持久化数据和缓存怎么做扩容？
5、过期键的删除策略
6、Redis的过期键的删除策略
7、Redis key的过期时间和永久有效分别怎么设置？
8、我们知道通过expire来设置key 的过期时间，那么对过期的数据怎么处理呢?
内存相关
1、MySQL里有2000w数据，redis中只存20w的数据，如何保证redis中的数据都是热点数据
2、Redis的内存淘汰策略有哪些
3、Redis主要消耗什么物理资源？
4、Redis的内存用完了会发生什么？
5、Redis如何做内存优化？
线程模型
1、Redis线程模型
事务
1、什么是事务？
2、Redis事务的概念
3、Redis事务的三个阶段
4、Redis事务相关命令
5、事务管理（ACID）概述
6、Redis事务支持隔离性吗
7、Redis事务保证原子性吗，支持回滚吗
8、Redis事务其他实现
集群方案
1、哨兵模式
2、官方Redis Cluster 方案(服务端路由查询)
3、基于客户端分配
4、基于代理服务器分片
Redis 主从架构
1、Redis集群的主从复制模型是怎样的？
2、生产环境中的 redis 是怎么部署的？
3、说说Redis哈希槽的概念？
4、Redis集群会有写操作丢失吗？为什么？
5、Redis集群之间是如何复制的？
6、Redis集群最大节点个数是多少？
7、Redis集群如何选择数据库？
分区
1、Redis是单线程的，如何提高多核CPU的利用率？
2、为什么要做Redis分区？
3、你知道有哪些Redis分区实现方案？
4、Redis分区有什么缺点？
分布式问题
1、Redis实现分布式锁
2、如何解决 Redis 的并发竞争 Key 问题
3、分布式Redis是前期做还是后期规模上来了再做好？为什么？
4、什么是 RedLock
缓存异常
1、缓存雪崩
2、缓存穿透
3、缓存击穿
4、缓存预热
5、缓存降级
6、热点数据和冷数据
7、缓存热点key
常用工具
1、Redis支持的Java客户端都有哪些？官方推荐用哪个？
2、Redis和Redisson有什么关系？
3、Jedis与Redisson对比有什么优缺点？
其他问题
1、Redis与Memcached的区别
2、如何保证缓存与数据库双写时的数据一致性？
3、Redis常见性能问题和解决方案？
4、Redis官方为什么不提供Windows版本？
5、一个字符串类型的值能存储最大容量是多少？
6、Redis如何做大量数据插入？
7、假如Redis里面有1亿个key，其中有10w个key是以某个固定的已知的前缀开头的，如果将它们全部找出来？
8、使用Redis做过异步队列吗，是如何实现的
9、Redis如何实现延时队列
10、Redis回收进程如何工作的？
11、Redis回收使用的是什么算法？


