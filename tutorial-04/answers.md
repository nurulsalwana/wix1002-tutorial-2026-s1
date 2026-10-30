# Tutorial 04 — Answers

## Part I

### Question 1

Write statements for each of the following

a. Find the largest integer n so that n3 is less than 2000.
```java
public class T4Q1a {
    public static void main(String[] args) {
        int n = 0;
        int cubeN = 0;

        while (cubeN < 2000) {
            n++;
            cubeN = n * n * n;
        }

        System.out.println("The largest integer n such that n^3 is less than 2000 is: " + (n - 1));
    }   
}
```

b. Display the square number of the first twelve integers starting from 1.
```java
public class T4Q1b {
    public static void main(String[] args) {
        
        for (int i = 1; i <= 12; i++) {
            int squared = i * i;
            System.out.println("The square of " + i + " is " + squared);
        }
    }
}
```

c. Display a 4-by-5 matrix using random number within 0 to 100.
```java
import java.util.Random;

public class T4Q1c {
    public static void main(String[] args) {
        Random rand = new Random();

        int counter = 0;
     stop: {
        for (int row = 1; row <= 4; row++) {
            for (int column = 1; column <= 5; column++) {
                int randomNum = rand.nextInt(100) + 1; 
                System.out.print(randomNum + "\t");
                counter++;
            }
            System.out.println();
        }
     }
    }
}
```

d. Compute the sum of numbers from 1 to a given number.
```java
import java.util.Scanner;

public class T4Q1d {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);

        System.out.print("Enter a number: ");
        int num=sc.nextInt();

        int sum=0;

        for (int i=1; i<=num; i++) {
            sum += i;
        }

        System.out.println("Sum of numbers from 1 to " + num + " is: " + sum);
    }
}
```

e. Compute the sum of the series: 1/25+2/24+3/23 … + 25/1 in two decimal
places.
```java
public class T4Q1e {
    public static void main(String[] args) {

        double sum=0;

        for (double numerator=1; numerator<=25; numerator++) {
            sum += numerator/(26-numerator);
        }
        System.out.printf("Sum: %.2f", sum);
    }

}
```

### Question 2

Correct the error for the following statements.
```java
a.
for (x = 10; x > 0; x--)
    sum += x;           

//should be x-- since the condition (x>0)(decrease)

b.
do{
    x += 2;
    y += x;
    System.out.println(x + " and " + y);
}while (x < 100);

// brackets and semicolon(last line) missing
c.
for ( x==1, y==20; x < y, x++, y-=2);
 System.out.println(x + " " + y);

 //& should be replaced with +

d.
i =1;
while(i<10) {
    if (i==10){
        System.out.println("Program End");
    }
    i++;
}

//no increament for i, causing infinite loop
```

### Question 3
Write the statements that display the first ten values of the Fibonacci sequence. Given the formula f1 = 1, f2 =1, fn = fn-1 + fn-2.
```java
public class T4Q3 {
    public static void main(String[] args) {
            
        int f1 = 1;
        int f2 = 1;

        System.out.print(f1 + " " + f2);

            for (int counter = 3; counter <= 10; counter++) {
                int sum = f1 + f2;
                System.out.print(" " + sum);

                f1 = f2;
                f2 = sum;

        }
    }
}
```
### Question 4
Write the statements that display the string in reverse order. (use String.length() to get the length of the string)

```java
import java.util.Scanner;

public class T4Q4 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter a word: ");
        String str = sc.nextLine();

        for (int i = str.length() - 1; i >= 0; i--) {
            System.out.print(str.charAt(i));
        }
    }
}
```