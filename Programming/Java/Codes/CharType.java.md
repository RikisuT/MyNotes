```java
package proj1;
public class chartype {
    public static void main(String[] args) {
        int a = 's';
        String Result=a>0&&a<9? "Digit":a>'a'&&a<'z'||a<'A'&&a<'Z'?"Charater":"Special Char";
        System.out.println(Result);
    }
}
```