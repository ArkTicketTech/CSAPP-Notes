select函数处理类型为`fd_set`的集合 用位向量表示

IO多路复用可以用作并发事件驱动程序的基础。把逻辑流模型化为状态机。

服务器借助IO多路复用 使用select函数检测输入事件的发生 当每一个已连接的描述符准备好可读的时候 就为相应的状态机执行转移

node.js nginx 都用的是IO多路复用的事件驱动的编程方式 因为有性能优势
