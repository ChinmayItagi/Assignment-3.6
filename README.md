Can you overload a method with the same return type? Explain your
answer with proper logic.
  
  Yes we can overload method with same return type but the argument list should be diffrent. If it is the case that arguments are same as that of the other then aleast the sequence of the arguments should be changed.
  Method Overloading means to have two or more methods with same name in the same class with different arguments. The benefit of method overloading is that it allows you to implement methods that support the same semantic operation but differ by argument number or type.

Important Points

Overloaded methods MUST change the argument list
Overloaded methods CAN change the return type
Overloaded methods CAN change the access modifier
Overloaded methods CAN declare new or broader checked exceptions
A method can be overloaded in the same class or in a subclass.


public class Main {
	public static int sum(int a , int b)
    {
		return a+b; 
    }
    public static int  sum(char c)  
    {
    	int n =(int)c;
         return n;
    }
	
	public static void main(String args[])
	{
		Scanner sc= new Scanner(System.in);
		
		int a = sc.nextInt();
		int b = sc.nextInt();
		System.out.println("output");
		System.out.println(sum(a,b));//sum with integer type as input
		System.out.println(sum('a'));//	sum with char type as input
		}
	}
  Here we can see that the method sum has the same return type but argument list is different one gives actual sum and the other gives the ascii value of the character.
