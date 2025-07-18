```java
package proj1;

public class C extends A {
    String Name;
    C(String Name) {
        super();
        this.Name=Name;
    }
    public static void main(String[] args) {
        C c = new C("hahaha");
        c.Name="Likhith";
        System.out.println("C");
    }
}
```