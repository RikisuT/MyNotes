# Control Flow in C++

Control flow determines the order in which instructions are executed in a program. C++ provides several control flow structures including:

- Conditional statements
- Loops
- Jump statements

---

## Conditional Statements

Used to make decisions in code based on conditions.

### `if` Statement

```cpp
if (condition) {
    // code to execute if condition is true
}
````

### `if...else` Statement

```cpp
if (condition) {
    // if true
} else {
    // if false
}
```

### `else if` Ladder

```cpp
if (condition1) {
    // ...
} else if (condition2) {
    // ...
} else {
    // ...
}
```

### Ternary Operator

```cpp
(condition) ? expression_if_true : expression_if_false;
```

Example:

```cpp
int a = 10, b = 20;
int max = (a > b) ? a : b;
```

---

## Switch Statement

Used when you have multiple possible values for a single variable.
Cannot use float values as they are approximate values.

```cpp
switch (expression) {
    case value1:
        // code
        break;
    case value2:
        // code
        break;
    default:
        // code if no match
}
```

 Don't forget `break` to prevent fall-through.

---

## Loops

Used to repeat code multiple times.

### `while` Loop

```cpp
while (condition) {
    // code
}
```

### `do...while` Loop

```cpp
do {
    // code
} while (condition);
```

> 🔸 Executes the loop body at least once.

### `for` Loop

```cpp
for (initialization; condition; increment) {
    // code
}
```

Example:

```cpp
for (int i = 0; i < 5; i++) {
    std::cout << i << " ";
}
```

---

## Jump Statements

### `break`

Exits a loop or switch early.

```cpp
for (int i = 0; i < 10; i++) {
    if (i == 5) break;
}
```

### `continue`

Skips the current iteration.

```cpp
for (int i = 0; i < 10; i++) {
    if (i == 5) continue;
    std::cout << i << " ";
}
```

### `return`

Exits from a function.

```cpp
int add(int a, int b) {
    return a + b;
}
```

---

## Nested Control Flow

Control structures can be nested:

```cpp
for (int i = 0; i < 3; i++) {
    if (i % 2 == 0) {
        std::cout << i << " is even\n";
    }
}
```

---

## What's Next?

Explore:

- [[Functions]]
- [[Loops and Iteration (Advanced)]]
- [[Switch vs If-Else]]