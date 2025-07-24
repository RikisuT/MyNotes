# C++ Basics

Welcome to the foundational page for learning C++! This page covers the core concepts every beginner must know before diving deeper into advanced topics.

---

## What is C++?

C++ is a **general-purpose, high-performance** programming language developed by Bjarne Stroustrup as an extension of the C programming language.  
It supports:

- Procedural Programming  
- Object-Oriented Programming (OOP)  
- Generic Programming  

---

## Basic Structure of a C++ Program

```cpp
#include <iostream>  // Preprocessor directive

int main() {
    std::cout << "Hello, World!" << std::endl;
    return 0;
}
````

**Key components:**

- `#include <iostream>`: Includes input/output stream library.
    
- `int main()`: Entry point of every C++ program.
    
- `std::cout`: Prints output to the console.
    
- `return 0;`: Indicates successful execution.
    

---

## Data Types

|Type|Description|Example|
|---|---|---|
|`int`|Integer|`int x = 5;`|
|`float`|Floating-point number|`float pi = 3.14;`|
|`double`|Double-precision float|`double d = 3.1415;`|
|`char`|Character|`char c = 'A';`|
|`bool`|Boolean (true/false)|`bool flag = true;`|
|`void`|No return value|`void func() {}`|

---

## Variables and Constants

```cpp
int age = 21;         // Variable
const float PI = 3.14; // Constant
```

- Variables can change during program execution.
    
- Constants remain fixed and cannot be modified.
    

---

## Input and Output

```cpp
#include <iostream>
using namespace std;

int main() {
    int age;
    cout << "Enter your age: ";
    cin >> age;
    cout << "You are " << age << " years old.";
    return 0;
}
```

- `cin` is used for input.
    
- `cout` is used for output.
    
- `<<` and `>>` are insertion and extraction operators respectively.
    

---

## Operators

- **Arithmetic**: `+`, `-`, `*`, `/`, `%`
    
- **Relational**: `==`, `!=`, `>`, `<`, `>=`, `<=`
    
- **Logical**: `&&`, `||`, `!`
    
- **Assignment**: `=`, `+=`, `-=`, `*=`, `/=`
    

---

## What's Next?

See:

- [[Programming/C++/Basics/Control Flow]]
- [[Functions]]
- [[Object-Oriented Programming]]
- [[Pointers & Memory]]

```

---

Let me know if you'd like me to generate any of the linked pages like `Control Flow`, `Functions`, etc. next — all ready for Obsidian formatting and backlinks!
```