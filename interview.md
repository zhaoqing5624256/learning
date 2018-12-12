# DB
+ ##  Redis
  - 设计与实现，如果redis有一亿个key,使用keys命令是否会影响线上服务（会，因为是单线程模型，可以部署多个节点）
  - 持久化方式：aod and rdb，怎么实现
  - list怎么实现（ziplist压缩空间 and quicklist实现链表）
  - sorted set怎么实现（dict+skiplist）
  - skiplist数据结构，实现
  - Redis 底层用到了哪些数据结构？使用 Redis 的 set 来做过什么？
  - Redis 使用过程中遇到什么问题？搭建过 Redis 集群吗？
  - 存储一个 Blob 文件，如何建索引？如果前缀部分大都相似怎么办？文件大小相差太多怎么办？
  
+ ## MySQL 
  - 索引(innodb, b+ tree, 为什么用b+树做索引节点，一个节点存了多少数据，怎么规定大小，与磁盘页对应)
  - MySQL Hash 索引适用情况？举下例子？
  - 调优
  - 分库分表
  - 事务隔离级别
  - mongo ？
  - spark ?
  - MySQL 索引是不是越多越好？为什么？
  - 如何分析“慢查询”日志进行 SQL/索引 优化？
+ HBase

# Java
* ## 多线程 
  * concurrenthashmap 
  * countdownlatch
  * volatile
  * 内存模型
  * Java集合类哪些是线程安全的
  * ArrayList扩容
  * G1和CMS的区别
  * Kafka的整体架构
  * Netty的一次请求过程
  * Java1.7和1.8版本HashMap内部结构的区别
  * 自旋锁/偏向锁/轻量级锁
  * ThreadLocal如果引用一个static变量是不是线程安全的

* sync/async IO
* 垃圾回收算法
* Java 内存分配策略？多个线程同时请求内存，如何分配？
* final 关键字如何实现
* 集合类，hashmap，HashMap怎么实现的
* 类加载
* finalize
* CopyOnWriteArrayList
 
# 算法
 * kth number in an array
 * quick sort worst case, best case
 * heap sort
 * depth first traversal tree
 * insert node to sorted tree 
 * 有向有权图，如何判断是否有环(dfs,bfs),拓扑图
 * 二叉树，最长路径(某个子树深度特别大怎么办)
 * 36进制加法
 * 单链表加法
 * 寻找峰值
 * use two stack(push, pop, count) to implement queue(enqueue, dequeue)
 * 从list当中取和为sum的数
 * n个无序正整数列表，取出a1,a2,a3..., a1<a2<a3..., 并且a1+a2+a3最大
 * 有一条马路，马路上有很多树，树的高度不一。现在要统一剪树，剪到高度为h。意思就是，比h高的树都剪到h，比h低的树高度不变。所有的树剪掉的总长度为C。现在要使C>某个值的情况下(假设为MM)，使h最大。问怎么确定h。如果误差是十的-6次方，时间复杂度是多少
 * find number in rotated sorted array
 * 求最大连续子数组和
 * 求字符串差集
 * 求平方根
 * PathSum
 * n个字符串，要求在每个字符串上都存在的字符
 * 线程安全，单例
 * n个树中找出异或与最大的数
 * 排序链表
 * 给n个数，求这n个数组成的集合的所有子集
 * 平面上有n个点，求最多有多少个点在同一条直线上
 * 给n个数，求最大的区间和
 * 给n个非降序的数和一个数k，求出k在n个数中第一次出现的位置
 * 给一个01矩阵，求出全为1的最大矩形位置和面积
 * 红黑树/旋转
 * 大数相加
 * 桶排序
 * 蛇形打印
 * Minimum Window Substring


* ## 图
  * 最小生成树: prime, kruskal
  * 最短路径: floyd,  dijkstra
  * 最长公共子序列
 
  
# operating system
 * linux 磁盘管理
 * linux 进程间通信方式 5
 * linux 共享内存如何实现
 * cgroup 在linux具体实现
 * 僵尸进程，孤儿进程(如何避免僵尸进程，父进程怎么知道子进程结束)
 * 进程死锁
 * 实现LRU cache（超时淘汰，LRU淘汰） linkedlist 和 hashmap实现
 * 内存管理
 * Buffered IO

# 虚拟化
 * docker 物理机 虚拟机 部署 实现
 * k8 ?

# 网络
+ ## TCP
  + 三次握手,不要第三次握手行不行，被黑客利用，对服务器DDos攻击：https://www.jianshu.com/p/1c65840fc02d
  + 四次挥手
  + 窗口 
  + recover
  + TCP 安全性体现在哪些方面，采用了哪些机制？
  + 为什么迅雷是基于UDP，而不是TCP的
 * DNS，HTTPDNS
 * 有哪些方法能加快网络连接速度
 * 拥塞避免算法
 * 浏览器输入网址后的全过程 
 * 发送大文件时客户端和服务端采取了什么机制？描述一下 Nagel 算法？
 * 要实现两台机器及时高效通讯应该怎么做？如何关闭 Nagel 算法？
 * socket 中 SO_REUSEPORT 和 SO_REUSEADDR 的区别？
 * select、epool 的区别？底层的数据结构是什么？
 * HTTP请求的方法和字段
 * ping命令用到了哪些协议
 * 网络通信的多路复用
 * HTTP断点续传
 * HTTP状态码

# 消息队列
 * rmq
 * kafka
 
# 其他
 * 项目当中印象深刻的难点，如何解决
 * 怎么设计微信朋友圈
 * 设置抢单功能，线程安全
 * 有两个TB级大文件，一个文件每行为id : name，另一个文件每行为id : age，要求合并成一个文件id : name, age 
 * Vue, React 双向绑定是如何实现的
 * python 协程
 * 海量日志查找某一段时间内的记录
 * 红黑树和AVL树的区别
 * 短链接算法
 * md5多少位(128bit,32位十六进制)
 * 缓存同步
 * 保证日志上传的幂等性
 * 秒杀场景，分布式锁，分布式事务
 * 一致性hash如何保证负载均衡
