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

## Example: AST Breakdown

Here's a simple Abstract Syntax Tree (AST) representation for the QBasic code above:

```
Program
├── InputStatement(prompt="Enter the first number: ", variable="a")
├── InputStatement(prompt="Enter the second number: ", variable="b")
├── AssignmentStatement(variable="sum", expression=BinaryOperation(left="a", operator="+", right="b"))
├── PrintStatement(values=["The sum of these numbers is: ", "sum"])
└── EndStatement()
```

Each node represents a statement or expression in the code, capturing its structure and relationships.  
In the execution phase, the interpreter can be tuned as follows.  
```cpp
if (root->type == InputStatement) {
    std::string inp;
    std::cout << root->prompt;
    std::cin >> inp;
    store (root->variable, inp);
}
```

## Example: Bytecode Generation (Optional)

Here's a sample bytecode representation for the QBasic program above. Each instruction is a simple operation that the interpreter's virtual machine would execute:

```
0: INPUT   "Enter the first number: " a
1: INPUT   "Enter the second number: " b
2: LOAD    a
3: LOAD    b
4: ADD
5: STORE   sum
6: PRINT   "The sum of these numbers is: "
7: LOAD    sum
8: PRINTLN
9: END
```

**Explanation of Bytecode Instructions:**
- `INPUT <prompt> <var>`: Display prompt and store user input in `<var>`.
- `LOAD <var>`: Push the value of `<var>` onto the stack.
- `ADD`: Pop two values from the stack, add them, and push the result.
- `STORE <var>`: Pop value from the stack and store in `<var>`.
- `PRINT <value>`: Print the value (string or variable) without newline.
- `PRINTLN`: Print the value on top of the stack with a newline.
- `END`: Terminate the program.

This bytecode can be interpreted by a simple stack-based virtual machine.

The task should implement either AST generation and execution of the AST, or Bytecode generation from AST and execution of said bytecode.  
> [!TIP]
> As this is task involves some coding, you are encouraged to use version control
> and make your project open-source. You are free to use any programming language you like.

Please create a basic implementation of the language along with a presentation, either using PPT or preferably an Open Source
tool such as [RevealJS](https://revealjs.com/). The interviewee needs to keep
in mind that the crowd he will be presenting to, will have mixed people of
different knowledge levels, so it is advised to keep the content balanced
for all rather than becoming very technical.

## Some Resources
- https://ruslanspivak.com/lsbasi-part1/
- https://github.com/codecrafters-io/build-your-own-x?tab=readme-ov-file#build-your-own-programming-language
- https://www.craftinginterpreters.com/contents.html

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