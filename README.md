# Basic-java
//print Hello world 
class A
{
  public static void main(String[] args)
  {
  System.out.println("Hello world");
  }
}
//method calling
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
  
