package mathgame;

import java.util.Scanner;
import java.util.Random;

public class MathGame {

    
    public static void main(String[] args) {
        play start = new play();
        start.newgame();
    }
    
}

    class play{
        int guest ,num,max,min;
        Scanner n = new Scanner(System.in);
        Random rn = new Random();
        
        public void newgame(){
            System.out.print("Guess a number between 1～1000\n");

            num=1+rn.nextInt(1000);
             System.out.print("Game Start!\n\nPlease input a integer between 1～1000：\n");
             
           guest=n.nextInt();
            max =1000;
            min =1;
            
            game();
        }
        
        public void game(){
            while(true){
                if(guest>num){
                     max = guest;
                     System.out.print("Oops, it is too LARGE...");
                     System.out.printf("Try again!\nRange: %3d～%3d\n",min,max);
                     guest=n.nextInt();
                }else if (guest<num){
                    min = guest;
                    System.out.print("Oops, it is too small...");
                    System.out.printf("Try again!\nRange: %3d～%3d\n",min,max);
                    guest=n.nextInt();
                }else{
                    System.out.printf("Oh?! Congratulations!\nAnswer is %3d\n",num);
                    System.out.print("Do you want to play again ?\nyes = 1\n");
                    guest=n.nextInt();
                    while(guest == 1){
                        newgame();
                    }
                    System.out.print("Thank for your playing...");
                    break;
                }
            }
        }
    }
