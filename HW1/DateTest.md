````java
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package date;

import java.util.Scanner;

public class DateTest {
    public static void main (String [] args) {
         
        Date display = new Date (0,0,0);
 
        Scanner input = new Scanner (System.in);
         
        int month;
        int day;
        int year;
         
        System.out.print ("Enter Month: ");
        month = input.nextInt();
        display.setMonth(month);
         
        System.out.println ();
         
        System.out.print ("Enter Day: ");
        day = input.nextInt();
        display.setday(day);
         
        System.out.println ();
         
        System.out.print ("Enter Year: ");
        year = input.nextInt();
        display.setYear(year);
         
        System.out.println ();
         
        display.displayDate();
 
    }
}

`````
