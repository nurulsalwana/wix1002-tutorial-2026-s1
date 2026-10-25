# Tutorial 03 — Answers

## Part I

### Question 1

Write statements for each of the following
a. Determine whether 3x8=27.

```java
answer = 3 * 8;

if answer == 27 {
    System.out.println("The equation is true.")
} else {
    System.out.println("The equation is false.")
}
    
```

b. Determine whether an input integer is an odd number or even number.

```java
if (number % 2 == 0){
    System.out.println("The number is even.");
} else {
    System.out.println("The number is odd.")
}
```

c. Determine whether a character is a capital letter.

```java
char letter = 'A' ;

if (Character.isUpperCase(letter)) {
    System.out.print(letter + "is a capital letter.");
} else {
    System.out.print(letter + "is not a capital letter.");
}
```

d. Display two strings in alphabetical order ignoring their case.

```java
String first = "apple";
String second = "banana";

int order = first.compareToIgnoreCase(second);

if (order < 0) {
    System.out.println(first + "," + second);
} else if (order > 0){
    System.out.println(second + "," + first);
} else {
    System.out.println("Equal content");
}
```

e. A switch statement that display Sunday, Monday, .., Satudary if the input is 0,
1, …, 6.

```java
switch (day) {
    case 0 :
        System.out.println("Sunday");
        break;
    case 1 :
        System.out.println("Monday");
        break;
    case 2 :
        System.out.println("Tuesday");
        break;
    case 3 :
        System.out.println("Wednesday");
        break;
    case 4 :
        System.out.println("Thursday");
        break;
    case 5 :
        System.out.println("Friday");
        break;
    case 6 :
        System.out.println("Saturday");
        break;
    default:
        System.out.println("Invalid input. Enter 0 to 6 only");
}
```

### Question 2

 Correct the error for the following statements.

 ```java
a.
if (num1 == num2){             //comparison operator
System.out.println("Number 1 is equal to number 2.");
}

b.
if (x > y && y > z) {          // must be two separate comparisons
 System.out.println("x is the largest number");
}

c.
String s1, s2;
if (s1.equals(s2)) {
    System.out.println("They are equal strings.");
} else {
 System.out.println("They are not equal strings.");
}

d.
if (x>0 || y>0) {           //should be brackets instead of semicolon
 System.out.println("Either x or y is positive");
}
```

### Question 3

3. Write the output for the following statements when x=9 and y=10
a.

```java
if (x < 10)         //true
if (y > 10)         //false
System.out.println("*****");    //skipped
else
System.out.println("#####");
System.out.println("$$$$$");

output:
#####
$$$$$


b.
if (x < 10) {
if (y < 10)
System.out.println("*****");
else{
System.out.println("#####");
System.out.println("$$$$$");
}}

output:
#####
$$$$$


c.
if (x < 10) {
if (y < 10)         //no '{'
System.out.println("*****");
System.out.println("#####");
}
else {
System.out.println("$$$$$");
}

output:
(No output produced, missing bracket)


d.
if (x > 10) {
if (y > 10) {
System.out.println("*****");
System.out.println("#####"); }
else
System.out.println("$$$$$");
}

output:
$$$$$
```

### Question 4
Write the java statements that used the if statement to find the biggest number among
three given integers.

```java
int number1 = 23;
int number2 = 5;
int number3 = 15;

if (number1 > number2 && number1 > number3) {
    answer = number1;
} else if (number2 > number1 && number2 > number3) {
    answer = number2;
} else {
    answer = number3;
}

print(answer + "is the biggest number")
```

### Question 5
Write the java statements that determine whether the Leap year. A Leap year is
divisible by 4 but not by 100. However, a Leap year is also divisible by 400.

```java
year = 2024;

if (((year % 4 == 0) && (year % 100 != 0)) || (year % 400 == 0)) {
    print(year + "is a leap year.");
} else {
    print(year + "is not a leap year.");
}
```
