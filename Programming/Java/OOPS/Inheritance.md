Certainly! Here's an expanded explanation of **Inheritance** in Java with code snippets for each **type of inheritance**:

---

# Inheritance in Java

Inheritance allows a class to acquire properties and methods of another class. The class that inherits is called the **subclass (child)**, and the class being inherited from is the **superclass (parent)**.

```java
public class Animal {
    void eat() {
        System.out.println("This animal eats food.");
    }
}
```

---

## 1. **Single Inheritance**

One subclass inherits from one superclass.

```java
public class Dog extends Animal {
    void bark() {
        System.out.println("Dog barks.");
    }
}
```

- `Dog` inherits `eat()` from `Animal`.

---

## 2. **Multilevel Inheritance**

A subclass inherits from a class that is already a subclass of another class.

```java
public class Puppy extends Dog {
    void weep() {
        System.out.println("Puppy weeps.");
    }
}
```

- `Puppy` inherits `bark()` from `Dog`, and `eat()` from `Animal`.

---

## 3. **Hierarchical Inheritance**

Multiple classes inherit from a single superclass.

```java
public class Cat extends Animal {
    void meow() {
        System.out.println("Cat meows.");
    }
}

public class Cow extends Animal {
    void moo() {
        System.out.println("Cow moos.");
    }
}
```

- Both `Cat` and `Cow` inherit `eat()` from `Animal`.

---

## 4. **Hybrid Inheritance** _(Not directly supported in Java)_

Java doesn't support hybrid inheritance (combining multiple and multilevel) **with classes**, but **interfaces** can be used to simulate it.

---

## 5. **Multiple Inheritance (Using Interfaces)**

A class can implement multiple interfaces.

```java
interface Printable {
    void print();
}

interface Showable {
    void show();
}

public class Document implements Printable, Showable {
    public void print() {
        System.out.println("Printing...");
    }

    public void show() {
        System.out.println("Showing...");
    }
}
```

- `Document` implements both `Printable` and `Showable`.
---

## Summary Table

|Type|Supported via|Example Classes|
|---|---|---|
|Single|Class|`Dog extends Animal`|
|Multilevel|Class|`Puppy → Dog → Animal`|
|Hierarchical|Class|`Cat`, `Cow` ← `Animal`|
|Multiple|Interface|`Document implements A, B`|
|Hybrid|Interface combo|Interfaces + Classes|

---
See Code:
- [[A.java]]
- [[B.java]]
- [[C.java]] 
