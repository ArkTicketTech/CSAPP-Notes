# Ch1

Status: Completed

1.1 信息就是位+上下文

个人理解： 代码也好， 文本也好， 视频也好， 在计算机内都是二进制存储和表示的。 如何区分他们，最大的不同就是，如何对这些二进制位进行解释。   按照8位一个字节可以将这些二进制转换成字母， 这就是ascii。  三个或四个字节一组，将其中的二进制位转换， 这个可以是UTF-8。 或者我们也可以自己定义转换方式， 这个就是原文中说的上下文的含义， 说到底，如何对字节序列进行编解码，不同的编解码方式，造就了丰富多彩的世界。

1.2, 1.3 程序的编译流程

.c 文件 —> 预处理 —> compile 出 .s 文件 —> 汇编器转换成 .o文件 —> 链接器 —> 可执行程序

此处细节可以参考 程序员修养, 链接、装载那本书

1.4 系统硬件组成

- cpu  核心组件，计算通路和控制通路
- 总线 数据传输
- io 设备，  磁盘，外设都属于io
- 内存

Amdahl’s Law

The main idea is that when we speed up one part of a system, the effect on the overall system performance depends on both how significant this part was and how much it speed up

Tnew = (1-a)Told + aTold 

S =  1 / ((1-a) + a/k)