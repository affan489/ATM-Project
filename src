import java.util.*;
class ATM {
    int pin = 1234;
    float Bal;

    public void checkpin()
    {
        System.out.println("Enter your PIN: ");
        Scanner sc = new Scanner(System.in);
        int enteredpin = sc.nextInt();
        if (enteredpin == pin) {
            menu();
        }
        else {
            System.out.println("Enter a valid pin");
            menu();
        }
    }

    public void menu() {
        System.out.println("Enter your choice");
        System.out.println("1. Check Balance");
        System.out.println("2. Widthdraw money");
        System.out.println("3. Deposit Money");
        System.out.println("4. Exit Money");


        Scanner sc = new Scanner(System.in);
        int opt = sc.nextInt();
        if (opt == 1) {
            checkBalance();
        } else if (opt == 2) {
            widhdrawMoney();
        } else if (opt == 3) {
            depositMoney();
        } else if (opt == 4) {
            return;
        } else {
            System.out.println("Enter a valid Choice");
        }

    }
    public void checkBalance() {
        System.out.println("Balance: " + Bal);
        menu();
    }

    public void widhdrawMoney() {
        System.out.println("Enter the amount to Widhdraw: ");
        Scanner sc = new Scanner(System.in);
        int amount = sc.nextInt();
        if (amount > Bal) {
            System.out.println("Insufficient Balance");
        } else {
            Bal = Bal - amount;
            System.out.println("Money widhdrawn successfully");
        }
        menu();
    }

    public void depositMoney() {
        System.out.println("Enter the amount to deposit: ");
        Scanner sc = new Scanner(System.in);
        float amount = sc.nextFloat();
        Bal = Bal + amount;
        System.out.println("Money deposited");
        menu();
    }
}

public class Main {
    public static void main(String[] args) {
        ATM myATM =new ATM();
        myATM.menu();
}}
