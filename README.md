# assignment3.6
 Que.1)
 Yes we can overload method with same return type but the argument list should be diffrent but 
method overloading is not possible by changing the return type of the method only because of ambiguity.
Basically method overloading is ,If a class has multiple methods having same name but different in parameters, it is known as Method Overloading.
it can be done be achieved by either changing data type or changing number of argument. 

In code below we passed two int and summed their result in method with return type as int , but in another method we passed we
two char's and returned them with add by adding. 
in case1 it gave me addition of two ints and in second it gave me addition of ASCII values of char's passed. hence,
Here we can see that the method sum has the same return type but argument list is different one gives actual sum and 
the other gives the ascii value of the character.

---CODE----
 import java.util.Scanner;
public class acad2 {
	public static int sum(int a , int b) //create method sum to sum two int
    {
        return a+b;  //return sum
         
    }
public static int  sum(char c,char t) //method with return type as int but sum char
    {
    	int n =(int)c;
    	int p=(int) t;
         return n+p;        //return sum;      
    }
	
    public static void main(String args[])
	{
		Scanner sc= new Scanner(System.in);
		
		int a = sc.nextInt(); //scan input from user
		int b = sc.nextInt();
		System.out.println("output");
		System.out.println(sum(a,b));//sum with integer type as input
		System.out.println(sum('c','r'));//	sum of ASCII values
		}
	}
    
    
    Que.2) Write a program in java using Arrays, that sorts the element in descending order.
    
package acadgild;
import java.util.*;

	public class acad
	{
	   public static void main(String args[])
	   {
	      Scanner sc=new Scanner(System.in);
	      int arr[]=new int[5];
	      for(int i=0;i<5;i++)
	      {
	    	  arr[i]=sc.nextInt();
	      }
	      Arrays.sort(arr);
	      for(int i=0;i<5;i++)
	    	  
	      {
	    	  System.out.println(arr[i]);
	      }
	      
	   }
	 
	  
	}
