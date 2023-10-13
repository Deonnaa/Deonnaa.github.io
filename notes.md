### [Week 1](https://github.com/SkillDistillery/SD41/blob/main/jfop/README.md)

`Java Fundamentals of Programming`

Day 1
* Day One System Setup
* Simple Programs
* Variables and Constants
* Introduction to Methods
* Screen Output and Keyboard Input
* Eclipse

Day 2
* Eclipse
* Expressions
  * Expressions: Where the Work Gets Done
     ``` java
     age = 29          //Assignment Expression
     5 + 3             //Arithmetic expressions 
     i < 10            //Relational expressions
     i < 10 && j > 5   //Logical expressions
     ``` 
  * Expression Evaluation: The Result
     ``` java
     Evaluating 3 + 5 results in 8.
     Evaluating 3 < 5 results in true.
     Evaluating 3 < 5 and 10 < 7 results in false.
     ```  
  * Assignment Expressions
     ``` java
     int myAge;
     myAge = 12;
     int yourAge = myAge = 9; //x and y both have value 9
     ```
    ``` java
    int myAge = 12;
    System.out.println("myAge is " + myAge);
    System.out.println(myAge = 99);
    System.out.println("myAge is now " + myAge);
     ```
     ``` java
     boolean value = false;
     System.out.println("value is " + value);
     System.out.println(value = true);
     System.out.println("value is now " + value);
     ```
  * Arithmetic Expressions
     ``` java
     length + 6.13     //Add Subtract
     5 - radius
     
     width * height    //Multiply Divide
     total / 2
     
     15 % 4            //Modulus
     year % 100
     ```     
  * Relational Expressions
     ```java
     hoursWorked < 40       // <,>,= operators
     age <= 12
     
     income > 55000         
     numPlayers >= 3
     
     menuItem == choice     //equal to(==), not equal to (!=)
     choice != 'q'
     ```      
  * Logical Expressions
    <table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Operator</th>
      <th>Example</th>
      <th>Evaluates to <code>true</code> when...</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>AND</td>
      <td><code>&&</code></td>
      <td><code>a && b</code></td>
      <td><strong>both</strong> a and b are true</td>
    </tr>
    <tr>
      <td>OR</td>
      <td><code>||</code></td>
      <td><code>a || b</code></td>
      <td><strong>either</strong> a or b is true</td>
    </tr>
    <tr>
      <td>AND<sup>1</sup></td>
      <td><code>&</code></td>
      <td><code>a & b</code></td>
      <td><strong>both</strong> a and b are true</td>
    </tr>
    <tr>
      <td>OR<sup>1</sup></td>
      <td><code>|</code></td>
      <td><code>a | b</code></td>
      <td><strong>either</strong> a or b is true</td>
    </tr>
  </tbody>
</table>


 * Short-Circuit Operators
 * Associativity
  	* Java reads statements left to right. When it sees operators, it looks for data to use with the operators. Associativity determines in which order a given operator looks for its operands.
  * Precedence
  * ```java
    int b = 5;
    int c = 2;
    a = b * (c + 10); // * looks right for a right-hand operand.
                      // parentheses cause c + 10 to execute first
    ```
  * Precedence Order
  	* Notice that assignment, =, has the lowest precedence of all. This is so that all calculations in a statement complete before the result is assigned to a variable. 
   	* ```java
      b < 42 || c > 50 && c < 100
      ( b < 42 ) || ( c > 50 && c < 100 )
      ``` 
  * Labs
* Conditionals: if and else
  * Sequential Execution
  * if Statement
  * if Syntax
  * Code Blocks
  * if and else if
  * if and else
  * Nested Control Statements
  * Comparing Strings in Java
  * Labs 
* Pair Programming
  * Driver
    * Codes only what directed by Navigator.
    * Stop and get clarification as needed.
    * To offer input, hands off keyboard until consensus is reached.
    * Constant narration: code out loud (Navigator too).
  * Navigator
    * Is responsible for communicating directions.
    * Close your laptop.
    * Never touches a keyboard, either Driver’s or their own.
    * Driver Googles when it’s Google time.
  * Four C's
    * Check your ego at the door.
    * Compromise.
    * Communicate.
    * Collaborate.  
