# 1.2 What is Express?

Express is a relatively small framework that sits on top of Node.js’s web server functionality to simplify its APIs and add helpful new features. It makes it easier to organize your application’s functionality with middleware and routing; it adds helpful
utilities to Node.js’s HTTP objects; it facilitates the rendering of dynamic HTML views;
it defines an easily implemented extensibility standard. This book explores those features in a lot more depth, so all of that lingo will be demystified soon.

### 1.2.1 The functionality in Node.js
When you’re creating a web application (to be more precise, a web server) in
Node.js, you write a single JavaScript function for your entire application. This function listens to a web browser’s requests, or the requests from a mobile application
consuming your API, or any other client talking to your server. When a request
comes in, this function will look at the request and determine how to respond. If you
visit the homepage in a web browser, for example, this function could determine
that you want the homepage and it will send back some HTML. If you send a message
to an API endpoint, this function could determine what you want and respond with
JSON (for example).

Imagine you’re writing a web application that tells users the time and time zone on
the server. It will work like this:
■ If the client requests the homepage, your application will return an HTML page
showing the time.
■ If the client requests anything else, your application will return an HTTP 404
“Not Found” error and some accompanying text.
If you were building your application on top of Node.js without Express, a client hitting your server might look like figure 1.2

![Figure1.2](image/Figure1.2.png)



The JavaScript function that processes browser requests in your application is called a
request handler. There’s nothing too special about this; it’s a JavaScript function that
takes the request, figures out what to do, and responds. Node.js’s HTTP server handles
the connection between the client and your JavaScript function so that you don’t have
to handle tricky network protocols.


In code, it’s a function that takes two arguments: an object that represents the
request and an object that represents the response. In your time/time zone application, the request handler function might check for the URL that the client is requesting. If they’re requesting the homepage, the request handler function should respond
with the current time in an HTML page. Otherwise, it should respond with a 404.
Every Node.js application is just like this: it’s a single request handler function
responding to requests. Conceptually, it’s pretty simple.


The problem is that the Node.js APIs can get complex. Want to send a single JPEG
file? That’ll be about 45 lines of code. Want to create reusable HTML templates? Figure out how to do it yourself. Node.js’s HTTP server is powerful, but it’s missing a lot
of features that you might want if you were building a real application.


Express was born to make it easier to write web applications with Node.js.


### 1.2.2 What Express adds to Node.js

In broad strokes, Express adds two big features to the Node.js HTTP server:
■ It adds a number of helpful conveniences to Node.js’s HTTP server, abstracting
away a lot of its complexity. For example, sending a single JPEG file is fairly complex in raw Node.js (especially if you have performance in mind); Express
reduces it to one line.
■ It lets you refactor one monolithic request handler function into many smaller
request handlers that handle only specific bits and pieces. This is more maintainable and more modular.
In contrast to figure 1.2, figure 1.3 shows how a request would flow through an Express
application

![Figure1.3](image/Figure1.3.png)

Figure 1.3 might look more complicated, but it’s much simpler for you as the developer. There are essentially two things going on here:

■ Rather than one large request handler function, Express has you writing
many smaller functions (many of which can be third-party functions and not
written by you). Some functions are executed for every request (for example,
a function that logs all requests), and other functions are only executed sometimes (for example, a function that handles only the homepage or the 404
page). Express has many utilities for partitioning these smaller request handler functions.

■ Request handler functions take two arguments: the request and the response.
Node’s HTTP server provides some functionality; for example, Node.js’s HTTP
server lets you extract the browser’s user agent in one of its variables. Express
augments this by adding extra features such as easy access to the incoming
request’s IP address and improved parsing of URLs. The response object also
gets beefed up; Express adds things like the sendFile method, a one-line command that translates to about 45 lines of complicated file code. This makes it
easier to write these request handler functions.

Instead of managing one monolithic request handler function with verbose Node.js
APIs, you write multiple small request handler functions that are made more pleasant
by Express and its easier APIs

------
[上一页](1-1-1-What_is_this_Nodejs_business.md)

[下一页]()