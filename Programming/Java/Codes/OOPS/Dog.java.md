```java
package proj1.OOPs;

public class Dog extends Animal{
    Dog(){
        super("Timmy","Bark");
        System.out.println("Dog");
    }
    @SuppressWarnings("unused")
    public static void main(String[] args) {
        Dog d = new Dog();
    }
}
```