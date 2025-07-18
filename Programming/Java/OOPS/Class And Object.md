# Java Classes and Objects

A class is a blueprint for creating objects.

```java
public class A {
    static int a;
    int b;
    ...
}
```

- `static int a` is a class variable (shared by all instances).
- `int b` is an instance variable (unique to each object).

Object Creation:

```java
A a1 = new A();
```

- Triggers the instance block.
- Gives access to instance methods and variables.

Variable Access:

- Local variable `int a = 10;` inside `main()` shadows the static variable `A.a`.
- Access static variable using `A.a`.
- Access instance variable `b` through object `a1.b`.
- A class is a blueprint for creating objects.
# Inter-Class Access

One class can access another class's static and instance members.

Example in `B.java`:

```java
A.Hi(); // static method
A a1 = new A();
a1.Hello(); // instance method
```

- Demonstrates cross-class access in the same package
- 
Referenced in:  [[CountObject.java]], [[MainClass.java]]