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

The Second line of code we see is `int main()`, is defining a function named `main()` which is needed for every C/C++ file to compile & link. The `()` is meant for arguments; `int main(int argc, char * argv[])`. The `int` of this function is the return type of the function, so when the code is ran it must return an integer which you can do via code with the `return` keyword;

```cpp
#include <iostream>
int main()
{
  std::cout << "Hello World!" << std::endl;
  return 0;
}
```

*OUTPUT*

```
Hello World!

```
You dont need to `return 0;` due to the compiler doing it for you most of the time

