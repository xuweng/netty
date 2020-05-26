# 资源

https://waylau.gitbooks.io/essential-netty-in-action/GETTING%20STARTED/Asynchronous%20and%20Event%20Driven.html

重点

    Selector Java 的无阻塞 I/O 实现的关键

    Selector 最终决定哪一组注册的 socket 准备执行 I/O
    
    Channel 是 NIO 基本的结构
    
    Netty 的异步编程模型是建立在 future 和 callback 的概念上的
    
    Netty 通过触发事件从应用程序中抽象出 Selector，从而避免手写调度代码。EventLoop 分配给每个 Channel 来处理所有的事件

重点2

    Netty 实现的 echo 服务器都需要下面这些：
    
    一个服务器 handler：这个组件实现了服务器的业务逻辑，决定了连接创建后和接收到信息后该如何处理
    
    Bootstrapping： 这个是配置服务器的启动代码。最少需要设置服务器绑定的端口，用来监听连接请求

总结

    在本章中，您构建并运行你的第一 个Netty 的客户端和服务器。虽然这是一个简单的应用程序，它可以扩展到几千个并发连接。