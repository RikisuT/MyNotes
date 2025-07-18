```java
package proj1.OOPs;

public class PolyB extends PolyA {
    public static void Pratham(){
        System.out.println("Vaibhav");
    }
    public static void main(String[] args) {
        PolyA a1=new PolyA();
        a1.Pratham();
        PolyB b1=new PolyB();
        b1.Pratham();
        PolyA a2=new PolyB();
        a2.Pratham();
        PolyB b2=(PolyB) a2;
        b2.Pratham();
    }
}

```