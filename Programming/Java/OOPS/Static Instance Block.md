# Static and Instance Blocks

## Static Block

Executed once when the class is loaded into memory, before `main()` or object creation.

```java
static {
    System.out.println("AAAA");
}
```

Used in:

- `A.java`: Prints "AAAA" on first use of class `A`
- `B.java`: Calls `A.Hi()` to trigger `A`'s static block

## Instance Block

Executed every time an object is created.

```java
{
    System.out.println("HEHE");
}
```

- In `A.java`, prints "HEHE" during object creation

See Code : [[A.java]], [[B.java]], [[C.java]]