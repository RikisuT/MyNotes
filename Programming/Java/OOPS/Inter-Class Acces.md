# Inter-Class Access

One class can access another class's static and instance members.

Example in `B.java`:

```java
A.Hi(); // static method
A a1 = new A();
a1.Hello(); // instance method
```

- Demonstrates cross-class access in the same package

See Code : [[B.java]]