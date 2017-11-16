```java
package circle;

import java.util.Scanner;
public class Circle {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        
        Scanner radius= new Scanner(System.in);
        
         System.out.println("Enter the radius:");
         double r= radius.nextDouble();
         double  area= Math.PI * Math.Pow(r,2) ;
         System.out.println("Area of Circle is: " + area);      
    }
    
}
```
