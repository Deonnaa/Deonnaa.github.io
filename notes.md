### [Week 1](https://github.com/SkillDistillery/SD41/blob/main/jfop/README.md)

#### Java Fundamentals of Programming

Day 1
1. Day One System Setup
2. Simple Programs
	1. Programming
```java
//simpleprograms/drills/
//Hello.java

public class Hello {

	public static void main(String[] args) {
		System.out.println("Hello, SD41!");
	}
}
```
*
 	2. The Programming Process
  	3. Programming Languages
  	4. Compiler Errors and Runtime Errors
  	5. Input - Process - Output
  	6. [Labs](https://github.com/SkillDistillery/SD41/blob/main/jfop/SimplePrograms/labs.md)
```java
//Lab1 - HelloName.java
public class HelloName {

	public static void main(String[] args) {
		System.out.println("Hello, Deonna!");
	}
}
```
```java
//Lab2 - TwoPrints.java
public class TwoPrints {

	public static void main(String[] args) {

		System.out.println("Hello,");
		System.out.println("Deonna!");
	}
}
```
```java
//Lab3 - HelloTabs.java
public class HelloTabs {

	public static void main(String[] args) {

		System.out.println("Hello,");
		System.out.println("\t\tDeonna!");
	}
}
```
```java
//Lab4 - HelloStars.java
public class HelloStars {

	public static void main(String[] args) {

		System.out.println("****************");
		System.out.println("*     Hello,   *");
		System.out.println("*    Deonna!   *");
		System.out.println("****************");
	}
}

```

```java
//Lab5 - Testing123.java
public class Testing123 {

	public static void main(String[] args) {

		System.out.println("Testing...");
		System.out.println("\t...1...");
		System.out.println("\t\t...2...");
		System.out.println("\t\t\t...3...");

		//or

		System.out.println("Testing...\n ...1...\n  ...2...\n   ...3...");

	}
}

```   
3. Variables and Constants
   1. Data Types
   2. Variables
```java
//variablesandconstants/drills/VariableNaming.java
public class VariableNaming {

	public static void main(String[] args) {
		int distanceTraveled;
		int radius;
		String fullName;
	}
}
```
*
   3. Variable Naming Rules
   4. Literals
   5. Assignment
```java
//variablesandconstants/drills/Assign.java
public class Assign {

	public static void main(String[] args) {
		double battingAverage = .345;
		double thisYearBa = battingAverage;
		battingAverage = .362; // reassignment
		System.out.println(battingAverage); // 0.362
		System.out.println(thisYearBa); // 0.345

		double battingAverage1 = .345;
		battingAverage1 = .362; // reassignment
		double thisYearBa1 = battingAverage1;
		System.out.println(battingAverage1); // 0.362
		System.out.println(thisYearBa1); // 0.362

	}
}
```
*   
   6. Printing Variables
```java
//variablesandconstants/drills/PrintingExample.java
public class PrintingExample {

	public static void main(String[] args) {
		int i_5 = 5;
		double d_5 = 5.00001;
		char c_5 = '5';

		System.out.println("int 5: " + i_5); // int 5: 5
		System.out.println("double 5: " + d_5); // double 5: 5.00001
		System.out.println("char 5: " + c_5); // char 5: 5
	}
}
```
```java
//variablesandconstants/drills/VariablePrinting.java
public class VariablePrinting {

	public static void main(String[] args) {
		double battingAverage = .345;
		double thisYearBa = battingAverage;
		battingAverage = .362; // reassignment

		System.out.println("battingAverage: " + battingAverage); // battingAverage: 0.362
		System.out.println("thisYearBa: " + thisYearBa); // thisYearBa: 0.345
	}
}

```
*    
   7. [Labs](https://github.com/SkillDistillery/SD41/blob/main/jfop/VariablesAndConstants/labs.md)
```java
//Lab1 - AgeInitial.java
public class AgeInitial {

	public static void main(String[] args) {
		int age = 31;
		char mi;
		mi = 'H';

		System.out.println("James " + mi + " Bond" + ": Age: " + age);
	}
}
```
```java
//Lab2 - StudentScores.java
public class StudentScores {

	public static void main(String[] args) {
		double score1 = 95.0;
		double score2 = 33.3;
		double score3 = 80.0;
		double score4 = 90.0;
		double average;

		average = (score1 + score2 + score3 + score4) / 4;

		System.out.println("Score 1: " + score1);
		System.out.println("Score 2: " + score2);
		System.out.println("Score 3: " + score3);
		System.out.println("Score 4: " + score4);

		System.out.println("The average test score was: " + average);
	}
}
```     
5. Introduction to Methods
	1. Methods
 	2. Calling Methods
```java
//introtomethods/drills/CallingMethods.java
public class CallingMethods {

	public static void main(String[] args) {
		System.out.println("Starting in main");

		System.out.println("main() calling secondMethod()");
		secondMethod();
		System.out.println("main() done calling secondMethod()");

		System.out.println("main() calling thirdMethod()");
		thirdMethod();
		System.out.println("main() done calling thirdMethod()");
		System.out.println("main() finished");
	}

	public static void secondMethod() {
		System.out.println("\tIn secondMethod()");
		System.out.println("\tsecondMethod() finishing");
	}

	public static void thirdMethod() {
		System.out.println("\tIn thirdMethod()");
		System.out.println("\tthirdMethod() calling fourthMethod()");
		fourthMethod();
		System.out.println("\t\tthirdMethod() done calling fourthMethod()");
		System.out.println("\t\tthirdMethod() finishing");
	}

	public static void fourthMethod() {
		System.out.println("In fourthMethod()");
		System.out.println("fourthMethod() finishing");
	}
}
```
*
   	3. The main Method
```java
public static void main(String[] args)
```
*	
 	4. Why Use Methods?
 	5. [Labs](https://github.com/SkillDistillery/SD41/blob/main/jfop/IntroToMethods/labs.md)
```java
//Lab1 - MyName.java
public class MyName {

	public static void main(String[] args) {
		firstName();
		space();
		lastName();
	}

	public static void firstName() {
		System.out.print("Jane");
	}

	public static void lastName() {
		System.out.print("Goodall");
	}

	public static void space() {
		System.out.print(" ");
	}
}
```  
7. Screen Output and Keyboard Input
	1. Screen Output
 	2. Formatting Output
```java
//screenoutputkeyboardinput/drills/Formatting.java
public class Formatting {

	public static void main(String[] args) {
		System.out.println("\\\\ His name was \"Robert Paulson.\" \nYou cry now. //");
	}
}
```
*  
  	3. String Output
```java
//screenoutputkeyboardinput/drills/StringOutput.java
public class StringOutput {

	public static void main(String[] args) {
		// Expected: snow ball
		System.out.println("snow " + " ball");

		// Expected: I could use some space >1 empty line 
		System.out.print("I could use some space\n\n");

		int tensVal = 9;
		int onesVal = 3;

		// Expected: Concatenated number is 93
		System.out.println("Concatenated number is " + tensVal + onesVal);

		// Expected: 12 is another number
		System.out.println(tensVal + onesVal + " is another number");
	}
}
```
*   
 	4. Reading from the Keyboard
```java
//screenoutputkeyboardinput/drills/ScannerInput.java


```
```java
//screenoutputkeyboardinput/drills/ScannerInput.java


```
*     
 	5. Labs
8. Eclipse

Day 2
1. Eclipse
2. Expressions
	1. Expressions: Where the Work Gets Done
 	2. Expression Evaluation: The Result
 	3. Assignment Expressions
 	4. Arithmetic Expressions
 	5. Relational Expressions
 	6. Logical Expressions
 	7. Short-Circuit Operators
 	8. Associativity
 	9. Precedence
 	10. Precedence Order
 	11. Labs
3. Conditionals: if and else
	1. Sequential Execution
 	2. if Statement
 	3. if Syntax
 	4. Code Blocks
 	5. if and else if
 	6. if and else
 	7. Nested Control Statements
 	8. Comparing Strings in Java
 	9. Labs
4. Pair Programming
5. Project: Simple Calculator
6. Project: Mad Libs

Day 3
1. More Expressions
  * Using Boolean Variables
  * Boolean Expressions
  * Assignment Operators
  * Auto-increment
  * The Ternary Conditional Operator
  * Labs
2. Conditionals: switch
  * switch Statements: Multi-Way Decisions
  * break; and default: in switch Statements
  * When to Use a switch Control Statement
  * Labs
3. while Loops
  * Looping
  * while Loops
  * while Loops - Details
  * Steps in a while Loop
  * Scope
  * do-while Loops
  * Infinite Loops
  * break and continue Statements
  * Labs
4. Project: Hi/Lo
5. Project: Remote Control Simulator

Day 4
1. Methods
  * Method Review
  * Methods Instead of Repeating Code
  * Returning Values from Methods
  * Using a Method's return value
  * Sending Data to Methods
  * Defining Parameters
  * Local Variables (Additional Drill)
  * Pass-by-value
  * Method Overloading
  * Labs
2. for Loops
  * for Loops
  * A for Loop Diagram
  * for Loop Parts
  * for Loop Body
  * break and continue Statements
  * For Loop - When and Why
  * Labs
3. Project: Fizz Buzz
4. Project: Fibonacci Series

Day 5
1. Numeral Systems
  * Counting and Tallying
  * Positional Notation
  * Numeral Systems for Programming
  * Numeric Literals in Java
  * The printf() Method 
2. Data Types in Java
  * Data Types You've Used
  * Memory and Java
  * Bits and Bytes
  * Counting in Binary
  * Most Significant Bit
  * Primitive Data Types
  * Primitives and Memory
  * Variable Types Tell Java What to Do
  * Declaring and Assigning Primitive Values
  * Floating Point Literals
  * long for Large Numbers
  * switch and Data Types
  * Labs
3. Casting Data Types
  * Implicit Type Conversions
  * Promotion of Data Types in Arithmetic
  * Promotion in Integer Arithmetic
  * The Cast Operator
  * Casting Hints
  * Labs
#### Homework Project: Make Change (Cash Register)

Day 6
1. Arrays
	* Variables - Single vs. Collections
	* Arrays are one of the primary data collections in Java.
	* An array allows us to have a single variable that points to multiple pieces of data.
	* Arrays
	* Declaring an Array
  	* Creating an Array
  	* Array Element Default Values
  	* Reading and Storing Data
  	* Array Initialization Shortcuts
  	* Iterating Arrays
  	* Passing Arrays to Methods
  	* Three Ways of Creating Arrays
  	* Labs
* Introduction to Objects
  * Classes
  * Creating Objects
  * Reference Variables 
  * State and Behavior
  * Field Initialization
  * The static Keyword
  * Some Objects You've Already Met
  * Labs
* Project: Deaf Grandma    

Day 7
* Advanced For Loops
  * Nested for Loops
  * Enhanced For Loops
  * Break and Continue With Enhanced For Loops
  * Labs
* Advanced Arrays
  * Array Syntax
  * Returning Array References from Methods
  * Arrays of Arrays
  * Accessing Elements of Multidimensional Arrays
  * Iterating Multidimensional Arrays
  * ForEach Loops for Iterating Arrays
  * Multidimensional Array Shortcuts
  * Variable Arguments Arrays
  * Labs
* Project: Tic Tac Toe

`Homework Project: Make Change (Cash Register`

-----
### [Week 2](https://github.com/SkillDistillery/SD41/blob/main/java1/README.md)

`Object-Oriented Programming in Java`

Day 1
* Packages
  * Namespaces
  * Introduction to Java Packages
  * Creating Packages
  * Package Names
  * Imports
  * Static Imports
  * Labs
* String and StringBuilder
  * The String Class
  * The String Pool
  * String Methods
  * The StringBuilder Class
  * StringBuilder Methods
  * Writing toString() Methods
  * Labs
* Project: Mad Libs

Day 2
* ASCII and Unicode Data
  * Standards
  * ASCII
  * Unicode
  * Labs
* Objects and Classes
  * Classes and Objects
  * Constructors
  * The Default Constructor
  * Objects in Memory
  * Imagining the Heap
  * Visibility
* Drawing Objects and Their Relationships
  * Representing Objects with Diagrams
  * UML Class Diagram
  * Classes and Their Associations
  * Labs
* Introduction to JUnit
  * Testing Java Applications
  * Building and Deploying Software
  * JUnit
  * Test Classes
  * Writing @Test Methods
  * assert Methods
  * @Before and @After
  * Test-Driven Development (TDD)
  * Labs
* Project: Caesar Cipher

Day 3
* Encapsulation
  * Changing Instance Fields
  * Visibility and Access Modifiers
  * Encapsulation
  * Getters and Setters
  * The this Keyword
  * Labs
* Object Initialization
  * this vs. this()
  * Initializing Static Fields
  * Initializing Instance Fields
  * Order of Initialization
  * Constant Fields and Variables
  * private Methods
  * Labs
* Inheritance in Java
  * Inheritance
  * The extends Keyword
  * final Classes 
  * UML and extends
  * Inheriting Fields 
  * Inheriting Methods 
  * Lab - Creating a Class Hierarchy
* Visibility
  * Field and Method Visibility
  * Getters and Setters
  * Lab - Improving Encapsulation
* Project: Food Trucks

Day 4
* Superclasses
  * Using a Superclass's Methods and Fields
  * Constructors and Inheritance
  * Rules for super()
  * The Object Class
  * Labs
* Polymorphism and Overriding
  * Polymorphism in Java
  * Overriding Superclass Behavior
  * @Override
  * Rules for Overriding
  * Lab - Using Polymorphism
* Abstract Classes
  * Abstract Classes
  * Abstract Methods
  * Using Abstract Classes
  * Labs
* Polymorphism and Casting
  * Casting
  * Downcasting
  * Casting and Precedence
  * Hiding Instance Fields
  * Labs
* Project: Animal Sanctuary

Day 5
* Equals and Hashcode
  * Comparing References
  * Object.equals()
  * Defining an equals() Method
  * Determining Equality
  * hashCode()
  * Labs
* The Primitive-Type Wrapper Classes
  * Wrapper Classes
  * Important Wrapper Class Methods
  * Comparing Wrapper Objects
  * Autoboxing
  * Float and Double
  * Integer-type Wrappers
  * Character
  * Boolean
  * Labs
* Interfaces
  * Interfaces
  * Declaring an Interface
  * Using Interfaces
  * Labs - Declaring and Using Interfaces
* Project: Lord of the Objects

`Homework Project: Lord of the Objects`

-----
### Week 3

`Object-Oriented Programming in Java`

`Java Libraries`

`Homework Project: Jets`

-----
### Week 4

`Java Libraries`

`Homework Project: Blackjack`

-----
### Week 5

`Java Libraries`

`OCP Exam Preparation`

-----
### Week 6

`OCP Exam Preparation`

-----
### Week 7

`OCP or Final Mock Exam`

`Web Basics`

`Introduction to SQL and JDBC`

`Homework Project: Film Query Application`

-----
### Week 8

`Dynamic Web Applications`

`Introduction to Spring MVC`

`SQL and JDBC Application Development`

`Group Project: Spring MVC Film C.R.U.D.`

-----
### Week 9

`Introduction to Spring MVC`

`JPA`

`SQL and JDBC Application Development`

`Homework Project: Spring MVC C.R.U.D.`

-----
### Week 10

`JPA`

`Full Stack Group MVC Project`

-----
### Week 11

`Full Stack Group MVC Project`

-----
### Week 12

`RESTful Services`

`Spring Data JPA`

`JavaScript`

-----
### Week 13

`JavaScript`

-----
### Week 14

`Angular`

-----
### Week 15

`Final Project`

-----
### Week 16

`Final Project`

`Final Review`

-----
### Resources
[Java Language Keywords](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/_keywords.html)

-----
### Project List
1. [Make Change] 
2. [Deaf Grandma]
3. [Food Truck]
4. 
5. 
6. 
7. 
8. 
9. 
10. 
