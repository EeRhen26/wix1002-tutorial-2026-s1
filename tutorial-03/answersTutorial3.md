# Tutorial 03 — Answers

### Question 1a

```java
int num = 3*8;
if(num == 27){
    System.out.println("3 x 8 = 27");
}
else{
    System.out.println("3 x 8 != 27");
}
```
### Question 1b

```java
Scanner input = new Scanner(System.in);
int num = input.nextInt();
if(num % 2 == 0){
    System.out.println("It is even number.");
}
else{
    System.out.println("It is odd number.");
}
```

### Question 1c

```java
Scanner input = new Scanner(System.in);
char user = input.next().charAt(0);
if(Character.isUpperCase(user)){
    System.out.println("It is capital letter.");
}
else{
    System.out.println("It is not capital letter.");
}
```

### Question 1d

```java
Scanner input = new Scanner(System.in);
System.out.println("Enter first string: ");
String entry1 = input.next();
System.out.println("Enter second string: ")
String entry2 = input.next();
char det1 = entry1.charAt(0);
char det2 = entry2.charAt(0);
if(det1 - det2 >= 0){
    System.out.println(entry1);
    System.out.println(entry2);
}
else{
    System.out.println(entry2);
    System.out.println(entry1);
}
```
### Question 1e

```java
Scanner input = new Scanner(System.in);
System.out.println("Enter the number from 1 to 7");
int day = input.nextInt();
day = day - 1; 
if(day == 0){
    System.out.println("Sunday");
}
else if(day == 1){
    System.out.println("Monday");
}
else if(day == 2){
    System.out.println("Tuesday");
}
else if(day == 3){
    System.out.println("Wednesday");
}
else if(day == 4){
    System.out.println("Thursday");
}
else if(day == 5){
    System.out.println("Friday");
}
else if(day == 6){
    System.out.println("Saturday");
}
else {
    System.out.println("Error");
}
```

### Question 2a

(num1 = num2) ---> (num1 == num2)

### Question 2b

(x>y>z) ---> (x>y && x>z)

### Question 2c

else (s1 != s2) ---> else

### Question 2d

if x>0 or y>0; ---> if (x>0 || y>0)

### Question 3a

\#\#\#\#\# \
$$$$$

### Question 3b

\#\#\#\#\# \
$$$$$

### Question 3c

(No output)

### Question 3d

`$$$$$`

### Question 4

```java
Scanner input = new Scanner(System.in);
System.out.println("Enter 3 integers: ");
int num1 = input.nextInt();
int num2 = input.nextInt();
int num3 = input.nextInt();
if(num1 > num2 && num1 > num3){
    System.out.println("The biggest number is " + num1);
}
else if(num2 > num1 && num2 > num3){
    System.out.println("The biggest number is " + num2);
}
else{
    System.out.println("The biggest number is " + num3);
}
```

### Question 5

```java
/* I'm assuming that years such as 100, 200, 300, 400 are not leap years because they are divisible by 100 as they question states not */
Scanner input = new Scanner(System.in);
System.out.print("Enter year (in integer form) : ");
int year = input.nextInt();
if(year % 400 == 0){
    System.out.println("It is a leap year.");
}
else{
    if(year % 100 == 0){
        System.out.println("It is not a leap year.");
    }
    else{
        if(year % 4 == 0){
            System.out.println("It is a leap year.");
        }
        else{
            System.out.println("It is not a leap year.");
        }
    }
}
```