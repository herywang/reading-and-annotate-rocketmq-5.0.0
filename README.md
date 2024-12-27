# RocketMQ 源码阅读笔记记录
rocket client包括两种方式：rocketmq自带的rocketmq-client和rocketmq-clients/rocketmq-client-java。
其中rocketmq自带的client是通过remoting协议进行通信，而rocketmq-clients/rocketmq-client-java是全新封装的gRPC协议进行通信。支持多种语言。
本文中我么将从rocket自带的rocketmq-client入手，进行源码阅读。后续有时间将会继续分析基于rocketmq-client-java进行分析。
## 目录

- [1.创建一个生产者的流程](./docs/1.%20生产者如何将消息发送到rocket%20server%3F.md)