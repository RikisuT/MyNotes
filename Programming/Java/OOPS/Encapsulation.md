# Encapsulation

Encapsulation is the bundling of data with methods that operate on that data. It restricts direct access to some of an object's components.

Example: `CountObject.java`

```java
public class CountObject {
    private String name;
    private int mono;
    private static int count = 0;
    public CountObject(String name, int mono) {
        this.name = name;
        this.mono = mono;
        incrementCount();
    }
    public void printStudentDetails() {
        System.out.println(name);
        System.out.println(mono);
    }
    private static void incrementCount() {
        count++;
    }
}
```

- Fields `name`, `mono`, and `count` are private
- Access is via public methods

See Code : [[Accounts.java]],[[Savings.java]], [[Loans.java]]