* Project: Simple Calculator
* Project: Mad Libs

Day 3
* More Expressions
  * Using Boolean Variables
  * Boolean Expressions
  * Assignment Operators
  * Auto-increment
  * The Ternary Conditional Operator
  * Labs
* Conditionals: switch
  * switch Statements: Multi-Way Decisions
  	* Of the data types we know, we can use int, char, and String data types in switch statements.

   	* ```java
      char grade = 'A';
      String message;

      switch (grade) {
      case 'A':
      message = "Keep it up";
      break;
      case 'B':
      message = "Good job";
      break;
      case 'C':
      message = "Doing alright";
      break;
      case 'D':
      message = "Let's talk";
      break;
      case 'F':
      message = "You should come to class";
      break;
      default:
      message = "That's not a grade";
      }
      ```
     
   	* 1234
  * break; and default: in switch Statements
  	* 123
  * When to Use a switch Control Statement
  	* 123
  * Labs
* while Loops
  * Looping
  * while Loops
  * while Loops - Details
  * Steps in a while Loop
  * Scope
  * do-while Loops
  * Infinite Loops
  * break and continue Statements
  * Labs
* Project: Hi/Lo
* Project: Remote Control Simulator

Day 4
* Methods
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
* for Loops
  * for Loops
  * A for Loop Diagram
  * for Loop Parts
  * for Loop Body
  * break and continue Statements
  * For Loop - When and Why
  * Labs
* Project: Fizz Buzz
* Project: Fibonacci Series

Day 5
* Numeral Systems
  * Counting and Tallying
  * Positional Notation
  * Numeral Systems for Programming
  * Numeric Literals in Java
  * The printf() Method 
* Data Types in Java
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
* Casting Data Types
  * Implicit Type Conversions
  * Promotion of Data Types in Arithmetic
  * Promotion in Integer Arithmetic
  * The Cast Operator
  * Casting Hints
  * Labs
* Homework Project: Make Change (Cash Register)

Day 6
* Arrays
  * Variables - Single vs. Collections
  	* Data collections are, as the name implies, collections of multiple pieces of data.
   * Arrays are one of the primary data collections in Java.
   * An array allows us to have a single variable that points to multiple pieces of data. 
  * Arrays
  * Declaring an Array
```java

```  
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
```java
Car myCar; //Doesnt grab any memory to store on heap yet
myCar = new Car(); //2 Lines new gives address on heap

Car myCar = new Car(); //1 line
```

```java
Car anotherCar = new Car();

Car aCar = myCar; //same location in memory 
```
  * Reference Variables
```java
//SphereReferences.java
Sphere sphRef = new Sphere();
sphRef.radius = 10;
System.out.print("Original sphRef radius: " + sph.radius); //10.0

Sphere otherSphereRef = sphRef;
System.out.print("otherSphereRef radius: " + otherSphereRef.radius); //10.0
otherSphereRef.radius = 20; //changes address in heap for both

System.out.print("Original sphRef radius: " + sph.radius); //20.0
System.out.print("otherSphereRef radius: " + otherSphereRef.radius); //20.0

//Sphere.java
public class Sphere(){
	public double radius;

	public double getVolume(){
	double vol = 4.0 / 3.0 * 3.14 * radius * radius * radius
	return vol;
	}
}

```    
  * State and Behavior
  * Field Initialization
  * The static Keyword
  * Some Objects You've Already Met
  * Labs
* Project: Deaf Grandma
```java
//Grandma.java
public class Grandma(){
public String [] heardYa = {"HEARD YOU", "HI"};
public String [] heardYa = {"HEARD YOU", "HI"};
public String [] heardYa = {"HEARD YOU", "HI"};

	


}


```    

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
* 123
 * 123 

`Final Project`

`Final Review`
* ``` java
     123
     ```
   * ``` java
     123
     ```     
   * ``` java
     123
     ```     
   * ``` java
     123
     ```
  * ``` java
    123
     ```  
