# Tutorial 04 — Answers

### Question 1a

```java
int n = 0, cube = 0;
while(cube <2000){
    n=n+1;
    cube = Math.pow(n,3);
}
System.out.println("The largest integer that has cube less than 2000 is "+(n-1));
```
### Question 1b

```java
int square = 0;
for(int i = 1; i<=12, i++){
    square = Math.pow(i,2);
    System.out.println(square);
}
```
### Question 1c

```java
Random choice = new Random();
int num = 0;
for (int i = 0; i<5, i++){
    for (int j = 0; j < 4; j++){
        num = choice.nextInt(101);
        System.out.print(num+"\n");
    }
    System.out.println();
}
```

### Quetion 1d

```java
Scanner input = new Scanner(System.in);
int sum = 0, user = 0;
System.out.print("Enter a number: ");
user = input.nextint();
for (int i = 1; i<=user; i++){
    sum = sum+i;
}
System.out.println(sum);
```

### Question 1e

```java
double sum = 0;
for (double i = 1; i<=25; i++){
    sum = sum + (i/(26-i));
}
System.out.printf(""%.2f%n",sum);
```

### Question 2a

for(x=10;x>0;x++) ---> for(x=0; x<10; x++)

### Question 2b

do
 x += 2;
 y += x;
 System.out.println(x + " and " + y);
while (x < 100)

|
|
|
V

int x = 0, y = 0;
do{
    x+= 2;
    y+= x;
    System.out.println(x+" and "+y);
}while(x<100);


### Question 2c

for ( x==1, y==20; x < y, x++, y-=2);
System.out.println(x & " " & y);
  |
  |
  |
  v
for (int x=1, y=20; x < y; x++, y-=2){
	System.out.println(x + " " + y);
}

### Question 2d

int i =1;
while(i<10) {
 if (i==10)
 System.out.println("Program End");
}

|
|
|
V

int i =1;
while(i<10) {
    if (i==10)
    System.out.println("Program End");
    i++;
}

### Question 3

```java
int num1 = 1, num2 = 1, counter = 1;
while (counter <=5){
    System.out.println(num1);
    System.out.println(num2);
    num1 = num1 + num2;
    num2 = num1 + num2;
    counter = counter + 1;
}
```

### Question 4

```java
char num;
Scanner input = new Scanner (System.in);
System.out.print("Enter a sentence: ");
String user = input.nextLine();
for (int i = 1; i <= user.length; i++){
    num = user.charAt(user.length-i);
    System.out.print(num);
}
```