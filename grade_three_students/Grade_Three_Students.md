```java
package grade_three_students;


public class Grade_Three_Students {

    
    public static void main(String[] args) {
        int[][] grades= {{100, 92, 93, 84},
                            {85, 96, 87},
                            {77, 67}};
        Group mygroup = new Group(grades);
        mygroup.calculate();
        System.out.printf("%s", mygroup);
    }
    
}
```
