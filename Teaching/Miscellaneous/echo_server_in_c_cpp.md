# Event Loop

## Background

A good server (web server, ssh server, ftp server, etc.) must be able to handle multiple clients at the same time. It must also do this with less performance impact and higher throughput. There has been many ways to do this, but the most common way is to use a single thread to handle all requests. This is not a good way to do it, because it will block the rest of the requests from being handled. This is where the **asynchronous IO** comes in.

There are many ways to acheive asynchronous I/O, but the most common way is to use the **event loop**. The event loop is a way to handle multiple requests at the same time. It is a way to handle multiple clients at the same time.

## Task

Create a presentation about and teach the audience about the following:
- Different types of I/O : Synchronous and Asynchronous
- Talk in detail about event driven I/O and event loop
- Research and talk about the use of the event loop  in nodejs


## Relevant Materials

[https://nodejs.dev/learn/the-nodejs-event-loop](https://nodejs.dev/learn/the-nodejs-event-loop)
[https://heynode.com/tutorial/explore-io-callbacks-phase-nodejs-event-loop/](https://heynode.com/tutorial/explore-io-callbacks-phase-nodejs-event-loop/)