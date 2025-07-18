```java
package proj1.OOPs;

public class polymorph {
    public static int add(int a,int b ){
        return a+b;
    }
    public static int add(int a,int b,int c ){
        return a+b+c;
    }
    public static void main(String[] args) {
        System.out.println(add(1,2,3));
        System.out.println(add(1,2));
    }
}
```