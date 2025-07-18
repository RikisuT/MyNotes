**Polymorphism** means **"many forms"**. In Java, polymorphism allows an object to take on **multiple forms**—the same method name can behave differently based on the **object** or **context**.

---

##  Why Use Polymorphism?

- Promotes **code reusability**
- Supports **method overriding** and **dynamic behavior**
- Enables **flexible and extensible** code

---

##  Types of Polymorphism in Java

| Type             | How It Works                      | When It's Resolved |
| ---------------- | --------------------------------- | ------------------ |
| **Compile-time** | Method Overloading                | At compile time    |
| **Runtime**      | Method Overriding via Inheritance | At runtime         |

---

##  1. Compile-Time Polymorphism (CTP)

Compile-Time Polymorphism means method or behavior is resolved during **compilation**. This is mainly achieved through:

### A. Method Overloading

**Same method name, different parameter list** within the same class.

```java
class Calculator {
    int add(int a, int b) {
        return a + b;
    }
    double add(double a, double b) {
        return a + b;
    }
    int add(int a, int b, int c) {
        return a + b + c;
    }
}
```

Allowed variations:

- Number of parameters
- Data types of parameters
- Order of parameters (if types differ)

---

###  B. Constructor Overloading

**Same class**, but **multiple constructors** with different parameters.

```java
class Student {
    Student() {
        System.out.println("Default constructor");
    }
    Student(String name) {
        System.out.println("Name: " + name);
    }
}
```

---

###  C. Variable Shadowing (Field Hiding)

Occurs when a **child class declares a variable with the same name** as in the parent class. This **hides** the parent class variable.

```java
class Parent {
    int value = 10;
}

class Child extends Parent {
    int value = 20; // shadows parent's value

    void show() {
        System.out.println("Child value: " + value);        // 20
        System.out.println("Parent value: " + super.value); // 10
    }
}
```

This is resolved at **compile time** based on the **reference type**.  
Shadowing applies only to **fields**, not instance methods.

---

###  D. Method Hiding (for static methods)

Occurs when a **static method** in a subclass has the **same signature** as one in the parent class. This is **not method overriding**, but **method hiding**.

```java
class PolyA {
    public static void Pratham() {
        System.out.println("Pratham");
    }
}

class PolyB extends PolyA {
    public static void Pratham() {
        System.out.println("Vaibhav");
    }

    public static void main(String[] args) {
        PolyA a1 = new PolyA();
        a1.Pratham();  // Pratham

        PolyB b1 = new PolyB();
        b1.Pratham();  // Vaibhav

        PolyA a2 = new PolyB();
        a2.Pratham();  // Pratham (NOT Vaibhav)

        PolyB b2 = (PolyB) a2;
        b2.Pratham();  // Vaibhav
    }
}
```

 Static methods are resolved at **compile time** using the **reference type**, not the object.  
 This is **not** polymorphism — it's method hiding.

---
##  2. Runtime Polymorphism (RTP)

Runtime Polymorphism happens when the method call is resolved **during execution** (runtime) using **dynamic method dispatch**.

###  A. Method Overriding

**Subclass provides a new implementation** for a method defined in the superclass.

```java
class Animal {
    void speak() {
        System.out.println("Animal speaks");
    }
}

class Dog extends Animal {
    @Override
    void speak() {
        System.out.println("Dog barks");
    }
}
```

---

###  B. Using Upcasting for RTP

```java
public class Main {
    public static void main(String[] args) {
        Animal obj = new Dog(); // Upcasting
        obj.speak();            // Calls Dog's speak() at runtime
    }
}
```

 Method is chosen based on the **actual object**, not the reference type.

---

###  C. Another Example

```java
class Shape {
    void draw() {
        System.out.println("Drawing shape");
    }
}

class Circle extends Shape {
    void draw() {
        System.out.println("Drawing circle");
    }
}

class Square extends Shape {
    void draw() {
        System.out.println("Drawing square");
    }
}

public class Main {
    public static void main(String[] args) {
        Shape s1 = new Circle();
        Shape s2 = new Square();

        s1.draw();  // Drawing circle
        s2.draw();  // Drawing square
    }
}
```

---

##  Summary

|Type|Technique|Resolved At|Example|
|---|---|---|---|
|CTP|Overloading|Compile time|`add(int, int)` vs `add(double)`|
|CTP|Shadowing|Compile time|`int value` in child vs parent|
|RTP|Overriding|Runtime|`Animal a = new Dog();`|

See Code : [[Polymorphism]]