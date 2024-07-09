# Basic-java
//print Hello world 
//Using main method print Hello world
class A
{
  public static void main(String[] args)
  {
  System.out.println("Hello world");
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
class C
{
  public static void m1()
  {
  System.out.println("m1 class");
  }
}
class D
{
  public static void main(String[] args)
  {
  System.out.println("main starts");
  c.m1();
  System.out.println("main ends");
  }
}
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


  


