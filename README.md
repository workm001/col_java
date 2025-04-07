# 07.03.25
## 1. Write a java program to check witch one is getter then bettween two numbers; 
### File Name: col_1.java
```java
import java.util.Scanner;
public class whoIsBig{

public static void main(String[] args){
Scanner sc = new Scanner(System.in);

	System.out.print("Enter First Number:");
	int a = sc.nextInt();
System.out.print("Enter Secound Number:");
	int b = sc.nextInt();
	
	if(a > b){
	 System.out.println(a + " is big");
	}else{
	 System.out.println(b + " is big");
	}
}

}
```
## 2. Write a java Program to cheack a number is Amstrong or not;
### File Name: col_2.java

```java 
import java.util.Scanner;

public class Amstrong{


public static void main(String[] args){
	Scanner sc = new Scanner(System.in);
		System.out.print("Enter a Number: ");
		int num = sc.nextInt();
	int num1, num2;
	num2 = num1 = num;
	int rem, sum = 0;
	int noDig  = 0; // have to initialized it or it will thrrow an error showing bellow 
	
	while(num1 != 0){
		noDig++;
		num1 /= 10;
	}
	while(num2 != 0){
		rem = num2%10;
		sum += (int) Math.pow(rem,noDig);
		num2 /= 10;
	}
	if(num == sum){
		System.out.println( num + " is a Amstrong");
	}else{
		System.out.println( num + " is not a Amstrong");
	}
}
}
```
### The Error if not initialized (int noDig) :
```java 
col_2.java:16: error: variable noDig might not have been initialized
		noDig++;
		^
col_2.java:21: error: variable noDig might not have been initialized
		sum += (int) Math.pow(rem,noDig);
		                          ^
2 errors
error: compilation failed

```