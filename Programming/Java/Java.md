# Java Overview

## What is Java?

Java is a **high-level**, **object-oriented**, **platform-independent** programming language. It was developed by **James Gosling** at **Sun Microsystems** (now owned by Oracle) and released in **1995**.

> Java’s motto: “Write Once, Run Anywhere” (WORA)

---

## Key Features of Java

- **Object-Oriented** – Everything is based on classes and objects
- **Platform-Independent** – Java code runs on any OS with the Java Virtual Machine (JVM)
- **Simple & Secure** – Designed to be easy to learn and resistant to memory leaks
- **Robust** – Strong memory management, exception handling, and type checking
- **Multithreaded** – Supports concurrent execution of two or more threads
- **Distributed** – Can be used to build distributed applications (e.g., RMI, EJB)

---

## Java Architecture

1. **Java Source Code (.java)** – You write this
2. **Compiler (javac)** – Converts `.java` to `.class` (bytecode)
3. **JVM (Java Virtual Machine)** – Runs the bytecode on your OS

```text
[Your Code] → javac → [Bytecode] → JVM → [Runs on any platform]
````

---

## Editions of Java

- **Java SE** (Standard Edition) – For desktop and core applications
- **Java EE / Jakarta EE** (Enterprise Edition) – For large-scale applications
- **Java ME** (Micro Edition) – For embedded systems and mobile
- **JavaFX** – For rich GUI desktop applications

---

## Common Java Tools

- **JDK** – Java Development Kit (includes compiler, tools, libraries)
- **JRE** – Java Runtime Environment (just the JVM + runtime libs)
- **IDE** – IntelliJ IDEA, Eclipse, VS Code, NetBeans

---

## First Java Program

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

- `public class HelloWorld` – defines a class named `HelloWorld`
- `main` – the entry point
- `System.out.println` – prints to the console

---

## Summary

Java is a powerful, cross-platform language suitable for everything from mobile apps to large-scale enterprise software. It's widely used in industry and academic settings alike.

---

tags: #java #introduction #overview
[[Data Types]] [[Basics Operators]] [[Control Flow]] [[OOPS in Java]] [[Type Casting]]

