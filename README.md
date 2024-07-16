# Basic-java

//print Hello world 
//Using main method print Hello world
class A
{
  public static void main(String[] args)
  {
  System.out.println("Hello world");  	//Hello world
  }
}
//method calling
//In any class atleast one main method required to run the program
//Here starting main method is calling m1() method by using the syntax :classname.methodname()
class B
{
 public static void main(String[] args)
  {
  System.out.println("main starts");		
  B.m1();
  }
 public static void m1();
 {
 System.out.println("main ends");
 }
}
//without main function calling another class main
//here one file doesnot consist of two classes
//so create two seperetae files with class name c and class name D
class C
{
  public static void m1()
  {
  System.out.println("m1 class");
  }
}
//Another file name created otherwise it will through error
class D
{
  public static void main(String[] args)
  {
  System.out.println("main starts");
  C.m1();
  System.out.println("main ends");
  }
}
//variables are three types -local,static,non static
//Declaring a local variable
//a local variable must be declared inside a method
//local variable must be used in which method it is declared
//local varibles must be intialized with a value otherwise it will give compile time error
class  E
{
	public static void main(String[] args) 
	{
		int a=10;
		System.out.println(a);
	}
}
//declaring static variable using classname
class F 
{
	static int i=20;
	public static void main(String[] args) 
	{
		System.out.println(F.i);
	}
}
//declaring a static variable using object loading
/*object creation syntax is
   classname variablename=new classname()
   variable name.i=value; */
class F 
{
	static char i;
	public static void main(String[] args) 
	{
		F x1=new F();
		x1.i='s';
		System.out.println(x1.i);
	}
}
//declaring static value using object creation
//creating multiple object creation it will store the value only one value at a time 
//Here declaring static int value by creating thre objects,in static it display the same value three times 
class G
{
	static int i;
	public static void main(String[] args) 
	{
		L s=new L();
		s.i=10;
		L m=new L();
		m.i=40;
		L n=new L();
		n.i=9;
		System.out.println(s.i);  //9
		System.out.println(m.i);  //9
		System.out.println(n.i);  //9
	}
}
//dellaring a multiple static values 
class H 
{
	static int i;
	static char j;
	public static void main(String[] args) 
	{
		L s=new L();
		s.i=10;
		L m=new L();
		m.i=40;
		L n=new L();
		n.j='r';
		System.out.println(s.i);	//40
		System.out.println(m.i);	//40
		System.out.println(n.j);	//r
	}
}
//delaring a static value for character data type giving integer value
//it will not throw any error
//but that block of statement will be skipped
class I 
{
	static int i;
	static char j;
	public static void main(String[] args) 
	{
		L s=new L();
		s.i=10;
		L m=new L();
		m.i=40;
		L n=new L();
		n.j=9;
		System.out.println(s.i);	//40
		System.out.println(m.i);	//40
		System.out.println(n.j);	//here this lock will not be executed and empty space created and come out of the program
	}
}
class J 
{
	static int i;
	static char j;
	public static void main(String[] args) 
	{
		L s=new L();
		s.i=10;
		L m=new L();
		m.i=40;
		L n=new L();
		n.j='s';
		System.out.println(s.i);
		System.out.println(m.i);
		System.out.println(n.j);
	}
}
//declaring  and intializing a staic variable outside the block
class K 
{
	static int i=1;
	static char j='d';
	public static void main(String[] args) 
	{
		L s=new L();
		s.i=10;
		L m=new L();
		m.i=40;
		L n=new L();
		n.j='s';
		System.out.println(s.i);	//40
		System.out.println(m.i);	//40
		System.out.println(n.j);	//d
	}
}
//declaring and intializing without using classname and object creation
class M 
{
	static int i=1;
	static char j='s';
	public static void main(String[] args) 
	{
		
		System.out.println(i);		//1
		System.out.println(i);		//1
		System.out.println(j);		//s
	}
}
//declaring and intializing with using class name
class N 
{
	static int i=45;
	static char j='g';
	public static void main(String[] args) 
	{
		System.out.println(L.i);	//45
		System.out.println(L.i);	//45
		System.out.println(L.j);	//g
	}
}
//hence static variable can be intialized using class name or object name but most of the cases class name is suggested to better understating
//in case of non static varible compulsory we should create an object otherwise it will throw an error
//delaring a non static variable
class O 
{
	int i=1;
	char j='d';
	public static void main(String[] args) 
	{
		L s=new L();
		s.i=10;
		L m=new L();
		m.i=40;
		L n=new L();
		n.j='s';
		System.out.println(s.i);		//10
		System.out.println(m.i);		//40
		System.out.println(n.j);		//s
	}
}
//oprators are arithematic,logical,unary,terinary operators
//Arithematic operators 
//in java there are totally five operators
//they are +,-,/,*,%
//'+' operator is used to add two or more values
//'-' operator is used to subtract two or more values
//'*' operator is used to  multiply the values
//'/' division operator is used to remove last digit in the number and also it divides the numbers and returns the quotient value
//'%' operator is used to take a last digit from the number and also it will return the remainder between the numbers

//using simple addition operator using direct values
class P
{
	public static void main(String[] args) 
	{
				
		System.out.println(7+7);	//14
	}
}
//using simple by using local variables
class Q 
{
	public static void main(String[] args) 
	{
		int a=7;
		int b=12;
		System.out.println(a+b);	//19
	}
}
//program to perform all arithmatic operations
class R
{
	public static void main(String[] args) 
	{
		int a=14;
		int b=5;
		System.out.println(a+b);	//19
    		System.out.println(a-b);	//9
		System.out.println(a*b);	//70
		System.out.println(a/b);	//2
		System.out.println(a%b);	//4

	}
}
// Logical Operators
//Here in this the logical operators are logical AND (&&),logical or(||) ,and finally logical Not(!)
//these logical operators are used to



