```java
package proj1;

public class CountObject {
    String name;
    int mono;
    String lol;
    static int count = 0;
    public CountObject(String name, int mono) {
        this.name = name;
        this.mono = mono;
        incrementCount();
    }
    public CountObject(String lol) {
        this.lol = lol;
        incrementCount();
    }
    public void printStudentDetails() {
        System.out.println("Student Name: " + name);
        System.out.println("Student ID: " + mono);
    }
    public void printLol() {
        System.out.println("Label: " + lol);
    }
    private static void incrementCount() {
        count++;
    }
    public static int getCount() {
        return count;
    }
    public static void main(String[] args) {
        CountObject student1 = new CountObject("Alice", 101);
        CountObject student2 = new CountObject("Bob", 102);
        CountObject labelOnlyObject = new CountObject("Unassigned");

        student1.printStudentDetails();
        student2.printStudentDetails();
        labelOnlyObject.printLol();

        System.out.println("Total Objects Created: " + getCount());
    }
}
```