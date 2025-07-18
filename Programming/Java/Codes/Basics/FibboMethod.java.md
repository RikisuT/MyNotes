```java
package proj1;

public class fibboMethod {
    public static void main(String[] args) {
        fibbo(10);
    }
    public static void fibbo(int c) {
        int a=0;
        int b=1;
        while (a < c) {
            System.out.println(a);
            a=a+b;
            b=a-b;
        }
    }
}
```