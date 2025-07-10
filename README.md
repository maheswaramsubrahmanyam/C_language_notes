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
}```
---

| Component    | Description                                                  |
| ------------ | ------------------------------------------------------------ |
| `#include`   | Preprocessor directive; the first thing read by the compiler |
| `stdio.h`    | Header file containing input/output functions                |
| `int main()` | Main function of the program with return type `int`          |
| `printf`     | Prints formatted strings to standard output                  |
| `return`     | Terminates the function and returns control to the caller    |
