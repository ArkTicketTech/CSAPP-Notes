# Ch5 Optimizing Program Performance

本章主要讲程序性能的优化。

编写高效的程序，要求：

1. 选择恰当的数据结构和算法；
2. 理解优化编译器的能力和局限性；
3. 并行的在多核或多处理器上执行。（chapter 12）

程序优化的步骤：

1. 消除不必要的工作，让代码尽可能有效地执行所期望的任务。包括消除不必要的函数调用、条件测试和内存引用等。
2. 利用处理器的指令集并行，同时处理多条指令。例如，降低一个计算的不同部分的数据相关，增加并行度。

