# I/O

## Background

A good server (web server, ssh server, ftp server, etc.) must be able to handle multiple clients at the same time. It must also do this with less performance impact and higher throughput. There has been many ways to do this, but the most common way is to use a single thread to handle all requests. This is not a good way to do it, because it will block the rest of the requests from being handled. This is where the **non-blocking IO** comes in.

There are many ways to acheive non-bloccking I/O, but the most common way is to use the **event loop**. The event loop is a way to handle multiple requests at the same time. It is a way to handle multiple clients at the same time.

## Task

Create a short presentationand teach the audience about the following:
- Different types of I/O : Blocking and Non-blocking ( Note: This is different from synchronous and asynchronous I/O)
- Present about event driven I/O and event loop
- Present about the use of the event loop  in nodejs (just the basic overview)
- Refer to the resources and create a basic presentation. It may not be in great detail, but it should be a good overview.

## Relevant Materials

[https://nodejs.org/en/docs/guides/blocking-vs-non-blocking/](https://nodejs.org/en/docs/guides/blocking-vs-non-blocking/) \
[https://www.geeksforgeeks.org/how-the-single-threaded-non-blocking-io-model-works-in-nodejs/](https://www.geeksforgeeks.org/how-the-single-threaded-non-blocking-io-model-works-in-nodejs/) \
[https://nodejs.dev/learn/the-nodejs-event-loop](https://nodejs.dev/learn/the-nodejs-event-loop) \
[https://heynode.com/tutorial/explore-io-callbacks-phase-nodejs-event-loop/](https://heynode.com/tutorial/explore-io-callbacks-phase-nodejs-event-loop/) \
[https://medium.com/@abshirj05/what-does-event-driven-and-non-blocking-i-o-mean-57ac4f54288e](https://medium.com/@abshirj05/what-does-event-driven-and-non-blocking-i-o-mean-57ac4f54288e) \
[https://developers.redhat.com/blog/2016/08/16/why-should-i-use-node-js-the-non-blocking-event-io-framework](https://developers.redhat.com/blog/2016/08/16/why-should-i-use-node-js-the-non-blocking-event-io-framework)