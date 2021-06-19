# Async Await in Python

**NOTE: Use Python3.8 and above**

This task, enlists the async await feature in Python.

This task contains three parts of subtasks that needs to be completed for implementing Async Await in Python.

## Background:

Python provides parallel programming using threads and multiprocessing. However, due to Global Interpreter Lock, Python cannot provide parallelism similar to what multi-threading works in other languages, such as Java/C++.

Effectively, only one thread runs at a time, while others are waiting for GIL to be released, so ultimately, we are running in a synchronous manner for **Python**.

In order to tackle that, different languages have provided language constructs for running the different blocking process concurrently.

For example, in JavaScript we use concepts of Promise, and in Python, it provides Async/Await - Asyncio. So it uses the concurrency paradigm.

## What do you need to do:

- Task 1 - Create a 3 coroutines for execution and see if you can parallelise the execution.

    <details>
    <summary>Details about Task</summary>

    ```python
    import asyncio
    import time

    async def sleep_coro(duration):
        await asyncio.sleep(duration)

    async def main():
        obj1 = sleep_coro(1)
        obj2 = sleep_coro(2)
        obj3 = sleep_coro(3)
        
        # See that the three object would execute synchronously, 
        # so it will take 1 + 2 + 3 seconds to execute.
        start = time.time()

        await obj1
        await obj2
        await obj3

        time_taken = time.time() - start
        print('Time Taken {0}'.format(time_taken))

    asyncio.run(main())
    ```  
    </details>

    Now google and find how you would parallelise the execution of task.
    <details>
    <summary>Solution to Task 1</summary>

    ```python
    import asyncio
    import time


    async def sleep_coro(duration):
        await asyncio.sleep(duration)


    async def main():
        obj1 = sleep_coro(1)
        obj2 = sleep_coro(2)
        obj3 = sleep_coro(3)

        # See that the three object would execute synchronously,
        # so it will take max(1, 2, 3) seconds to execute.
        start = time.time()

        await asyncio.gather(obj1, obj2, obj3)

        time_taken = time.time() - start
        print('Time Taken {0}'.format(time_taken))

    asyncio.run(main())
    ```  
    </details>

    Task for the above part - Now replace the `sleep_coro` with a function that would download a page from `https://www.google.com/search?q={name_arr}` where `name_arr = ['Yash', 'KOSS', 'Your Name']` 

    Use this resource for more details for downloading a page - https://docs.aiohttp.org/en/stable/#client-example


* <details>
    <summary>Task 2</summary>

    Task 2 - Write up a script to download the JSON file for the URL - `https://xkcd.com/{comic_id}/info.0.json`, where the `comic_id` is a natural number from `1 - 200`. Download the json response and save it in a file. Do it in a synchronous manner, something like this - 

    ```python
    for i in range(1, 201):
    # pseudo code
    # download response
    # create a file with a unique name
    # paste the json contents in the file
    ```

    Now, using Async/Await, try to parallelise the downloading of files, so that you can accelerate the execution.

    Record the time taken, and compare the time difference of execution.

    </details>


## Materials:

* https://realpython.com/async-io-python/
* https://docs.python.org/3/library/asyncio.html
* https://docs.aiohttp.org/en/stable/#client-example

## Tech Stack:
* Asyncio, Async/Await in Python, AioHttp

## Learning from the Task:
* From this task, you will learn that how Asyncio achieves concurrency in Python.