# Async Await in Python

**NOTE: Use Python3.8 and above**

This task, enlists the async await feature in Python.

## Background:

Python provides parallel programming using threads and multiprocessing. However, due to Global Interpreter Lock, Python cannot provide parallelism similar to what multi-threading works in other languages, such as Java/C++.

Effectively, only one thread runs at a time, while others are waiting for GIL to be released, so ultimately, we are running in a synchronous manner for **Python**.

In order to tackle that, different languages have provided language constructs for running the different blocking process concurrently.

For example, in JavaScript we use concepts of Promise, and in Python, it provides Async/Await - Asyncio. So it uses the concurrency paradigm.

## What do you need to do:

- You need to create a presentation highlighting how python tackles the problem of locked threading with its concurrency paradigm to provide added performance using multiple threads

- Provide some example use cases of this functionality 

- Write some example code snippets and try to parallelise its execution.Benchmark it and note the performance gains (use a time library to calculate execution time or an IDE)

- Try to incorporate a function that takes a significant amount of time to execute and note the performance gains from a parallelized solution  
  
- Focus on understanding how python implements multi-threading differently from other languages like golang and C++

## Materials:  

* https://realpython.com/async-io-python/

* https://docs.python.org/3/library/asyncio.html

* https://docs.aiohttp.org/en/stable/#client-example

## Tech Stack:

* Asyncio, Async/Await in Python, AioHttp

## Learning from the Task:

- Upon completion of this task you will learn about synchronous and asynchronous programming
- How python uses multiple threads of the process to achieve better performance
- Applications of asynchronous programming in real world applications
- How multi-threaded processors are now being used to achieve even higher performance in certain kinds of computational operations  
