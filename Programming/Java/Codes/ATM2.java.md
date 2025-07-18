```java
package proj1;

public class ATM2 {
    String Name;
    int AccNo;
    double Balance;
    ATM2(){
        
    }
    ATM2(String Name, int AccNo, double Balance){
        this.AccNo=AccNo;
        this.Name=Name;
        this.Balance=Balance;
    }
    void accdetails(){
        System.out.println("Name : "+Name);
        System.out.println("Account Number : "+AccNo);
        System.out.println("Balance : "+Balance);
    }
    void Withdraw(double amount){
        if(amount<=Balance){
            Balance-=amount;
            System.out.println("Balance : "+Balance);
        }
        else
            System.out.println("Not enough balance \n Balance : "+Balance);

    }
    void Deposit(double amount){
        Balance+=amount;
        System.out.println("Balance : "+Balance);
    }
    public static void main(String[] args) {
        ATM2 a=new ATM2("Likhtih", 119191, 1000000);
        a.accdetails();
        a.Deposit(100000.0);
        a.Withdraw(1414.1313);
        
    }
}

```