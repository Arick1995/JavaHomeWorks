````java
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package date;

/**
 *
 * @author User
 */
public class Date {
 
    private int md;
    private int dd;
    private int yd;
     
    public Date (int month, int day, int year) {
        md = month;
        dd = day;
        yd = year;
    }
     
    public void setMonth (int month) {
        md = month;
    }
     
    public int getMonth() {
        return md;
    }
     
    public void setday (int day) {
        dd = day;
    }
     
    public int getDay() {
        return dd;
    }
     
    public void setYear (int year ) {
        yd = year;
    }
     
    public int getYear() {
        return yd;
    }
     
    public void displayDate () {
        System.out.printf ("%d/%d/%d\n", getMonth(), getDay(), getYear());
    }
 
}
````
