```java
package grade_three_students;


public class Group {
    private int[][] grades;
    private int[] ave = new int[3];
    
    public Group(int grades[][]){
        this.grades=grades;
    }
    public void calculate(){
        int sum;
        int i=0;
        for(int[] s: grades){
            sum=0;
            for(int score : s){
                sum+=score;
            }
            ave[i++]=sum/s.length;
        }
    }
    public String toString(){
        return "average: \n"+"row 0:"+ave[0]+"\n"+"row 1:"+ave[1]+"\n"+"row 2:"+ave[2];
    }
    
}
```
