```java
package proj1;

public class Savings extends Account{
    int Saving;
    Savings(int Saving){
        super("Likhtih", 119191, 1000000);
        this.Saving=Saving;
    }
    public void Savingaccdetails(){
        System.out.println("Saving : "+Saving);
    }
    public static void main(String[] args) {
        Savings a=new Savings(10000);
        a.accdetails();
        a.Savingaccdetails();
    }
}

```