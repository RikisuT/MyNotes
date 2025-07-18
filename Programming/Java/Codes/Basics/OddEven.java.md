```java
package proj1;
import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int a=scanner.nextInt();
        String result=(a%2==0)?"Even":"Odd";
        System.out.println(result);
        scanner.close();
    }    
}
```