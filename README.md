# 第一章
## 操作系统的基本特性

### 并行与并发
* 并行性：多项事件在同一 **时刻** 发生
* 并发性：多项事件在同一 **时间间隔内** 发生

### 资源共享
* 互斥资源共享：某些资源可以同时供多个进程使用，但**同一时间段**只能有一个进程使用，比如音响、打印机等。
* 同时访问共享：在**同一时间段**虽然可以有多个进程同时使用（比如硬盘），但在微观上（精确到毫秒级），这些进程对资源的访问仍然是交替进行的，即某一瞬间，仍是只能有一个进程访问。
  * *一个打电话的房间，互斥资源共享只能有一个人在房间打电话，但是同时访问共享，大家都可以在房间里，不过要排队打电话*

### 虚拟
类似把信道通过复用技术划分成数个虚拟信道，计算机网络学过了
* 时分复用技术：资源在时间上进行复用，不同程序并发使用，多道程序分时使用计算机的硬件资源，提高资源的利用率。
* 空分复用技术：用来实现虚拟磁盘（物理磁盘虚拟为逻辑磁盘，电脑上的C盘、D盘等）、虚拟内存（在逻辑上扩大程序的存储容量）等，提高资源的利用率，提高编程效率。

### 异步
通俗来说：就是十几年前，人们想打电话不是随时能打的，而是要去电话亭才能打，如果手上有活或者电话亭有人，都没办法马上打，而且你也不知道电话亭里的人什么时候打完，你得一直等。那么，由于资源等因素的限制，是的进程的执行不是一气呵成，而是断断续续的，未知的。换句话说，就是以人们不可预知的速度向前推进的，此即进程的异步性。

