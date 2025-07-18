```java
class Person {
    String name;
    Person() {
        this("Unknown"); 
        System.out.println("Person default constructor called");
    }
    Person(String name) {
        this.name = name;
        System.out.println("Person parameterized constructor called: " + name);
    }
}
class Student extends Person {
    int rollNo;
    Student(String name, int rollNo) {
        super(name);
        this.rollNo = rollNo;
        System.out.println("Student constructor called: Roll No = " + rollNo);
    }
}
public class Main {
    public static void main(String[] args) {
        Student s1 = new Student("Likhith", 42);
    }
}
```