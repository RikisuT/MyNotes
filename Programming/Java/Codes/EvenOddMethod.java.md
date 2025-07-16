```java
package proj1;
import java.util.Scanner;
public class EvenOddMethod {
    public static void Check(int a){
        System.out.println(a%2==0?"Even":"Odd");
    }
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("Enter Your Number : ");
        int a=scanner.nextInt();
        Check(a);
        scanner.close();
    }
}
```