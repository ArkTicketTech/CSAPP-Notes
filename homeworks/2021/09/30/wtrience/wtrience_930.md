***
20210927
# 1
## 1.1 信息是由bit和context组成
系统中的所有信息，包括磁盘文件、存储在内存中的程序、存储在内存中的用户数据和通过网络传输的数据都用一串位表示。区别不同数据对象的唯一东西是我们查看它们的上下文
## 1.2 程序编译的过程 文件转换
预处理器、编译器、汇编器和连接器称为编译系统。
hello.c->hello.i->hello.s->hello.o+printf.o->hello
    processor   compiler    assembler   linker
***
20210928
## 1.3 了解编译系统如何工作
目的：
* 优化程序性能
    * switch\if-else的效率？
    *  指针引用\数组索引的效率？
* 理解链接时的报错
    * 无法解析引用
    * 静态库、动态库
* 避免安全漏洞
    * 缓存区溢出bug
    * 堆栈规则

## 1.4 处理器读取和解释存储在内存中的指令
典型系统的硬件组织。
* CPU:中央处理器
* ALU:算术逻辑单元
* PC:程序计数器
* USB:通用串行总线。


### 1.4.1 系统的硬件组织
* 总线（传输固定大小的字节快）
* 输入输出设备
* 主内存
* 处理器

### 1.4.2 HELLO程序运行过程

## 1.5 缓存问题
**利用缓存内存来提高程序的性能**

## 1.6 存储设备层次结构
***
20210929
## 1.7 操作系统硬件管理
应用程序对硬件的操作需要经过操作系统
1、保护硬件
2、为应用程序提供机制
### 1.7.1 进程
### 1.7.2 线程
一个进程实际上可以由多个被称为线程的执行单元组成
### 1.7.3 虚拟内存
### 1.7.4 文件
## 1.8 系统之间通过网络进行通信
## 1.9 之后所讲的重要思想
* Amdahl法则
* 并发和并行
* 抽象在计算机系统的重要性
***
20210930
# PART I 程序结构与执行
