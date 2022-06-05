# Parallel Processing Using Nvidia CUDA C Library

## Background

### Parallel Computing:

Parallel computing is a type of computation in which many calculations or processes are carried out simultaneously.Large problems can often be divided into smaller ones, which can then be solved at the same time. There are several different forms of parallel computing: bit-level, instruction-level, data, and task parallelism. Parallelism has long been employed in high-performance computing.Parallel computers can be roughly classified according to the level at which the hardware supports parallelism, with multi-core and multi-processor computers having multiple processing elements within a single machine, while clusters and grids use multiple computers to work on the same task. Specialized parallel computer architectures(Like GPU's) are sometimes used alongside traditional processors, for accelerating specific tasks. 

### Nvidia CUDA C Library :

The Graphics Processing Unit (GPU) provides much higher instruction throughput and memory bandwidth than the CPU within a similar price and power envelope.In general, an application has a mix of parallel parts and sequential parts, so systems are designed with a mix of GPUs and CPUs in order to maximize overall performance. Applications with a high degree of parallelism can exploit this massively parallel nature of the GPU to achieve higher performance than on the CPU.

CUDA (or Compute Unified Device Architecture) is a parallel computing platform and application programming interface (API) that allows software to use certain types of graphics processing units (GPUs) for general purpose processing, an approach called general-purpose computing on GPUs (GPGPU). CUDA is a software layer that gives direct access to the GPU's virtual instruction set and parallel computational elements, for the execution of functions that contain parallel instructions(aka compute kernels).

For Example: adding two vectors A{1 2 3 4} + B{4 3 2 1} = C{5 5 5 5}, In a classic C code using CPU you would iterate through the 
loop and add them sequentially(C[i]=A[i]+B[i]), but using the CUDA C library you can devide each element of a vector into a thread(a thread of execution is the smallest sequence of programmed instructions that can be managed independently) and add the threads together at once in just one instruction cycle like- C[threadIdx.x]= A[threadIdx.x]+B[threadIdx.x]. (Where the the threadIdx corresponds to the index of the thread on GPU and data field(x) is the dimension of the vector)

## What do you need to do

The interviewee needs to make a presentation (keep the presentation simple, a simple PowerPoint presentation is good enough). The interviewee needs to keep in mind that the crowd he will be presenting to, will have mixed people of different knowledge levels, so it is advised that to keep the content balanced for all, explaing the basics along with thorough conceptual insights of the topics mentioned. Your presentation should mainly consist of the following parts.

> - Introduction to types of Parallel Computing(bit-level,instruction-level,data and task parallelism).Basic explaination along with examples (**Not the code** just conceptual examples)
> - Difference between GPU and CPU(hardware level).
> - Install the CUDA Devlopment Kit from this [link](https://developer.nvidia.com/cuda-downloads).
> - Introduction to CUDA Parallel Programming Paradigm. Explaining the following topics.
>    - Compute Kernels
>    - Thread Heirarchy
>    - Memory Heirarchy
>    - functions like `cudaMalloc`, `cudaMemcpy`, `cudaFree` `__syncthreads` and `cudaDeviceSynchronize`
> - Task to be demonstrated using CUDA Programming.

## **Note**: In case you don't have CUDA compatible device use this [google collab doc](https://colab.research.google.com/drive/1Hp6FobU5DDUeqP5cCCZiT7TiyPfGMe1V?usp=sharing) to run your CUDA code


Pease remember to keep the presentation short and concise. Long presentation bores the audience and you will also get tired in presenting. It has also been observed that images, quotes, interactive programming sessions tend to keep the audience interested in the content. **(Recommended: Keep he presentation with 20 slides). Make presentation such that it can be presented within 8-10 mins. Interview should be also prepared for questions regarding the topics being presented by him/her.**

### Task Details

- **Part I**: Print "Hello World on GPU" 1024 times using cuda kernel with 4 blocks and 256 threads and compare the time with a sequential C code to print "Hello World on CPU" 1024 times. Compare the performance wrt time using the C clock function from time library. 

- **Part II**: Add 2 dimensional matrix A and B to result in a new matrix C. The Size of the matrix is 32x32. The elements of the matrix are `A[i][j]=i` and `B[i][j]=j`. Compute this on GPU kernel of size 4 blocks containg 16*16 threads and copy the result on GPU to CPU using cudaMemcpy and print the result on terminal. Compare the performance wrt time again.

## Materials

- https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html
- https://en.wikipedia.org/wiki/Parallel_computing
- [Verify If you have CUDA compatible GPU](https://docs.nvidia.com/cuda/cuda-installation-guide-microsoft-windows/index.html#verify-you-have-cuda-enabled-system) 

## Tech Stack

Prior knowledge of basic C [upto Multidimensional Array] and basic knowledge about computing systems.

## Learning from the Task

- Foremost and major skill that a student will earn is to how to google. Obviously not all person are acquainted with all the technical stuffs and during the making of the presentation, interviewee will learn more about how to google for correct information and gather relevant data properly from the chunk of web pages that google will throw at you on or search query. The resources provided will give you a head start but are not complete resources. Other than that it will help you in learning how to use official documentation of softwares.

- An in depth comparative study will improve your knowledge about computing systems and will provide you surprising insights about using your GPU's other than games :)

- This task will also help you to know in depth about execution of code at hardware level. Dont just try to complete the task by giving definitions and small code demos in ur ppt. Try to understand the difference between running a code on your CPU and running a code on your GPU by doing experiments in your code to understand the CUDA library functions properly. It will help you in the final interview too.

#### For any questions, please reach out to [Aditya Ranjan Jha](mailto:adisofficial.2001@gmail.com)

