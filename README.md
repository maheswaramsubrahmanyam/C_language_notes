C First Program

In the previous lesson, we learned how to set up the environment for C. Now, we will see how to run C first program.  It’s quite easy. Let’s begin with launching Turbo C and running C first program.

Go to Start > Turbo C

Open Turbo C and open a new project,

File > New


#include <stdio.h>
 
``int main()
{
   printf("Studyopedia C Language Tutorial"); 
 
   return 0;
}``

 
Here,

#include

It is the preprocessor and the first word read by the compiler

stdio.h

It is the header file.

int main()

main() function with return type int.

printf
Used to print the formatted string to stdout. The standard output is stdout.

return

Terminates the function execution and the return statement returns the control to the calling function.


C is the widely used language. It provides many features that are given below.

Simple
Machine Independent or Portable
Mid-level programming language
structured programming language
Rich Library
Memory Management
Fast Speed
Pointers
Recursion
Extensible
![image](https://github.com/user-attachments/assets/8228baea-a92c-4bae-9741-5f5021984f7a)

<br>
<br>
What is a compilation?<br>
The compilation is a process of converting the source code into object code. It is done with the help of the compiler. The compiler checks the source code for the syntactical or structural errors, and if the source code is error-free, then it generates the object code.<br>


![image](https://github.com/user-attachments/assets/a713bb4a-d5fa-4e57-959a-89c735294ba5)
<br>
The c compilation process converts the source code taken as input into the object code or machine code. The compilation process can be divided into four steps, i.e., Pre-processing, Compiling, Assembling, and Linking.<br>

The preprocessor takes the source code as an input, and it removes all the comments from the source code. The preprocessor takes the preprocessor directive and interprets it. For example, if <stdio.h>, the directive is available in the program, then the preprocessor interprets the directive and replace this directive with the content of the 'stdio.h' file.<br>
