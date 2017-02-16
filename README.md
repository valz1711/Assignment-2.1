
1)
  public class acad {
    public static void main(String[] args){
      int d=5;                             //assigning value to integer d
      int e=10;                            //assigning value to integer e
      System.out.println(d+e);             //Printing the sum
    }
  }
  
2)
  import java.util.Scanner;
  public class acad {
    public static void main(String[] args){
      Scanner s=new Scanner(System.in);
      int d=s.nextInt();                //accepting and assigning the value of first integer from user
      int e=s.nextInt();                //accepting and assigning the value of second integer from user
      System.out.println(d+e);          //printing the sum
    }
  }
  
3)
  import java.util.Scanner;
  public class acad {
    public static void main(String[] args){
      Scanner s=new Scanner(System.in);
      int d=s.nextInt();         //accepting value of first integer from user
      int e=s.nextInt();        //accepting value of second integer from user
      System.out.println("First number is:"+d);
      System.out.println("Second number is:"+e);
      sum(d,e);
    }
    public static void sum(int a,int b){
      System.out.println("Sum is:"+(a+b));
    }//method for calculating and displaying the sum
  }
  
4)
  import java.util.ArrayList;
  import java.util.Scanner;
  public class acad {
    public static void main(String[] args){
      Scanner s=new Scanner(System.in);
      int a=s.nextInt();            //accepting value of first integer from user
      int b=s.nextInt();            //accepting value of second integer from user
      ArrayList<Integer> odd=new ArrayList<Integer>();
      ArrayList<Integer> even=new ArrayList<Integer>();
      for(int i=a;i<=b;i++){
        if(i%2==0)
          even.add(i);               //Storing even numbers in arraylist
        else
          odd.add(i);                //Storing odd numbers in arraylist
      }System.out.println("Odd numbers are:\n");
      for(int i:odd)
        System.out.print(i+" ");
      System.out.println("\nEven numbers are:\n");
      for(int i:even)
        System.out.print(i+" ");
    }
  }

5)
  import java.util.Scanner;
  public class acad {
    public static void main(String[] args){
      Scanner sc=new Scanner(System.in);
      int n=sc.nextInt();                                     //accepting the number
      System.out.println("Input: "+n);
      System.out.println("O/p:");
       for(int i=1;i<=10;i++){
        System.out.println(n+" * "+i+" = "+(n*i));            //displaying table of given number
       }
    }
  }
  
6)
  import java.util.Scanner;
  public class acad {
    public static void main(String[] args){
      Scanner s=new Scanner(System.in);
      int a=s.nextInt();       //Accepting 3 numbers from the user
      int b=s.nextInt();
      int d=s.nextInt();
      sum(a,b);
      sum(a,b,d);
    }     
    //Method overloading
    public static void sum(int a,int b){
      System.out.println("Sum of first 2 numbers is:"+(a+b));
    }
    public static void sum(int a,int b,int d){
      System.out.println("Sum of all 3 numbers is:"+(a+b+d));
    }
  }
  
7)
    import java.util.Scanner;
    public class acad {
  	  public static String getstring(String a , String b)
      {
		    String s=a+" "+b;
		    return s;
      }
      public static String  getstring(String c)  
      {
    	  String s1=c;
        return c;
      }
	    public static void main(String args[])
	    {
		    Scanner s= new Scanner(System.in);
		    String a = s.nextLine();
		    String b= s.nextLine();
		    String c="s";
		    System.out.println("String");
		    System.out.println(getstring(a,b)); //2 String as input
		    System.out.println(getstring(c));   //1 String as input
		  }
	  }
 
 8)
  import java.util.Arrays;
  import java.util.Scanner;
  public class acad {
    public static void main(String[] args){
      Scanner sc=new Scanner(System.in);
      int n=sc.nextInt(); //size of array
      int[] arr=new int[n];
      for(int i=0;i<n;i++){
        arr[i]=sc.nextInt();
      }
      Arrays.sort(arr);               //sorting array
      for(int i=arr.length-1;i>=0;i--){
        System.out.print(arr[i]+" "); // displaying sorted reverse ordered array elements
      }
    }
   } 
