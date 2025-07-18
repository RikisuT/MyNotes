```java
package proj1;
public class vovel {
    public static void main(String[] args) {
        char s='Š';
        switch (Character.toLowerCase(s)) {            
            case 'a':
            case 'e':
            case 'i':
            case 'o':
            case 'u':
                System.out.println("Vovel");
                break;
            default:
                System.out.println("Consonant");
        }
        System.out.println(Character.toLowerCase(s));
    }
}

```