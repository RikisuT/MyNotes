```java
package proj1;

public class Loans extends Account{
    double Loan;
    public Loans(double Loan) {
        super("Likhtih", 119191, 20000);
        this.Loan=Loan;
    }
    public void Loanaccountdetails(){
        System.out.println("Loan : "+Loan);
    }
    public static void main(String[] args) {
        Loans a=new Loans(10000);
        a.accdetails();
        a.Loanaccountdetails();
    }
}
```