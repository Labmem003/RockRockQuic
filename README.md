# RockRockQuic
Quic协议 [介绍、资料与文档汇总+英文资料翻译、落地使用、源码解析] 。目前关于quic的中文资料文档比较少，希望此 Repository 能起到一定的补充作用。

**介绍**，会尽量用浅显的词语介绍 Quic 的背景、概念和什么时候为什么适合使用Quic。    
**资料与文档汇总+英文资料翻译**，其实就是把我看过的有价值的资料汇总起来，如果是英文的就顺便翻译。这个章节应该会随着我的阅读经历不断更新。  
**基本应用**，会教你跑起 Google 官方的玩具例子（Toy Client & Server）。从这个小节开始（还有资料小节的某些文章），需要有C++基础。如果你还不懂C++，自荐下根据我自身入门经验总结的资料：[小白 C++ 入门并发疯学习路线(书单)](https://juejin.im/post/5bb08fc8e51d450e62380e5b)。   
**源码解析**，以上一节的玩具例子为入口，曲径通幽、循序渐进地解析代码。  
**Client端工程化应用**，主要是介绍将 Chromium 内成熟源码搞出来独立应用。关于工程化的成熟应用，我也才接触，造诣不深，欢迎小伙伴来交流见解。  

你可以随时反馈意见或建议，以改进这篇文档。

## 介绍
**快速科普：**  
Quic 全称 quick udp internet connection [1]，“快速 UDP 互联网连接”，（和英文 quick 谐音，简称“快”）是由 Google 提出的使用 udp 进行的可靠的多路并发传输的协议。  
总的来说，Quic 的核心特性可概括为用 UDP 去除握手延迟的0RTT建连特性；再在应用程序层面实现 TCP 的可靠性，TLS 的安全性和 HTTP2 的并发性。
此外，还拥有改进的可插拔灵活拥塞控制、不同精细度级别（具体的每条流 和 整体的连接）的流量控制、避免队头阻塞的多路复用、连接迁移（网络制式的变化也不必重建连接）、前向冗余纠错等独特新特性。  
Quic的发明，是由于TCP有缺陷，TCP 要改进，但不方便改，新增一个协议又不被已有的设备支持，唯一的方案就是使用 UDP 作为底层协议，在 UDP 之上实现数据可达性。

**详细的背景和理念科普：**   
[QUIC 协议概述](https://github.com/bestswifter/blog/blob/master/articles/quic.md)  
[技术扫盲：新一代基于UDP的低延时网络传输层协议——QUIC详解](http://www.52im.net/forum.php?mod=viewthread&tid=1309)  
[Google QUIC协议：从TCP到UDP的Web平台](http://www.infoq.com/cn/articles/quic-google-protocol-web-platform-from-tcp-to-udp) 


## 资料汇总+英文资料翻译


Todo...(Coming later)

## 基本应用
Todo...

## 源码解析
Todo...

## 工程化应用
Todo...

## Q&A
Todo...
