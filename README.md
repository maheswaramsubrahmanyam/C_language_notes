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
###What is a compilation?<br>
The compilation is a process of converting the source code into object code. It is done with the help of the compiler. The compiler checks the source code for the syntactical or structural errors, and if the source code is error-free, then it generates the object code.<br>


![image](https://github.com/user-attachments/assets/a713bb4a-d5fa-4e57-959a-89c735294ba5)
<br>
The c compilation process converts the source code taken as input into the object code or machine code. The compilation process can be divided into four steps, i.e., Pre-processing, Compiling, Assembling, and Linking.<br>

The preprocessor takes the source code as an input, and it removes all the comments from the source code. The preprocessor takes the preprocessor directive and interprets it. For example, if <stdio.h>, the directive is available in the program, then the preprocessor interprets the directive and replace this directive with the content of the 'stdio.h' file.<br>

<br>

![image](https://github.com/user-attachments/assets/01ff5016-9c46-4e48-9fec-f175be345b3f)
<br>

Preprocessor<br>
The preprocessor processes directives like #include and #define before actual compilation.<br>
It expands macros and includes header files into the source code.<br>
<br>
Compiler<br>
The compiler translates the expanded code into low-level assembly code.<br>
It also performs syntax checking and optimization during this phase.<br>
<br>
Assembler<br>
The assembler converts the assembly code into machine-level object code.<br>
It generates a file with a .obj (DOS) or .o (UNIX) extension.<br>
<br>
Linker<br>
The linker combines the program’s object code with library object code.<br>
It produces the final executable file like .exe (DOS) or a.out (UNIX).<br>
<br>


```
// # data types in C 
// Integer => int 
// Float  => float
// Boolean => bool
// String => char string

// ========================
// Variables in C 
// variables are containers for storing data values like number or charater 

// In c language we have diffrent types of varables 
// int -> (-infinity to + infinity)
// float -> (0.1 5.99)
// char -> storing single letter / charater susch as 'a','A'

// Declaring (Creating) Variables 

// syntax:
// Data_type Varable_name = value;

// Data_type => (int,float , char, string)
// varable_name => container name 
// value => 99, 0.54, 'c' ,"hjfs"

// example:
// int num = 10;
// float num2 = 0.693;
// int a; # Varable Declartion 
// a = 20; #value assigned to variable 

// ----------------------------------------
// Format Specifires

// int => %d 
// float => %f 
// char => %c 
// string => %s 
// printf()
#include<stdio.h>
int main() {
    
int a = 156;
int d = 25;

printf("%d \n%d \n",a,d);

float b = 14.3;
printf("%f\n",b);

char c = 'A';
printf("%c\n",c);
return 0;

}```
<br>

```#include<stdio.h>
int main() {
    
int a = 156;
float b = 14.3;
char c = 'A';

// to combine text and variables, seperate them with a comma inside the printf() function
printf("My integer value is :%d", a);

return 0;

}```

