LINUX X86-64中的异常

0-31是Intel架构师定义的异常

32-255是操作系统定义的中断和陷阱

异常号：

0 除法错误

13 一般保护故障

14 缺页

18 机器检查

系统调用：每一个系统调用有一个唯一的整数号 对应于一个到内核中跳转表的偏移量（跳转表不等于异常表）



syscall指令用来进行系统调用

参数通过寄存器传递

%rax为系统调用号 其他寄存器存放参数