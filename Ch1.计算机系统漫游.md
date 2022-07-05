

统揽全书的一个章节



* 只由ASCII码（单字节）字符构成的文件称为文本文件，所有其他文件称为二进制文件。源程序实际上就是一个由值 0 和 1 组成的位=二进制位。

  * ? 中文字符是怎么表示的？

* > linux> gee -o hello hello.c

gcc编译器执行4个阶段的程序：

<img src="/Users/dinckham/Library/Application Support/typora-user-images/image-20220704155603381.png" alt="image-20220704155603381" style="zoom: 50%;" />

  * ? Java程序的编译阶段是怎样的？ 其他语言？

* 优化程序性能，提到的几个问题很有意思：

  * 一个switch语句总是比一系列的if-else语句高效得多？
  * 一个函数调用的开销有多大？
  * while循环比for循环更有效吗？
  * 指针引用比数组索引更有效吗？
  * 循环求和的结果放本地变量，会比放一个通过引用传递的参数中，运行为何快很多？
  * 简单重排列下算术表达式中的括号就能让函数运行得更快？

* 典型系统的硬件组成：

  <img src="/Users/dinckham/Library/Application Support/typora-user-images/image-20220705085112183.png" alt="image-20220705085112183" style="zoom:50%;" />

  * 问题：数据从磁盘加载到内存，必须要经过cpu么？DMA？
  * L1、L2、L3等高速缓存的引入，利用了局部性的原理，即程序具有访问局部区域里的数据和代码的趋势。
  * 软硬件之间是操作系统。通过基本的概念抽象（进程、虚拟内存、文件），来向应用程序提供简单一致的机制来控制复杂而不同的低级硬件设备。比如文件是对I/O设备的抽象，虚拟内存是对主存和磁盘I/O设备的抽象，进程则是对cpu、主存等的抽象。

  

* 存储器层次结构：一方面是机械原理，较大的存储设备运转更慢，另外是快速设备的造价更高。

​	<img src="/Users/dinckham/Library/Application Support/typora-user-images/image-20220705093047838.png" alt="image-20220705093047838" style="zoom:50%;" />

* 进程是操作系统对一个正在运行的程序的一种抽象。
* 虚拟内存是一个抽象概念， 它为每个进程提供了一个假象， 即每个进程都在独占地使用主存。

* Amdahl定律：对系统的某个部分加速时，其对系统整体性能的影响取决于该部分的重要性（占比）和加速程度（提升比例）。说明要显著加速整个系统，必须提升全系统中相当大的部分的速度。

​		<img src="/Users/dinckham/Library/Application Support/typora-user-images/image-20220705100248239.png" alt="image-20220705100248239" style="zoom:50%;" />

​	（a表示占比，k表示提升比例）。比如60%占比的部分，提升3倍，整体也就提升（1/(0.4+0.6/3) = 1.67倍。





