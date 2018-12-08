# DB
+ ##  redis 
  - 设计与实现，如果redis有一亿个key,使用keys命令是否会影响线上服务（会，因为是单线程模型，可以部署多个节点）
  - 持久化方式：aod and rdb，怎么实现
  - list怎么实现（ziplist压缩空间 and quicklist实现链表）
  - sorted set怎么实现（dict+skiplist）
  - skiplist数据结构，实现
  
+ ## MYSQL 
  - 索引(innodb, b+ tree, 为什么用b+树做索引节点，一个节点存了多少数据，怎么规定大小，与磁盘页对应)
  - 调优
  - 分库分表
  - 事务隔离级别
  - mongo ？
  - spark ?

# Java
 + 多线程 concurrenthashmap countdownlatch
 + Java集合类哪些是线程安全的
 + 集合类，hashmap怎么实现的

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


# operating system
 * linux 磁盘管理
 * linux 进程间通信方式 5
 * linux 共享内存如何实现
 * cgroup 在linux具体实现
 * 僵尸进程，孤儿进程(如何避免僵尸进程，父进程怎么知道子进程结束)
 * 进程死锁
 * 实现LRU cache（超时淘汰，LRU淘汰） linkedlist 和 hashmap实现
 * 内存管理

# 虚拟化
 * docker 物理机 虚拟机 部署 实现
 * k8 ?

# 网络
 * TCP 三次握手,不要第三次握手行不行，被黑客利用，对服务器DDos攻击：https://www.jianshu.com/p/1c65840fc02d 四次挥手，窗口，recoverm,三次握手
 * 为什么迅雷是基于udp，而不是tcp的
 * DNS，HTTPDNS
 * 有哪些方法能加快网络连接速度
 * 拥塞避免算法

# 消息队列
 * rmq
 * kafka
# 其他
 * 项目当中印象深刻的难点，如何解决

