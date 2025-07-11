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
---
📝 Example Code: Combining Text and Variables

<br>

```#include<stdio.h>

int main() {
    int a = 156;
    float b = 14.3;
    char c = 'A';

    to combine text and variables, separate them with a comma inside printf()
    printf("My integer value is : %d", a);

    return 0;
}
```



---

💬 Comments in C Language<br<
Comments are used to explain the code. They improve readability and are not part of the execution.<br>

🔹 Single-line Comments<br>
Declared with two forward slashes //

```
// printing hello world using printf() function
printf("Hello World");
```

🔸 Multi-line Comments<br>
Start with /* and end with */<br>
```
/*
This is a multi-line comment.
Used to explain a block of code.
Helps in making the code more understandable.
*/
```


## 🧠 Get the Memory Size of Data Types in C

In the **Data Types** chapter, we learned that the memory size of a variable depends on its type.

### 📊 Common Data Type Sizes

| Data Type | Typical Size      |
|-----------|-------------------|
| `int`     | 2 or 4 bytes       |
| `float`   | 4 bytes            |
| `double`  | 8 bytes            |
| `char`    | 1 byte             |

> 🧩 The **memory size** refers to how much space a type occupies in the computer's memory.

---

## 📏 Using `sizeof` Operator

To get the actual memory size (in bytes) of a data type or variable, use the `sizeof` operator.

### 🔍 Example Code

```c
#include <stdio.h>

int main() {
    int myInt;
    float myFloat;
    double myDouble;
    char myChar;

    printf("%zu\n", sizeof(myInt));
    printf("%zu\n", sizeof(myFloat));
    printf("%zu\n", sizeof(myDouble));
    printf("%zu\n", sizeof(myChar));

    return 0;
}
```

---
## 🔁 Type Conversion in C

**Type Conversion** is the process of converting one data type into another. This is especially important when performing operations between different types (e.g., integers and floats).

---

### 📦 Example Use Case

Suppose you're dividing two integers:

```c
int a = 5;
int b = 2;
int result;

result = a / b;  // Output: 2 (0.5 is neglected because of integer division)
```
---
🧠 Types of Type Conversion<br>
Type conversions in C are of two types:<br>

Implicit Conversion (Automatic)<br>

Explicit Conversion (Manual)<br>

1️⃣ Implicit Conversion<br>
In implicit conversion, the compiler automatically converts a smaller data type to a larger data type to prevent data loss.<br>

🔍 Example: Implicit Conversion<br>
```
#include<stdio.h>

int main() {
    float a = 88;  // Integer 88 is implicitly converted to float
    printf("%f", a);
    return 0;
}
```
2️⃣ Explicit Conversion (Type Casting)<br>
In explicit conversion, the programmer manually converts one data type into another using casting.<br>

🔍 Example: Explicit Conversion<br>
```
#include<stdio.h>

int main() {
    int a = 5;
    int b = 2;

    float result = (float) a / b;  // Casting a to float before division
    printf("%f\n", result);

    return 0;
}
```
📝 Note: Using (float) before a variable tells the compiler to treat that variable as a float for the operation.<br>

---

## 🔒 Constants in C

In C programming, if you want to make a variable **constant**—meaning its value should never change throughout the program—you can use the `const` keyword.

### 🧠 What is `const`?

- `const` is a **keyword** used to declare **constant variables**.
- Once declared with `const`, the value of the variable **cannot be modified** later in the program.

---

### 🔍 Example: Constant Variable in C

```c
#include<stdio.h>

int main() {
    const int a = 10;  // 'a' is a constant and cannot be changed
    printf("%d\n", a);
    return 0;
}
```

##📌 Tip: Constants are especially useful for defining fixed values like PI, maximum limits, configuration settings, etc.<br>

```
const float PI = 3.14;
const int MAX_USERS = 100;
```
---

# ⚙️ Operators in C

**Operators** are used to perform operations on variables and values.

---

## ➕ Basic Operator Example

```c
int myNum = 100 + 50;
```
Although the + operator is often used to add together two values, it can also be used with:
```
int sum1 = 100 + 50;        // 150
int sum2 = sum1 + 250;      // 400
int sum3 = sum2 + sum2;     // 800
```
---
🧩 Types of Operators in C <br>
C divides operators into the following groups:<br>

