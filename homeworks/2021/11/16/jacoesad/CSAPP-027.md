> ***2021.11.16\***

------

### 3.5.4 Discussion

通常编译器产生的代码中，会用一个寄存器存放多个程序值，并且会在寄存器之间传送程序值。

### 3.5.5 Special Arithmetic Operations

16字节成为八字（oct word）。

[特殊算数操作](https://www.notion.so/df216ad0c5314b9f8603da0dc68e89f9)

`imulq`和`mulq`两个指令，要求一个参数必须在寄存器`%rax`中，另一个作为指令源操作数给出。乘积存放在`%rdx`（高64位）和`%rax`（低64位）中。

除法类似，将寄存器`%rdx`（高64位）和`%rax`（低64位）中的128位作为被除数，除数作为指令的操作数给出。将商存储在`%rax`中，将余数存储在`%rdx`中。