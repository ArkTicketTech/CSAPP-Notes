文件：

**普通文件**

**目录**：包含了一组**链接**的文件，每一个链接把一个文件名映射到一个文件。

套接字：用来和另一个进程进行跨网络通讯的文件

命名管道

符号链接

等类型

## 网络编程

C/S模型中的基本操作是事务（指的不是数据库事务）

1. 客户端需要服务时候 向服务器发起一个请求 发起一个事务
2. 服务器收到请求之后 工作
3. 服务器给客户端发送一个响应 并等待下一个请求
4. 客户端收到响应并处理

**注意：客户端和服务器是进程，而不是机器**

