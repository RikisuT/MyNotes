```java
package proj1;

public class B {
    static int looooo()
    {
        System.out.println("BBB");
        return 5;
    }
    public static void main(String[] args) {
        System.out.println("Class B start");
        A.Hi();
        System.out.println(A.a);
        A a1 = new A();
        a1.Hello();
        System.out.println(a1.b);
        System.out.println("Class B end");

    }
}
```