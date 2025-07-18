```java
package proj1.OOPs;

public class Animal {
    Animal(){
        System.out.println("Animal");
    }
    Animal(String name,String sound){
        System.out.println(name);
        System.out.println(sound);
        
    }
    @SuppressWarnings("unused")
    public static void main(String[] args) {
        System.out.println("Class Animal start");
        Animal a1=new Animal();
        Animal a2=new Animal("Dog","Bark");
        System.out.println("Class Animal end");
    }
}
```