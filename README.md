# java_hackerrank_solutions
[1. Java String Introduction](https://www.hackerrank.com/challenges/java-strings-introduction/problem)<br>
[Java compareTo() docs](https://www.javatpoint.com/java-string-compareto)

```java
import java.io.*;
import java.util.*;

public class Solution {

    public static void main(String[] args) {
        
        Scanner sc=new Scanner(System.in);
        String A=sc.next();
        String B=sc.next();
        /* Enter your code here. Print output to STDOUT. */
        System.out.println(A.length()+B.length());
        System.out.println(A.compareTo(B)>0?"Yes":"No");
        System.out.print(A.substring(0,1).toUpperCase()+A.substring(1)+" "+B.substring(0,1).toUpperCase()+B.substring(1));
<<<<<<< HEAD
        
=======
>>>>>>> e6c04b8 (3rd problem added)
    }
}
```
[2. Java Output Formatting](https://www.hackerrank.com/challenges/java-output-formatting/problem)
<<<<<<< HEAD
=======

>>>>>>> e6c04b8 (3rd problem added)
```java
import java.util.Scanner;

public class Solution {

    public static void main(String[] args) {
            Scanner sc=new Scanner(System.in);
            System.out.println("================================");
            for(int i=0;i<3;i++){
                String s1=sc.next();
                int x=sc.nextInt();
                //Complete this line
              
                System.out.printf("%-15s%03d%n", s1, x);
            }
            System.out.println("================================");

    }
}
"%-15s" means that within 15 blank space, the String "s1" will be filled in the left.
(fill in the blanks from the left) "%03d" means that within 3 0s,
the integer"x" will be filled in the right.(fill in the zeros from the right).
```
<<<<<<< HEAD
=======

[3. Java Loops II](https://www.hackerrank.com/challenges/java-loops/problem)

```java
import java.util.*;
import java.io.*;

class Solution{
    public static void main(String []argh){
        Scanner in = new Scanner(System.in);
        int t=in.nextInt();
        int prev=0,p=0;
        for(int i=0;i<t;i++){
            int a = in.nextInt();
            int b = in.nextInt();
            int n = in.nextInt();
            //write your code
            for(int j=0;j<n;j++){
                prev+=(int)Math.pow(2,j)*b;
                System.out.print(prev+" ");
            }
            System.out.println();
        }
        in.close();
    }
}
```
>>>>>>> e6c04b8 (3rd problem added)
