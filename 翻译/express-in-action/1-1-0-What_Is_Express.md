# 第1章 Express是什么？


这个章节包括


> - Node.js, 是一个典型的用来在服务端运行JavaScript的平台 
> - Express，是一个位于Node.js web服务端最上层的框架，使得Node.js更简单易用 
> - Express 的两个特性，中间件（Middleware） 和 路由（routing）
> - 请求处理函数




在我们谈论Express之前呢，我们需要先谈谈Node.js。


JavaScript编程语言生命里的大部分时间，是生活在web浏览器中的。它由一个修改web页面细节的简单脚本语言开始，却成长为拥有大量应用程序和库的复杂语言。许多浏览器厂商，像谋智（Mozilla）和谷歌（Google）开始为了快速的JavaScript运行环境而投入资源，最终浏览器获得了更快JavaScript引擎。

在2009年，Node.js诞生了。Node.js带着V8--Google Chrome浏览器的强大的JavaScript引擎，脱离了浏览器，而且使它能够运行在服务端。在浏览器端，开发者们除了JavaScript别无选择。开发者们在开发服务端项目时，除了Ruby
，Python， C#，Java现在还能选择JavaScript。


JavaScript可能不是每个人最精通的语言，但Node.js有实实在在的优势。首先，V8 JavaScript引擎非常快，且Node.js鼓励异步编程风格，在避免多线程噩梦的同时也让代码更快。JavaScript因为它的流行，也有一大堆有用的库。但Node.js最大的优点是在浏览器和服务器之间共享代码的能力。当（分别）在浏览器端和服务器端（开发）时，开发者们不需要切换任何环境。现在他们可以在这两个JavaScript运行环境之间使用相同的代码以及编写相同的案例：浏览器和服务器。


Node.js很流行--因为人们认为它相当酷。就像基于浏览器的JavaScript一样，Node.js提供了一系列你构建应用程序时所需要的低级特性。但就像基于浏览器的JavaScript一样，它所提供的低级产品繁琐且难用。


进入Express, 它是一个框架，就像在Node.js web服务层上的光层，使得node.js在开发web应用程序的时候更加舒适


Express在哲学层面很像jQuery。人们想要往他们的页面里添加动态的内容，但原生浏览器的API可能繁琐、混乱、而且特性很有限。开发者不得不经常写很多样板代码。jQuery的存在是为了减掉这些样板代码，通过简化浏览器的API并且加入一些有用的新特性。基本上就是这样。


Express也完全一样。人们想要用Node.js来开发一个web应用，但原生Node.js的API可能繁琐、混乱、而且特性很有限。开发者不得不经常写很多样板代码。Express的存在是为了减掉这些样板代码，通过简化Node.js的API并且加入一些有用的新特性。基本上就是这样!


就像jQuery一样，Express目的是可扩展。它不干涉你应用的大部分决策，并且很容易扩展第三方库。在这整本书和你的Express生涯中，你必须对你的应用架构做决策，而且你将通过许多强大的第三方模块来扩展你的Express


然而，你可能还未能对这本书做一个“简短”的定义。在这个章节（以及这本书，是真的）的剩余部分将深入的讨论Express


**注意** 这本书假设你已经精通JavaScript，而不是Node.js

------
[上一页](1-0-0-Part1_Intro.md)

[下一页](1-1-1-What_is_this_Nodejs_business.md)