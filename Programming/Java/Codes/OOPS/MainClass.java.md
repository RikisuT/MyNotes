```java
package proj1;
public class MainClass {
    public static void main(String[] args) {
        A obj = new A();
        obj.publicMethod(10,3,'O');
        // obj.privateMethod(); 
    }
}
class A {
    public void publicMethod(int a,int b,char c) {
        System.out.println("Public");
        System.out.println(a);
        privateMethod((double) a / b);
    }
    private void privateMethod(double a) {
        System.out.println(a);
        System.out.println("Private");
    }
}
```