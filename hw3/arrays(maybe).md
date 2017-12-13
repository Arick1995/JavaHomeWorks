````java
package array;

import java.util.*;

public class Array {

        
       
       
       
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        
        int[] arr = new int[12];
        int[][] rd = new int[12][2];
        int j = 0;
        
        
        System.out.println("Enter in the array numbers with a space: ");
        for(int i = 0; i < arr.length; i++) {
            arr[i] = input.nextInt();
        }
       
        for(int i =0; i < arr.length; i++) {
            arr[i] = (arr[i] * -1);
        }
        Arrays.sort(arr);
        for(int i =0; i < arr.length; i++) {
            arr[i] = (arr[i] * -1);
    }
        rd[j][0] = arr[0];
        for(int i =0;i<arr.length;i++){
            if(arr[i]==rd[j][0]){
                rd[j][1]++;
            }else if(arr[i] != arr[i-1]){
                j++;
                rd[j][0] = arr[i];
                rd[j][1]++;
            }
       }
        System.out.println("num\tfre");
        for(int i = 0;i<12;i++){
         System.out.println(rd[i][0]+"\t"+rd[i][1]);
        }
}
    
}
