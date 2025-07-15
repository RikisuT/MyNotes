```java
package proj1;
public class sports {
    public static void main(String[] args) {
        int sub1=40;
        int sub2=70;
        int sub3=59;
        if(sub1>=40 && sub2>=40 && sub3>=40){
            double per=(sub1+sub2+sub3)/3;
            if(per>=85)
                System.out.println("Grade A");
            else if(per>=60 && per<85)
                System.out.println("Grade B");
            else if(per<60&&per>=40)
                System.out.println("Grade C");
            else
                System.out.println("Fail");
        }
    }
}
```