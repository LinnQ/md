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


Node.js caught on—people thought it was pretty cool. Like browser-based JavaScript,
Node.js provides a bevy of low-level features you’d need to build an application. But
like browser-based JavaScript, its low-level offerings can be verbose and difficult to use.


Enter Express, a framework that acts as a light layer atop the Node.js web server,
making it more pleasant to develop Node.js web applications.


Express is philosophically similar to jQuery. People want to add dynamic content
to their web pages, but the vanilla browser APIs can be verbose, confusing, and limited
in features. Developers often have to write boilerplate code, and a lot of it. jQuery
exists to cut down on this boilerplate code by simplifying the APIs of the browser and
adding helpful new features. That’s basically it.


Express is exactly the same. People want to make web applications with Node.js,
but the vanilla Node.js APIs can be verbose, confusing, and limited in features. Developers often have to write a lot of boilerplate code. Express exists to cut down on this
boilerplate code by simplifying the APIs of Node.js and adding helpful new features.
That’s basically it!


Like jQuery, Express aims to be extensible. It’s hands-off about most parts of your
applications’ decisions and is easily extended with third-party libraries. Throughout this
book and your Express career, you’ll have to make decisions about your applications’
architectures, and you’ll extend Express with a bevy of powerful third-party modules.


You probably didn’t pick up this book for the “in short” definition, though. The
rest of this chapter (and book, really) will discuss Express in much more depth.


NOTE This book assumes that you’re proficient in JavaScript but not Node.js.

------
[上一页](1-0-0-Part1_Intro.md)

[下一页](1-1-1-What_is_this_Nodejs_business.md)