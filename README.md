
### col_1.java
## Write a java program to check witch one is getter then bettween two numbers; 
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