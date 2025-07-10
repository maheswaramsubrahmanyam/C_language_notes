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
![image](https://github.com/user-attachments/assets/ff56cf6a-9e3e-4a24-bea8-f35ce9f91e9b)

---
###Data Types:<br>
| Type     | Description                     | Example                 |
| -------- | ------------------------------- | ----------------------- |
| `int`    | Integer                         | `int a = 5;`            |
| `float`  | Floating-point (decimal) number | `float b = 0.54;`       |
| `char`   | Single character                | `char c = 'A';`         |
| `string` | Character array (not a keyword) | `char str[] = "Hello";` |


---
📦 Variables in C <br>
Variables are containers for storing data values.<br>

Syntax<br>
```Data_type variable_name = value;```

Data_type: e.g., int, float, char<br>

variable_name: any valid identifier<br>

value: e.g., 99, 0.54, 'c', "text"<br>

```
int num = 10;
float num2 = 0.693;
int a;       // Variable declaration
a = 20;      // Assigning value

```
---
🔠 Format Specifiers <br>
Use format specifiers with printf() to print variable values.<br>
| Data Type | Format Specifier |
| --------- | ---------------- |
| `int`     | `%d`             |
| `float`   | `%f`             |
| `char`    | `%c`             |
| `string`  | `%s`             |

---
🧾 Example Code: Format Specifiers
<br>

```
#include<stdio.h>

int main() {
    int a = 156;
    int d = 25;

    printf("%d \n%d \n", a, d);

    float b = 14.3;
    printf("%f\n", b);

    char c = 'A';
    printf("%c\n", c);

    return 0;
}
```


