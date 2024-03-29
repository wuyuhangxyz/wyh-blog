---
title: SOAP的概念与主要特点
tags:
  - 网络架构
categories:
  - 网络技术，网络架构
abbrlink: 47245
date: 2022-09-04 15:10:59
---

# 前言

在上一篇文章[HTTP所有方法详解](https://www.wuyuhang.ml/2022/09/03/HTTP%E6%89%80%E6%9C%89%E6%96%B9%E6%B3%95%E8%AF%A6%E8%A7%A3/)当中，我在最后给自己挖了一个坑，说要在下一篇文章里面介绍**SOAP**和**RESTful**，没办法，自己挖的坑怎么都得填上，于是，我写了这篇文章。

我们在开发API或者调用别人的API的过程中，可能经常听到诸如“REST API”这样的名词，而并不知道它是意味着什么，而像**SOAP**这样的名词，平时可能几乎不会接触到，其实，**SOAP**与**REST**是**Web Service**（**Web Service**在百度上面的教程一抓一大把，但是都云里雾里的，我们可以直接理解为Web Service就是通过Web向外提供的API组件）的两种方式。

由于它们的内容稍多，所以我要分好几篇文章来讲，这篇文章主要讲解**SOAP的概念与主要特点**。

# 概述

这里的SOAP可不是肥皂的意思，SOAP指**Simple Object Access Protocol**，即**简单对象访问协议**，是一种基于HTTP和XML的简单网络协议，可使应用程序在 HTTP 之上进行信息交换。简单来说，SOAP就是一种网络协议，用HTTP传输信息，信息的格式是XML。SOAP被发明已经很有一些年头了，它最初就是在HTTP诞生之后，作为一种统一的协议，在计算机之间进行信息交换。

# 特点

- SOAP 是一种*通信协议*
- SOAP 用于*应用程序之间*的通信
- SOAP 是一种用于*发送消息*的格式
- SOAP 被设计用来*通过因特网*进行通信
- SOAP *独立于平台*
- SOAP *独立于语言*
- SOAP *基于 XML*
- SOAP *很简单并可扩展*
- SOAP 允许您*绕过防火墙*
- SOAP 将被作为 *W3C 标准*来发展

# 规范

SOAP最初被开发出来，是为了制定一套通用的信息交换规范，它使用XML作为数据的固定格式，有一套严格的规范和语法规则。它的语法规则如下：

1、SOAP封装（envelop）：它定义了一个框架，描述消息中的内容是什么，是谁发送的，谁应当接受并处理它以及如何处理它们。

2、SOAP编码规则（encoding rules）：它定义了一种序列化的机制，用于表示应用程序需要使用的数据类型的实例。

3、SOAP RPC表示（RPC representation）：它定义了一个协定，用于表示远程过程调用和应答。

4、SOAP绑定（binding）：它定义了SOAP协议使用哪种协议交换信息。使用HTTP/TCP/UDP协议都可以。

可以看到，SOAP的规范是非常严格而完整的，使用XML来表述也使得SOAP可以轻松地跨平台传输。

# 发展史

最初，SOAP的发明是为了取代当时流行的**RPC**协议（我们在该系列的后面会进行讲解），通过Internet来在多个计算机之间传输信息。在当时，SOAP确实是一种非常简单而轻量化的协议，XML的协议也带来了很多的便利。

后来，SOAP越来越多的被用于Web Service，大家为了应对不同的协议和解决方案，为SOAP增加了很多内容，后来，更是有了WS-*这个系列的诞生，增加了SOAP的成熟度，但是SOAP却越来越臃肿了。

后来，随着**JSON**的出现和**REST**的提出，大家都喜欢上了**REST**这种简单优雅的方式，嫌弃SOAP过于臃肿了，所以SOAP就渐渐没落了，现在已经很少见到它，只是一些老牌的企业还在使用。

# 总结

+ SOAP**是一种应用协议，最初为使用Internet传递信息提供了一套完整的范式**
+ SOAP**是跨平台、跨语言的**
+ SOAP**使用XML作为传输数据的结构，可以轻松地进行校验**
+ SOAP**可拓展性强，使得它过于臃肿**
+ SOAP**现在的使用已经不多了**

# 最后

这篇文章是初步讲解了SOAP的概念与特点，其实我也是第一次写关于这种网络协议的内容，也查了很久的资料，希望能够帮到大家吧，如果有错误可以在评论区指出，我会第一时间修改。
