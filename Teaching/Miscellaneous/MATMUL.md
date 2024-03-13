# MATMUL Optimisation
## Background
Matrix multiplication is a fundamental operation in numerous computational and mathematical tasks. This operation is fundamental in many areas, including graphics rendering, scientific simulations, machine learning, and more. Given the significance of matrix multiplication these various fields, failing to implement it with performance in mind can pose a severe computational bottleneck.

A naïve implementation of this algorithm (shown below) exhibits a time complexity of O(n^3) for two n × n matrices. 
``` python
import sys, random
from tqdm import tqdm
from time import *

n = 4096

A = [[random.random()
      for row in range(n)]
      for col in range(n)]

B = [[random.random()
      for row in range(n)]
      for col in range(n)]

C = [[0 for row in range(n)]
     for col in range(n)] 

print("calculating ... \n")

start = time()
for i in tqdm(range(n)):
    for j in range(n):
        for k in range(n):
            C[i][j] += A[i][k] * B[k][j]
end = time()

print("%0.6f"%(end-start))
```
## What do you need to do

Your task is to optimize the above algorithm through any means possible. You can explore various avenues, including switching languages, utilizing compiler flags, parallelizing the code, employing alternative algorithms, any optimization specific to your PC's architecture, or any other method you deem fit to enhance performance. Use the time module to benchmark the optimization process. Try to delve deeper into the optimisations you've employed and understand how they work. You don't have to implement all the above mentioned optimisations by hand. Also don't stick just to the ideas and materials mentioned in this tasks, you can look around on the internet for more ideas. Just make sure you understand how and why everything works.

Additionally, you are required to create a presentation encompassing the following elements, although you are encouraged to expand beyond these:

-   Documentation of your entire process, including the motivation and reasoning behind the steps you followed to optimize the code.
-   Explanation of any new concepts encountered during the optimization process.
-   Demonstration of your understanding of the underlying technology and techniques explored while seeking better optimizations.

## Materials:

[GCC compiler optimisation](https://gcc.gnu.org/onlinedocs/gcc/Optimize-Options.html)
[Vectorisation](https://chryswoods.com/vector_c++/part1.html)
[Cache misses in matmul](https://www.youtube.com/watch?v=5Xc_CzpgSFk)
[More about cache misses](https://dev.to/frosnerd/hit-me-baby-one-more-time---what-are-cache-hits-and-why-should-you-care-4500)
[Verify If you have CUDA compatible GPU](https://docs.nvidia.com/cuda/cuda-installation-guide-microsoft-windows/index.html#verify-you-have-cuda-enabled-system)
[CUDA programming guide](https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html)
[CUDA loop unrolling](https://www.nvidia.com/docs/IO/116711/sc11-unrolling-parallel-loops.pdf)

## Learning from the Task

-   One of the primary and most important skills that you will learn is how to search for information effectively online. While the provided resources give a starting point, they're not all-inclusive. This process also helps in learning how to use official software documentation effectively.
- This task will give you an opportunity to learn how code executes on your computer at a deeper level. The task encourages exploring new concepts beyond the initial codebase. This could include diving into topics such as multi-threading, SIMD instructions, CUDA, memory management, and more.
-   You'll gain insights into optimizing code for smoother execution, delve deeper into GPUs, parallelization, and software performance engineering. It'll feel familiar to anyone who's struggled to run high-demand games on GPUs with limited memory :)
