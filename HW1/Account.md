````Java
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package account;

/**
 *
 * @author User
 */
public class Account {
    private String name;
    private double balance;
    
    public Account(String name,double balance){
        this.name=name;
        if (balance>0.0)
            this.balance = balance;
    }
    
    public void withdraw(double withdrawAmount){
        if(balance<withdrawAmount){
            System.out.printf("Sorry, account's balances insufficient.%n%n");
        }else{
            if (withdrawAmount > 0.0){
                balance-= withdrawAmount;
            }
        }
    }
    
    public double getBalance(){
        return balance;
    }
    
    public void setName(String name){
        this.name=name;
    }
    
    public String getName(){
        return name;
    }
}
`````
