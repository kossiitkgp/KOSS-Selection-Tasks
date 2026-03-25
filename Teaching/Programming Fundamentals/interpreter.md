# Interpreted Programming Language

## Background
An interpreter is a program that directly executes instructions written in a programming or scripting language, without requiring them to have been compiled into machine-level code. It reads the source code line by line, translates it, and performs the specified operations immediately, allowing for easier debugging and rapid development.  

## What you need to do

As a part of this task you will have to create your own runtime for a programming language.  
You need to define:  
- A language syntax
- A memory store
- Abstract Syntax Trees
- Bytecode engine (optional)

Example syntax:  

```basic
INPUT "Enter the first number: ", a
INPUT "Enter the second number: ", b
sum = a + b
PRINT "The sum of these numbers is: ", sum
END
```

This example is from the classic language QBasic, which is a begineer-friendly language that uses a "top-down" approach, meaning the computer reads and executes your code line by line.  

### What is an AST?
An Abstract Syntax Tree (AST) is a tree representation of the structure of source code. Each node in the tree represents a construct in the code (like a variable assignment, function call, or operator), and the edges represent the relationships between these constructs. The AST abstracts away syntactic details like parentheses and semicolons, focusing only on the meaningful structure of the program. This makes it easier for interpreters and compilers to analyze and execute the code.  
Consider a statement like the following:  
```py
a = 20
```  
then one appropriate AST could be:  
```py
VariableDeclarationStatement (name = 'a', value = Integer (20))
```
This can be represented as a C struct:
```c
struct VariableDeclarationStatement {
    char *name;
    value_type value;
}
```

## Bytecode Generation (Optional)

Bytecode is a numerical representation of AST.  
ASTs are complex data structures and its computationally expensive working with them.  
Bytecode simplifies logic by providing a linear execution order which:
- is computationally inexpensive to catch.
- is computationally inexpensive to execute.  

Instead of doing a big task, bytecode splits the task into smaller tasks that do not involve extensive use of data structures.  
For learning more about bytecode, you can refer the following resources:
- [Medium: The Life of a Bytecode Language by Better Programming](https://medium.com/better-programming/the-life-of-a-bytecode-language-fca666928e7b)
- [Medium: What Do we Know about ByteCode by Vikas Taank](https://medium.com/@vikas.taank_40391/what-do-we-know-about-bytecode-283a00f69e97)
- [Writing a compiler. Bytecode basics](https://www.youtube.com/watch?v=ZID0IJiOJdE)

The task should implement either AST generation and execution of the AST, or Bytecode generation from AST and execution of said bytecode.  
> [!TIP]
> As this is task involves some coding, you are encouraged to use version control
> and make your project open-source. You are free to use any programming language you like.

Please create a basic implementation of the language along with a presentation, either using PPT or preferably an Open Source
tool such as [RevealJS](https://revealjs.com/). The interviewee needs to keep
in mind that the crowd he will be presenting to, will have mixed people of
different knowledge levels, so it is advised to keep the content balanced
for all rather than becoming very technical.

## Resources

To help you build your interpreter, here are some excellent resources:

- **[Crafting Interpreters](https://www.craftinginterpreters.com/contents.html)** - A comprehensive guide covering language design, lexing, parsing, and execution with practical examples.
- **[Let's Build a Simple Interpreter](https://ruslanspivak.com/lsbasi-part1/) by Ruslan Spivak** - A detailed series that walks through building an interpreter step-by-step from scratch.
- **[Build Your Own X](https://github.com/codecrafters-io/build-your-own-x?tab=readme-ov-file#build-your-own-programming-language)** - A curated collection of projects including building programming languages with community implementations.

These resources provide different approaches and perspectives, from theoretical foundations to practical implementations. We recommend starting with one that matches your learning style—whether you prefer narrative tutorials or hands-on project-based learning.


## Learning from the Task

Completing this task will help you gain practical experience in several key areas of computer science and software engineering:

- **Language Design:** You'll learn how to define the syntax and semantics of a programming language, making decisions about how code should be structured and interpreted.
- **Parsing and AST Construction:** You'll understand how to convert source code into an Abstract Syntax Tree (AST), which is a fundamental concept in compilers and interpreters.
- **Interpreter Implementation:** You'll gain hands-on experience in building an interpreter that can execute code by traversing the AST or by running bytecode on a virtual machine.
- **Memory Management:** You'll explore how variables and values are stored and managed during program execution.
- **Error Handling:** You'll learn how to detect and report errors in user code, an essential skill for building robust software.
- **Software Architecture:** You'll practice structuring your codebase for clarity and extensibility, which is crucial for larger projects.
- **Presentation Skills:** By preparing a presentation, you'll develop the ability to communicate technical concepts to audiences with varying levels of expertise.

This task provides a strong foundation for understanding how programming languages work under the hood, and will be valuable for anyone interested in compilers, interpreters, or language design.