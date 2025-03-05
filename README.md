# Java

----------------ARRAYLIST------------

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner sc=new Scanner(System.in);
	    ArrayList <Integer> list=new ArrayList<>(10);
	    list.add(64);
		System.out.println(list);
		
		ArrayList<Integer> list2=new ArrayList<>(10);
		for(int i=0;i<8;i++){
		    int res=sc.nextInt();
		    list2.add(res);
		}
		System.out.println(list2);
	}
}
NOTE:Never name a class the same as a Java built-in class.
-------------------------------------------------------

-------------IF AND ELSE------------------

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner sc=new Scanner(System.in);
	    int n=sc.nextInt();
	    int salary=sc.nextInt();
	    if (salary>50000){
	        salary+=1000;
	    }
	    if(salary>25000){
	        salary+=2000;
	    }
	    else{
	        salary+=4000;
	    }
	    if(salary>60000){
	        salary+=500;
	    }
	    else if(salary>7000){
	        salary+=1000;
	    }
	    else{
	        salary+=1500;
	    }
	    System.out.println(salary);
	}
}
--------------------------------------/

----------------WHILE AND DO WHILE-------------------

	    while(salary>5000){
	        salary+=4000;
	    }
     import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner sc=new Scanner(System.in);
	    int salary=sc.nextInt();
	    do{ 
	        salary+=400;
	    }while(salary<2000);
	    System.out.println(salary);
	}
}

-------------------------------------------/
import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner sc=new Scanner(System.in);
	    int a=sc.nextInt();
	    System.out.println(a);
	    float b=sc.nextFloat();
	    System.out.println(b);
	    String c=sc.next();
	    System.out.println(c);
	    long d=sc.nextLong();
	    System.out.println(d);
	    double e=sc.nextDouble();
	    System.out.println(e);
	    byte f=sc.nextByte();
	    System.out.println(f);
	}
}
--------------------------------------------/
