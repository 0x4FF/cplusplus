**Analyze** 
```cpp
#include <iostream>
int main()
{
    std::cout << "Hello World!" << std::endl;
}
```

So when we look at this code the first line we see is `#include <iostream>`. This is a preprocessor directive that includes the content of the standard C++ header file, what is a "preprocessor" you might ask?.

*Preprocessor*

The preprocessor is a program that processes its input data to produce output that is used as input to another program, it is apart of the compilation process, while writing code you can include preprocessor directives like; `#include <iostream>`. `<iostream>` is a header file including instructions to later be used in the source code.

*Functions*

The Second line of code we see is `int main()`, is defining a function named `main()` which is needed for every C/C++ file to compile & link. The `()` is meant for arguments; `int main(int argc, char * argv[])`.

The `int` of this function is the return type of the function, so when the code is ran it must return an integer if it doesnt return an integer a error will be raised which you can avoid via code with the `return` keyword, you may also see this being called exit code;

```cpp
#include <iostream>
int main()
{
  std::cout << "Hello World!" << std::endl; // you can also remove std::endl;
  return 0;
}
```

*OUTPUT*

```
Hello World!

```
You dont need to `return 0;` due to the compiler doing it for you most of the time.


The next line of code is `std::cout << "Hello World!" << std::endl;` which is placed inside `{}` in order for it to be read by the compiler(https://en.wikipedia.org/wiki/Compiler) to run.

Now lets break this code down, `std` is a namespace, there are many namespaces. Here, we use `::` to show we want to use `cout` from the std namespace. `cout` is the character output function and it returns output to the console or terminal. 

*NOTE:* `cout` uses the `write()` system call in linux systems



**Comments**

A comment is a way to put arbitrary text inside source code without having the C++ compiler interpret it with any
functional meaning. Comments are used to give insight into the design or method of a program.

```
// This is a single-line comment

/*
  * This is a block or multi-line comment.
*/
```
The above example is valid C++ (and C) code. However, having additional `/*` inside a block comment might result in
a warning on some compilers.

The double forward-slash sequence `//` will mark all text until a newline as a comment

The sequence `/*` is used to declare the start of the comment block and the sequence `*/` is used to declare the end
of a multi-line comment.

As with all programming languages, comments provide several benefits:

    Explicit documentation of code to make it easier to read/maintain
    Explanation of the purpose and functionality of code
    Details on the history or reasoning behind the code
    Placement of copyright/licenses, project notes, special thanks, contributor credits, etc. directly in the source code.

***COMPILATION***

A compiler is a program that translates code from a programming language into another form which is (more)
directly executable for a computer. Using a compiler to translate code is called compilation.

The compiler has Four Main steps:

*Preprocessing*

If you included a header file such as `#include <stdio.h>`, it will look for the `stdio.h` file and copy the header file into the source code file.
The preprocessor also generates macro code and replaces symbolic constants defined using `#define` with their values.

*Compiling*

After the code has been preprocessed the compiler takes the ouput data and goes through a few phases
```
1. Lexical analysis; the process of converting a sequence of characters into a sequence of tokens

2. Parsing; the process of analyzing a string of symbols, either in natural language, computer languages or data structures, kinda like grammar for programming languages

3. Semantic analysis; the process of gathering necessary semantic information from the source code and type checking
```

*Assembling & Linking*

The assembler will convert the assembly code into pure binary code or machine code (zeros and ones). This code is also known as object code.

The Linker will then link the object code from multiple objects into one

*Execution*

You then run the binary file; `./<filename>` `<filename>.exe` in the terminal
