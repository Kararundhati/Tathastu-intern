1.//basic calculator operation
import java.util.*;
import java.lang.*;
import java.io.*;

/* Name of the class has to be "Main" only if the class is public. */
class calculator
{
	public static void main (String[] args) throws java.lang.Exception
	{
		int ch,a,b;
		Scanner s=new Scanner(System.in);
		ch=s.nextInt();
		a=s.nextInt();
		b=s.nextInt();
		switch(ch)
		{
			case 1:
		System.out.println(a+b);
		break;
		case 2:
		System.out.println(a-b);
		break;
		case 3:
System.out.println(a*b);
break;
		case 4:
		System.out.println(a/b);
		break;
		case 5:
		System.out.println(a%b);
		break;
		default:
		System.out.println("enter valid case");
	
	}
}
}

2.//fiboonaci series 1to n
import java.util.*;
import java.lang.*;
import java.io.*;

/* Name of the class has to be "Main" only if the class is public. */
class fibbonaci
{
	public static void main (String[] args) throws java.lang.Exception
	{
		int a=0,b=1,c,i,n;
		System.out.println(a+"\n"+b);
		Scanner s=new Scanner(System.in);
		n=s.nextInt();
		for(i=2;i<n;i++)
		{
			c=a+b;
			System.out.println(""+c);
		   a=b;
		   b=c;
	   }
   }
}
3.//factorial of a number
import java.util.*;
import java.lang.*;
import java.io.*;

/* Name of the class has to be "Main" only if the class is public. */
class fact
{
	static int factorial(int n){
		if(n==0)
		return 1;
		else
return(n*factorial(n-1));
}
	public static void main (String[] args) throws java.lang.Exception
	{
		int i,n,f=1;
		Scanner s=new Scanner(System.in);
		n=s.nextInt();
		f=factorial(n);
		
		System.out.println("factorial of num is"+f);
	}

}
4.//whether the given string is palindrome or not
import java.util.Scanner;
 
class ChkPalindrome
{
   public static void main(String args[])
   {
      String str, rev = "";
      Scanner sc = new Scanner(System.in);
 
      System.out.println("Enter a string:");
      str = sc.nextLine();
 
      int length = str.length();
 
      for ( int i = length - 1; i >= 0; i-- )
         rev = rev + str.charAt(i);
 
      if (str.equals(rev))
         System.out.println(str+" is a palindrome");
      else
         System.out.println(str+" is not a palindrome");
 
   }
}
5.//calculate permutation and combination of 2number
import java.util.*;
import java.lang.*;
import java.io.*;

class A
{
	double fact(double n)
	{
             	    double f=1;
	    for(int i=1;i<=n;i++)
	    {
	   	   f=f*i;
 	    }
  	      return f;	 
	}
	public static void main(String arg[])	
	{
	A a=new A();	
	Scanner sc=new Scanner(System.in);
	System.out.println("Enter value of n");
               int n=sc.nextInt();
	System.out.println("Enter value of r");
               int r=sc.nextInt();
	if(n>=r)
	{
		double com=a.fact(n)/(a.fact(n-r)*a.fact(r));
		double per=a.fact(n)/a.fact(n-r);	
		System.out.println("The value of "+n+"p"+r+" is : "+per);	
		System.out.println("The value of "+n+"c"+r+" is : "+com);
	}
	else
			System.out.println("Please enter n>=r");		
	}
}
6.//print diamond 💎pattern
import java.util.Scanner;
public class Diamond
{
    public static void main(String args[]) 
    {
        int n, i, j, space = 1;
        System.out.print("Enter the number of rows: ");
        Scanner s = new Scanner(System.in);
        n = s.nextInt();
        space = n - 1;
        for (j = 1; j <= n; j++) 
        {
            for (i = 1; i <= space; i++) 
            {
                System.out.print(" ");
            }
            space--;
            for (i = 1; i <= 2 * j - 1; i++) 
            {
                System.out.print("*");                
            }
            System.out.println("");
        }
        space = 1;
        for (j = 1; j <= n - 1; j++) 
        {
            for (i = 1; i <= space; i++) 
            {
                System.out.print(" ");
            }
            space++;
            for (i = 1; i <= 2 * (n - j) - 1; i++) 
            {
                System.out.print("*");
            }
            System.out.println("");
        }
    }
}
7.//reverse the letter present in the given string
import java.util.*;
import java.lang.*;
import java.io.*;

public class stringreverse 
{
	public static void main(String[] args) 
	{
	String str = "Welcome To coding";
	String[] strArray = str.split(" ");
	for (String temp: strArray){
		System.out.println(temp);}
		for(int i=0; i<3; i++)
		{ 
	char[] s1 = strArray[i].toCharArray(); for (int j = s1.length-1; j>=0; j--){
		System.out.print(s1[j]);
		}
		System.out.print(" ");
		}
		}
		}

8.//given array is mirror inverse or not
import java.util.*;
import java.lang.*;
import java.io.*;
public class mirrorinverse
{
public static void main(String args[])
{
int count=0;
int arr[]={3,4,5,0,1,2};
for(int i=0;i<arr.length;i++)
{
if(arr[arr[i]]==i);
{
	count++;
}
}
if(count!=0)
{
System.out.println("the given array is mirror inverse");
}
else
{
System.out.println("the given qrray is not mirror inverse");
}
}
}
9.//remove elements from an array list
import java.util.ArrayList;  
  
public class RemoveMethod {  
   public static void main(String[] args) {  
      
      ArrayList<String> arr = new ArrayList<String>(5);   
      arr.add("abhit");  
      arr.add("aru");  
      arr.add("apu");  
      arr.add("rohan");  
      System.out.println("The list of the size is: " + arr.size());  
      for (String name : arr) {  
         System.out.println("Name is: " + name);  
      }    
      arr.remove(1);  
      System.out.println("\nAfter removing the element the size of the ArrayList is: " + arr.size());  
      for (String name : arr) {  
         System.out.println("Name is: " + name);  
      }  
   }  
}  

10.//transpose of a given matrix
public class Transpose  
{  
    public static void main(String[] args) {  
        int rows, cols;  
          
          int a[][] = {  
                          {1, 2, 3},  
                          {4, 5, 6},  
                          {7, 8, 9}  
                       };  
            
          rows = a.length;  
        cols = a[0].length;  
        int t[][] = new int[cols][rows];  
        for(int i = 0; i < cols; i++){  
            for(int j = 0; j < rows; j++){   
                t[i][j] = a[j][i];  
            }  
        }  
          
        System.out.println("Transpose of given matrix: ");  
        for(int i = 0; i < cols; i++){  
            for(int j = 0; j < rows; j++){  
               System.out.print(t[i][j] + " ");  
            }  
            System.out.println();  
        }  
    }  
}  


//Total 10 interesting programming 👍



