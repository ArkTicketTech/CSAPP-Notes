碎片化：

造成堆空间利用率低的原因是碎片现象。

内部碎片：分配了大小是512B的块 但是块内只有10B的一个数据存放

外部碎片：分配模式是001001001的时候有三个Byte可用 但如果我们请求3B的连续内存 那么无法满足

解决方法：使用启发式策略来维持少量的大空闲块 而不是大量的小空闲块

