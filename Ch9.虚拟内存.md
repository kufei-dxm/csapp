##### 感悟

* 硬着头皮读了一些章节，操作系统真是最牛逼的系统软件，是对数据结构和算法的最精妙的应用，处处体现着对性能的极致要求。也难怪数据结构、算法是计算机的基础了。（书中举了很多系统调用的实现原理和代码，无一不透露着数据结构的巧妙设计）
* csapp要细读理解，难度不小。不过看完后，再去看其他的技术文章，发现难度都变小了 ^_^。所以，专业基础知识，再难都要啃下来，修炼好内功，再练其他外功可触类旁通。



##### 疑惑

* ？ 虚拟内存怎么会在磁盘上？
* Java代码中new创建新的对象，和虚拟内存的关系是？



##### 摘记

* 虚拟内存提供了三个重 要的能力：=> 提供一种抽象
  * 将虚拟内存看成是一个存储在磁盘上的地址空间的高速缓存，在主存中只保存活动区域， 并根据需要在磁盘和主存之间来回传送数据， 通过这种方式，它高效地使用了主存。=> 把虚拟内存看成存储在磁盘上的数据的DRAM缓存。（这里有点难以理解）
    * 概念上，虚拟内存可以视为存储在磁盘上的字节序列；存储在磁盘上的虚拟内存的内容缓存在主存中。
  * 为每个进程提供了一致的地址空间， 从而简化了内存管理。
  * 它保护了每个进程的地址空间不被其他 进程破坏。

* 操作系统为每个进程提供了一个独立的页表（内存中的一个数据结构），因而也就是一个独立的虚拟地址空间。多个虚拟页面可以映射到同一个共享物理页面上。
* 通常，虚拟地址空间比物理地址空间大得多。？？

