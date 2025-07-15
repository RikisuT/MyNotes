```java 
public class Conditional {
    public static void main(String[] args) {
        int marks = 85;
        if (marks >= 60) {
            System.out.println("Passed");
            if (marks >= 90) {
                System.out.println("Excellent!");
            } else {
                System.out.println("Good job!");
            }
        } else {
            System.out.println("Failed");
        }
    }
}
```
