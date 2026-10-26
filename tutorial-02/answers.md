# Tutorial 02 — Answers

## Part I

### Question 1

```java
public class question1 {

    public static void main(String[] args) {
        System.out.println("Q1 A:");
        System.out.println("Faculty of Computer Science ");
        System.out.println("and Information Technology");
        System.out.println("\nQ1 B:");
        System.out.println("Faculty\nof\nComputer\nScience\nand\nInformation\nTechnology");
    }
}
```
### Question 2
```java
public class question2 {
    public static void main(String[] args) {
       System.out.println("\"SDN\"-Software Defined Networking");
    }
}
```

### Question 3
``` text
a. System.out.println("Java Programming");
b. System.out.println("Introduction to Java!");
c. System.out.println("\\t is the horizontal tab character");
d. System.out.println("Java is case sensitive!" );
```

### Question 4
``` text
a. Declare a variable that used to store the value of a matric number.
ans: String matricNo;
//flexible, exclusive

b. Declare a variable that used to store the value of π.
ans: double pi;

c. Initialize a variable named M with the value set to false.
ans: boolean M = "false";

d. Initialize a variable named P with the value set to 8800000000.
ans: long P = 8800000000;

e. Initialize a variable named letter with the value set to U.
ans: char letter = 'U';

f. Declare a constant variable named PRO. The value of the constant variable is Java. 
ans: final String PRO = "Java";
```

### Question 5
``` text
a.
double AMOUNT = 32.5;
AMOUNT += 10;
System.out.println("The amount is " + AMOUNT);

b.
String chapter = "Summary";
System.out.println(chapter);

c.
int num1 = 5;
int num;
num++;  //have to initialize value before operation
num1 = num;

d.
double num = 3000;
System.out.printf("%4.2f\n", num);

e.
String contact;
Scanner keyboard = new Scanner(System.in);
contact = keyboard.nextLine();
```

### Question 6
```java
import java.util.Scanner;

public class question6 {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.print("Enter diameter: ");
        double diameter = input.nextDouble();
        
        double circumference = Math.PI * diameter;

        System.out.printf(java.util.Locale.US, "The circumference of the circle is : %.3f\n", circumference);
    }
}

```

### Question 7
```java
import java.util.Scanner;

public class question7 {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.print("Enter value in inch: ");
        double inch = input.nextDouble();
        
        double convertedValue = inch * 2.54 / 100;

        System.out.printf(java.util.Locale.US, "%.2f inches = %.2f meters\n", inch, convertedValue);
    }
    
}
```

## Part II

### Question 1

Write your answer here.
