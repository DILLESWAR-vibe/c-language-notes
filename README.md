#  C Programming Notes

A complete guide to learning and revising the C programming language — covering all important topics, concepts, and examples.

---

## 📘 1. Introduction to C

- C is a **procedural programming language** developed by **Dennis Ritchie** in **1972** at Bell Labs.  
- It is widely used for **system programming**, **embedded systems**, and **software development**.  
- C is known as the **mother of all modern languages** (like C++, Java, and Python).  
- Programs in C are compiled and executed for high performance.

### 🔹 Structure of a C Program
```c
#include <stdio.h>

int main() {
    printf("Hello, World!");
    return 0;
}

🔤 2. Basic Concepts

Keywords: Predefined words with special meaning (e.g., int, float, return, if, for)

Identifiers: Names given to variables, functions, arrays, etc.

Variables: Used to store data values.

Constants: Fixed values that cannot be changed during program execution.

🔹 Example
int age = 20;
const float PI = 3.14;
printf("Age: %d, PI: %.2f", age, PI);

➕ 3. Operators and Expressions
Types of Operators

Arithmetic (+, -, *, /, %)

Relational (==, !=, <, >, <=, >=)

Logical (&&, ||, !)

Assignment (=, +=, -=)

Increment/Decrement (++, --)

Bitwise (&, |, ^, <<, >>)

🔹 Example
int a = 10, b = 5;
printf("Sum = %d", a + b);

🔁 4. Control Statements
Decision Making

if

if-else

else-if ladder

switch

Loops

for

while

do-while

Jump Statements

break

continue

goto

🔹 Example
for(int i = 1; i <= 5; i++) {
    printf("%d ", i);
}

🧩 5. Functions

A function is a block of code that performs a specific task.

Promotes code reusability and modular programming.

Types

Library functions (printf, scanf, sqrt, etc.)

User-defined functions

🔹 Example
int add(int x, int y) {
    return x + y;
}

int main() {
    printf("%d", add(5, 10));
    return 0;
}

🧮 6. Arrays

Collection of elements of the same data type stored in contiguous memory.

Accessed using index numbers (starting from 0).

🔹 Example
int arr[5] = {1, 2, 3, 4, 5};
for(int i = 0; i < 5; i++) {
    printf("%d ", arr[i]);
}

🔠 7. Strings

A string is a sequence of characters ending with a null character \0.

Can be handled using character arrays or string functions.

Common Functions

strlen()

strcpy()

strcat()

strcmp()

🔹 Example
char name[20] = "C Language";
printf("Welcome to %s", name);

📍 8. Pointers

A pointer is a variable that stores the memory address of another variable.

Used for dynamic memory allocation and function arguments.

🔹 Example
int a = 10;
int *ptr = &a;
printf("Value: %d, Address: %p", *ptr, ptr);

🧱 9. Structures and Unions
Structures

Used to group different data types together.

struct Student {
    int id;
    char name[50];
    float marks;
};

Unions

Similar to structures, but shares memory among members.

union Data {
    int i;
    float f;
    char str[20];
};

📂 10. File Handling

Used to read and write data to files.

File Functions

fopen()

fprintf()

fscanf()

fclose()

🔹 Example
FILE *fp = fopen("data.txt", "w");
fprintf(fp, "Hello File");
fclose(fp);

💾 11. Dynamic Memory Allocation

Functions:

malloc()

calloc()

realloc()

free()

🔹 Example
int *ptr;
ptr = (int*) malloc(5 * sizeof(int));
