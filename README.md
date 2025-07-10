# C Language - First Program, Compilation, and Basics

Welcome to the C Programming Tutorial. In this lesson, you'll learn how to run your **first C program**, understand the **C compilation process**, and get introduced to **data types**, **variables**, **format specifiers**, and **comments** in C.

---

## 🚀 Running Your First C Program

Before you begin, ensure you have Turbo C installed and set up.

### Steps to Run

1. Go to: `Start > Turbo C`
2. Open a new project: `File > New`
3. Write the following code:

```c
#include <stdio.h>

int main()
{
    printf("Studyopedia C Language Tutorial"); 
    return 0;
}
```
---
| Component    | Description                                                  |
| ------------ | ------------------------------------------------------------ |
| `#include`   | Preprocessor directive; the first thing read by the compiler |
| `stdio.h`    | Header file containing input/output functions                |
| `int main()` | Main function of the program with return type `int`          |
| `printf`     | Prints formatted strings to standard output                  |
| `return`     | Terminates the function and returns control to the caller    |

---

🌟 Features of C Language<br>
Simple<br>
<br>
Machine Independent or Portable<br>

Mid-level programming language<br>

Structured programming language<br>

Rich Library<br>

Memory Management<br>

Fast Speed<br>

Pointers<br>

Recursion<br>

Extensible<br>

---
⚙️ What is Compilation?<br>
Compilation is a process of converting the source code into object code.<br>
It is done with the help of a compiler. The compiler checks the source code for syntactical or structural errors and generates the object code if the code is error-free.<br>![image](https://github.com/user-attachments/assets/2b1b3b50-642c-4612-bfd6-232ec9eb2059)
<br>


---
🛠️ C Compilation Process <br>
The compilation process can be divided into four steps: <br>

Pre-processing <br>

Compiling <br>

Assembling <br>

Linking <br>

🔸 Preprocessor <br>
Processes directives like #include and #define before actual compilation. <br>

Expands macros and includes header files into the source code. <br>

🔸 Compiler <br>
Translates the expanded code into low-level assembly code. <br>

Performs syntax checking and optimization. <br>

🔸 Assembler <br>
Converts the assembly code into machine-level object code. <br>

Generates a file with a .obj (DOS) or .o (UNIX) extension. <br>

🔸 Linker <br>
Combines the program’s object code with library object code. <br>

Produces the final executable file (.exe for DOS or a.out for UNIX). <br>
---

