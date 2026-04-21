# Mini-Compiler-Project
This project implements a simplified compiler using Flex for lexical analysis and Bison for parsing, allowing raw user input to be converted into tokens, interpreted using grammar rules, and executed in real time. It supports arithmetic operations, advanced math functions, variables, and control flow constructs like if/else statements, loops, and switch cases, making it feel like a small programming language rather than just a calculator. The system is structured across multiple components including a lexer, parser, main driver, and build system, closely mirroring how real compilers are organized. While it successfully demonstrates the full pipeline from input to execution, it has limitations such as single-pass loop execution and lack of a type system, which could be improved by adding features like an abstract syntax tree and more advanced language support. 

**Steps to run the mini compiler:**

1. **Open terminal and go to the project folder**

```bash
cd path/to/mini-compiler
```

2. **Compile everything using the Makefile**

```bash
make
```

This runs Flex, Bison, and GCC to build the executable.

3. **Run the compiler**

```bash
./compiler
```

4. **Enter input in the terminal**

* End each line with `;`

```c
x = 10;
y = 3;
x + y;
print x;
```

5. **Exit when done**

* Press `Ctrl + D` or `Ctrl + C`

**If `make` doesn’t work: install dependencies**

* macOS:

```bash
brew install flex bison gcc
```

* Ubuntu:

```bash
sudo apt update
sudo apt install flex bison gcc
```

This matches the compile and run flow shown in the report’s integration section. 


This matches the compile and run flow shown in the report’s integration section. 
