```java
package proj1;

public class A {
    static int a;
    int b;
    static
    {
        System.out.println("AAAA");
    }
    public static void Hi(){
        System.out.println("Hi");
    }
    {
        System.out.println("HEHE");
    }
    public void Hello(){
        System.out.println("Hello");
    }
    public static void main(String[] args) {
        System.out.println("Class A start");
        int a=10;
        Hi();
        A a1=new A();
        System.err.println(a);
        System.err.println(A.a);
        System.err.println(a1.b);
        System.out.println("Class A end");
        a1.Hello();

    }
}

```