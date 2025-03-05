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
import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner sc=new Scanner(System.in);
	    int a=78;
	    System.out.println(a);
	    float b=78.98f;
	    System.out.println(b);
	    String c="ayt";
	    System.out.println(c);
	    long d=73647647;
	    System.out.println(d);
	    double e=789827.8267;
	    System.out.println(e);
	    boolean g=true;
	    float h=(int)(b);
	    System.out.println(h);
	    byte j;
            int k =102456;
            j=(byte)(k);
            System.out.println(j);
	    
	}
}

NOTE: // string cannot be converted to int
// int to byte takes only last two digits
// int*byte=int
// float*double=double
//char*long=long
----------------------------------------------------

-----------------ARMSTRONG NUMBER--------------------

import java.util.*;
public class Main{
    public static int armstrong(int n){
        int original=n;
        int sum=0;
        while(n!=0){
        int rem=n%10;
        n=n/10;
        sum=sum+rem*rem*rem;
        }
        return sum;
    }
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        int original=n;
        int p=armstrong(n);
        if(p==original){
            System.out.println("It is an armstrong number");
        }
        else{
            System.out.println("It is not an armstrong number");
        }
    }
}


import java.util.*;
public class Main{
    public static boolean armstrong(int n){
        int count=String.valueOf(n).length();
        int og=n;
        double armstrong=0;
        while(n>0){
            int a=n%10;
            armstrong = (int) (armstrong + Math.pow(a, count));
            n=n/10;
        }
        return armstrong==og;
    }
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        if(armstrong(n)){
            System.out.println("It is armstrong");
        }
        else{
            System.out.println("Not armstrong");
        }
   }
}
-------------------------/

import java.util.*;
public class Main{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        int a[]=new int[5];
        for(int i=0;i<a.length;i++){
            a[i]=sc.nextInt();
        }
        func1(a);
        System.out.println(Arrays.toString(a));
        int res[]=func(a);
        System.out.println(Arrays.toString(res));
        }
        public static int[] func(int nums[]){
            nums[0]=99;
            return nums;
        }
        public static void func1(int nums[]){
            nums[0]=98;
    }
}
---------------------------------/

import java.util.*;
public class Main{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        int a[]={1,2,3,4,5,6,67,8,9};
        int start=2;
        int end=9;
        int target=67;
        int ans=linearSearch(a,target,start,end);
        System.out.println(ans);
    }
    public static int linearSearch(int a[],int target,int start,int end){
        if(a.length==0){
            return -1;
        }
        for(start=0;start<end;start++){
            if(a[start]==target){
                return start;
            }
        }
        return-1;
    }
}
---------------------------------------------------/

import java.util.*;
public class Main{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        ArrayList <Integer> list=new ArrayList<>();
        list.add(24);
        list.add(98);
        list.add(18);
        System.out.println(list);
        list.remove(1);
        System.out.println(list);
        list.set(1,16);
        System.out.println(list);
        System.out.println(list.contains(9));
        
    }
}
---------------------------------------------------------/
import java.util.*;
public class Main{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        int a[]=new int[5];
        for(int i=0;i<a.length;i++){
            a[i]=sc.nextInt();
        }
        for(int i=0;i<a.length;i++){
            System.out.println(a[i]+" ");
        }
        for(int x:a){
            System.out.println(x+" ");
        }
        System.out.println(Arrays.toString(a));
    }
}
-----------------------------------------------------------/
