# The Inner Workings of Compilers

## Background

A compiler is a type of software tool that takes code written in a high-level programming language and converts it into binary code that a computer can execute. This conversion process happens in multiple stages, each of which is important for turning human-readable code into instructions that computers can understand. Knowing how a compiler works can help programmers write code that runs more efficiently. 

C, C++, Go, Rust, etc. are examples of compiled languages. The gnu compiler collection (GCC) is used to compile C/C++ programmes. Python, javascript, perl are interpreted languages. 

## Task Description

- Research the inner workings of compilers and interpreters to understand their fundamental differences, delving into their unique strengths and weaknesses
- Try to understand how these programs translate high-level, human-readable code into machine code, exploring the intricacies of the conversion process
- Discuss the various challenges encountered during the development of compilers and interpreters, such as addressing platform independence through the use of intermediate representation and handling hardware specific optimisations across different architectures
- Explore advanced optimisation techniques utilised by compiler engineers, such as dead code elimination, loop optimisation, and register allocation, to improve the efficiency and performance of generated machine code
- Use a disassembler to compare the compiled assembly code to higher level code to show how a compiler optimises for allocating more memory in registers instead of the memory
- Create a detailed presentation documenting the learning journey throughout the task, incorporating explanations along with relevant code snippets to illustrate practical applications and key concepts
- Optionally you can write a simple compiler for an already existing language or design your own language :P


## Key Takeaways

Upon completing this task, you will acquire a deep insight into the intricate process of compiler construction, significantly expanding your expertise in low-level development. This will particularly enrich your understanding of optimising code for enhanced performance and navigating challenges related to hardware independence. 

## Resources

- [Crafting interpreters](https://craftinginterpreters.com/contents.html)
- [An introduction to compilers](https://nicoleorchard.com/blog/compilers/)
- [Optimisations in C++ compilers](https://queue.acm.org/detail.cfm?id=3372264)
- [LLVM Tutorials](https://llvm.org/docs/tutorial/)
- [Numba, a python JIT](http://numba.pydata.org/)
- [A jit compiler for x86 in 86 lines](https://github.com/EarlGray/c4)
