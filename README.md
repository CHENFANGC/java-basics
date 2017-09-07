# java-basics
Interview points

Unit one 

  part I Java多线程开发
  
    1.基本的锁synchronized, Lock, Condition的用法。ThreadLocal的实现（Map）
    
    2.了解线程池参数意义；知道怎么分析线程异常的情况（例如cpu占用过高，可利用top命令找出线程id，再利用jstack定位stacktrace）
    
    3.了解其他线程同步的类的用法，比如CountdownLatch，Exchanger，Barrier，Semaphore等
    
    4.知道怎么用wait和notify来控制线程同步（java monitor基础）；了解AbstractQueuedSynchronizer原理


  part II JVM
  
    1.jdk6的hotspot堆的结构。了解两个survivor区
    
    2.了解常用GC算法的特点，能讲清楚CMS算法的过程，有根据不同应用程序调优jvm参数的经验（比如对于网络程序，知道调整survivor ratio的大小）
    
    3.熟悉常用GC算法的应用场景及优缺点，能根据不同的需求进行选型
    
    4.了解垃圾回收生命周期，具体可考察Strong, Soft, Weak和Phantom引用的区别，以及都有什么作用（主要区别在于被GC的时间不同。
    
      Soft比Weak更不eager被GC。Weak和Phantom的区别在于入ReferenceQueue的时候不同）；
      
      或者知道线程safepoint，能指出哪些执行语句能达到safepoint


  part III 网络
  
    1.对http 协议有一定熟悉，知道get与post的区别，对http的header常见参数了解一些
    
    2.知道socket的用法。对于nio，知道怎么用socket.select和socket.accept写出一个基本的socket服务（大概伪代码写出来就行）
    
    3.如果用过Netty，能说出netty的基本概念（事件驱动，channel的几种状态，channel pipeline等。如果熟悉netty3，了解boss和worker；
    
      如果熟悉netty4，了解eventloop）；如果没用过netty，说说用过的网络IO框架
      
    4.了解常见io模型：bio，nio，aio,对tcp调优有经验，或者有c100k规模的网络程序的开发经验


  part IV 开源框架相关
  
    1.能说出使用过的开源框架的概念和原理，和一些经验
    
    2.看过开源框架的代码
    
    3.自己有开源框架或者深度参与过


  part V 其他
  
    1.对jdk 源码看过部分类的实现 如String, HashMap等
    
    2.能列举出一些常用的设计模式在生产中的一些应用场景
    
    3.java里类加载的机制（能说出delegate或者双亲委派就行）；了解String pool；Integer -128~128的缓存
    
    4.对java 虚拟机规范以及java 语言特性有深入了解


Unit two

part I 服务器相关

  LINUX
  
    1.熟练使用tail、less等。
    
    2.熟练使用grep、find、sed、awk等基本用法。了解文件权限规则。
    
    3.编写过功能相对复杂的shell 脚本，例如 日志处理，启动shell脚本等

  Redis
  
    1.redis主从部署、持久化、备份、监控等基本运维
    
    2.了解各种存储结构，基本配置参数含义
    
    3.redis数据清理、数据恢复

