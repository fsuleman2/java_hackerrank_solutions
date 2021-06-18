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
    }
}
```
[2. Java Output Formatting](https://www.hackerrank.com/challenges/java-output-formatting/problem)

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
[]()

```java

```
[4. Java Datatypes](https://www.hackerrank.com/challenges/java-datatypes/problem)

```java
import java.util.*;
import java.io.*;

class Solution{
    public static void main(String []argh)
    {
        Scanner sc = new Scanner(System.in);
        int t=sc.nextInt();

        for(int i=0;i<t;i++)
        {
            try
            {
                long x=sc.nextLong();
                System.out.println(x+" can be fitted in:");
                if(x>=-128 && x<=127)System.out.println("* byte");
                //Complete the code
                if(x>=-Math.pow(2,15) && x<=Math.pow(2,15)-1)
                {
                    System.out.println("* short");
                }
                if(x>=-Math.pow(2,31) && x<=Math.pow(2,31)-1)
                {
                    System.out.println("* int");
                }
                if(x>=-Math.pow(2,63) && x<=Math.pow(2,63)-1){
                    System.out.println("* long");
                }
            }
            catch(Exception e)
            {
                System.out.println(sc.next()+" can't be fitted anywhere.");
            }
        }
    }
}
```
[5. Java End-of-file](https://www.hackerrank.com/challenges/java-end-of-file/problem)

```java
import java.io.*;
import java.util.*;
import java.text.*;
import java.math.*;
import java.util.regex.*;

public class Solution {

    public static void main(String[] args) {
        /* Enter your code here. Read input from STDIN. Print output to STDOUT. Your class should be named Solution. */
        Scanner sc = new Scanner(System.in);
        int i=1;
        while(sc.hasNext())
        {
            String s = sc.nextLine();
            System.out.println(i+" "+s);
            i++;
        }
    }
}
```
[6. Java String Reverse](https://www.hackerrank.com/challenges/java-string-reverse/problem)

```java
import java.io.*;
import java.util.*;

public class Solution {
//I have use StringBuilder class to reverse a String in java
public static String reverseMethod(String str)
{
    StringBuilder sb = new StringBuilder(str);
    sb.reverse();
        return sb.toString();
}
    public static void main(String[] args) {
        
        Scanner sc=new Scanner(System.in);
        String A=sc.next();
        /* Enter your code here. Print output to STDOUT. */
       String str1 = reverseMethod(A);
       System.out.println(str1.equals(A)?"Yes":"No");
        
    }
}
```
```java
import java.io.*;
import java.util.*;
//I have solved above problem in another way
public class Solution {
    public static void main(String[] args) {
        
        Scanner sc=new Scanner(System.in);
        String A=sc.next();
        //start writing your code
        String rev="";
        int len = A.length();
        for(int i=len-1;i>=0;i--)
        {
            rev+=A.charAt(i);
        }
        System.out.println(A.equals(rev)?"Yes":"No");
        
    }
}
```
[7. Java Substring](https://www.hackerrank.com/challenges/java-substring/problem)

```java
import java.io.*;
import java.util.*;
import java.text.*;
import java.math.*;
import java.util.regex.*;

public class Solution {

    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        String S = in.next();
        int start = in.nextInt();
        int end = in.nextInt();
        for(int i=start;i<end;i++)
        {
            char c=S.charAt(i);
            System.out.print(c);
        }
    }
}
```
