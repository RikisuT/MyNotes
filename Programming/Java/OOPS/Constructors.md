# Constructors in Java

##  What is a Constructor?

A **constructor** is a special method used to **initialize objects**. It runs **automatically** when an object is created using `new`.

```java
class Student {
    Student() {
        System.out.println("Constructor called");
    }
}
```

---

##  Types of Constructors

### 1. **Default Constructor**

Automatically provided by Java if no constructor is defined.
C.java
```java
class A {
    A() {
        System.out.println("Default constructor");
    }
}
```

### 2. **Parameterized Constructor**

Takes arguments to initialize data members.

```java
class A {
    int x;

    A(int value) {
        x = value;
    }
}
```

### 3. **Copy Constructor** _(Java doesn’t support this natively but you can define one)_

```java
class A {
    int x;

    A(int val) {
        x = val;
    }

    A(A obj) {
        x = obj.x;
    }
}
```

---

##  Constructor Overloading

Multiple constructors with different parameters.

```java
class A {
    A() {
        System.out.println("No-arg constructor");
    }

    A(int x) {
        System.out.println("Param constructor: " + x);
    }
}
```

---

##  Constructor Chaining

Using `this()` to call another constructor in the same class.

```java
class A {
    A() {
        this(10);
        System.out.println("Default");
    }

    A(int x) {
        System.out.println("Param: " + x);
    }
}
```

---

##  `super()` and Inheritance

Use `super()` to call the parent class constructor.

```java
class Parent {
    Parent() {
        System.out.println("Parent Constructor");
    }
}

class Child extends Parent {
    Child() {
        super(); // Calls Parent()
        System.out.println("Child Constructor");
    }
}
```

---

#  Upcasting and  Downcasting

##  Upcasting (Safe)

Subclass → Superclass reference

```java
class Animal {
    void sound() {
        System.out.println("Some sound");
    }
}

class Dog extends Animal {
    void bark() {
        System.out.println("Bark");
    }
}

Animal a = new Dog(); // Upcasting
a.sound(); // Allowed
// a.bark(); ❌ Not allowed
```

- Used for **polymorphism** .
- Always safe and implicit

---

##  Downcasting (Risky)

Superclass → Subclass reference (requires explicit cast)

```java
Animal a = new Dog(); // Upcast
Dog d = (Dog) a;      // Downcast
d.bark();             // Allowed now
```

 Risky: Fails at runtime if the object is **not actually** of the subclass type

```java
Animal a = new Animal();
Dog d = (Dog) a; // ❌ Runtime error: ClassCastException
```

---

##  Summary

|Concept|Description|
|---|---|
|Constructor|Initializes objects when created|
|`this()`|Calls another constructor in same class|
|`super()`|Calls parent class constructor|
|Upcasting|Subclass → Superclass reference (safe, automatic)|
|Downcasting|Superclass → Subclass reference (manual, risky)|


See Code :
[[C.java]]