Arithmetic Operators<br>

Assignment Operators<br>

Comparison Operators<br>

Logical Operators<br>

Bitwise Operators<br>

## ➗ Arithmetic Operators<br>

Arithmetic operators are used to perform basic mathematical operations.<br>

| Operator | Name           | Description                       | Example |
| -------- | -------------- | --------------------------------- | ------- |
| `+`      | Addition       | Adds two values                   | `x + y` |
| `-`      | Subtraction    | Subtracts one value from another  | `x - y` |
| `*`      | Multiplication | Multiplies two values             | `x * y` |
| `/`      | Division       | Divides one value by another      | `x / y` |
| `%`      | Modulus        | Returns the remainder of division | `x % y` |
| `++`     | Increment      | Increases value by 1              | `++x`   |
| `--`     | Decrement      | Decreases value by 1              | `--x`   |


---
## 📝 Assignment Operators
Assignment operators are used to assign values to variables.<br>

```
int x = 10;  // Assigns 10 to x
x += 5;      // Equivalent to x = x + 5;
```
| Operator | Example   | Same As      | 
| -------- | --------- | ------------ |
| `=`      | `x = 5`   | `x = 5`      | 
| `+=`     | `x += 3`  | `x = x + 3`  | 
| `-=`     | `x -= 3`  | `x = x - 3`  |    
| `*=`     | `x *= 3`  | `x = x * 3`  |     
| `/=`     | `x /= 3`  | `x = x / 3`  |      
| `%=`     | `x %= 3`  | `x = x % 3`  |   
| `&=`     | `x &= 3`  | `x = x & 3`  |     
| `        | =`        |  `x          | 
| `^=`     | `x ^= 3`  | `x = x ^ 3`  |   
| `>>=`    | `x >>= 3` | `x = x >> 3` |   
| `<<=`    | `x <<= 3` | `x = x << 3` |    


---

## 🔍 Comparison Operators
Used to compare two values. Returns 1 for true, 0 for false.<br>

```
int x = 5;
int y = 3;

printf("%d", x > y);  // Outputs 1 because 5 > 3
```

| Operator | Name                  | Example  | Description                             |
| -------- | --------------------- | -------- | --------------------------------------- |
| `==`     | Equal to              | `x == y` | True if x is equal to y                 |
| `!=`     | Not equal to          | `x != y` | True if x is not equal to y             |
| `>`      | Greater than          | `x > y`  | True if x is greater than y             |
| `<`      | Less than             | `x < y`  | True if x is less than y                |
| `>=`     | Greater than or equal | `x >= y` | True if x is greater than or equal to y |
| `<=`     | Less than or equal    | `x <= y` | True if x is less than or equal to y    |


---

## 🔗 Logical Operators

Used to combine multiple conditions and return true or false.<br>

| Operator | Name | Example              | Description                                |   
| -------- | ---- | -------------------- | ------------------------------------------ | 
| `&&`     | AND  | `x < 5 && x < 10`    | True if **both** conditions are true       |     
| `||`     |  OR  |  `x < 5 || x < 10`   | True if **at least one** condition is true |                               
| `!`      | NOT  | `!(x < 5 && x < 10)` | Reverses the result (true becomes false)   |         


---

# 🔀 Conditions and If Statements in C

C supports logical conditions that allow you to perform different actions based on different decisions.

---

## 📐 Logical Conditions

These are the common logical conditions used in C:

| Condition              | Symbol  |
|------------------------|---------|
| Less than              | `<`     |
| Less than or equal to  | `<=`    |
| Greater than           | `>`     |
| Greater than or equal  | `>=`    |
| Equal to               | `==`    |
| Not equal to           | `!=`    |

---

## 🧠 Conditional Statements in C

C provides the following conditional statements:

- `if` – Executes a block of code if a specified condition is `true`.
- `else` – Executes a block of code if the same condition is `false`.
- `else if` – Specifies a new condition to test if the first condition is `false`.
- `switch` – Selects one of many blocks of code to be executed.

---

## ✅ The `if` Statement

Use the `if` statement to specify a block of code to run when a condition is true.

### 🧾 Syntax

```c
if (condition) {
    // block of code to be executed if the condition is true
}
```

