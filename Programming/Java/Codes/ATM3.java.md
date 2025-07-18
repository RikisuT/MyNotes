```java
package proj1;

public class ATM3 extends ATM2{
    int Saving;
    ATM3(int Saving){
        super("Likhtih", 119191, 1000000);
        this.Saving=Saving;
    }
    public void Savingaccdetails(){
        System.out.println("Saving : "+Saving);
    }
    public static void main(String[] args) {
        ATM3 a=new ATM3(10000);
        a.accdetails();
        a.Savingaccdetails();
    }
}

```