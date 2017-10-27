````java
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package account;

import java.util.Scanner;

public class AccountTest {
    public static void main(String[] args){
        Account account1 = new Account("Jane Green",50.00);
        Account account2 = new Account("John Blue",-7.53);
        
        System.out.printf("%s balance: $%.2f%n", account1.getName(),account1.getBalance());
        System.out.printf("%s balance: $%.2f%n%n", account2.getName(),account2.getBalance());
        
        Scanner input = new Scanner(System.in);
        
        System.out.print("Enter withdraw amount for account1: ");
        double withdrawAmount = input.nextDouble();
        System.out.printf("%nwithdrawing %.2f from account1's balance%n%n",withdrawAmount);
        account1.withdraw(withdrawAmount);
        
        System.out.printf("%s balance: $%.2f%n", account1.getName(),account1.getBalance());
        System.out.printf("%s balance: $%.2f%n%n", account2.getName(),account2.getBalance());
        
        System.out.print("Enter withdraw amount for account2: ");
        withdrawAmount = input.nextDouble();
        System.out.printf("%nwithdrawing %.2f from account2's balance%n%n",withdrawAmount);
        account2.withdraw(withdrawAmount);
        
        System.out.printf("%s balance: $%.2f%n", account1.getName(),account1.getBalance());
        System.out.printf("%s balance: $%.2f%n%n", account2.getName(),account2.getBalance());
    }
}
`````
