### [Week 1](https://github.com/SkillDistillery/SD41/blob/main/jfop/README.md)

#### Java Fundamentals of Programming

Day 1
1. Day One System Setup
2. Simple Programs
	1. Programming
```java
//simpleprograms/drills/Hello.java
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
4. Introduction to Methods
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
5. Screen Output and Keyboard Input
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
java.util.Scanner scanner = new java.util.Scanner(System.in);
scanner.close();
```
```java
String str = scanner.next();
int i = scanner.nextInt();
boolean b = scanner.nextBoolean();
double d = scanner.nextDouble();
```
```java
//screenoutputkeyboardinput/drills/ScannerInput.java
public class ScannerInput {

	public static void main(String[] args) {
		java.util.Scanner keyboard = new java.util.Scanner(System.in);

		int yearBorn;

		System.out.print("Please enter the year you were born: ");
		yearBorn = keyboard.nextInt();

		System.out.println("You were born in " + yearBorn + "! Crazy me too!");

		keyboard.close();
	}
}
```
```java
//screenoutputkeyboardinput/drills/ScannerInput.java
public class ScannerInput {

	public static void main(String[] args) {
		java.util.Scanner keyboard = new java.util.Scanner(System.in);

		int yearBorn;

		System.out.print("Please enter the year you were born: ");
		yearBorn = keyboard.nextInt();
		// yearBorn = hello world or "1992"

//		Exception in thread "main" java.util.InputMismatchException
//		  at java.util.Scanner.throwFor(Scanner.java:864)
//		  at java.util.Scanner.next(Scanner.java:1485)
//		  at java.util.Scanner.nextInt(Scanner.java:2117)
//		  at java.util.Scanner.nextInt(Scanner.java:2076)
//		  at ScannerInputSolution.main(ScannerInputSolution.java:12)

//		 This is because Java accepts all user input as a String and then 
//		 tries to convert it to the correct type.

		System.out.println("You were born in " + yearBorn + "! Crazy me too!");

		keyboard.close();
	}
}

```
*     
 	5. [Labs](https://github.com/SkillDistillery/SD41/blob/main/jfop/ScreenOutputKeyboardInput/labs.md)
```java
//Lab1 - FiveIntegers.java
public class FiveIntegers {

	public static void main(String[] args) {
		java.util.Scanner sc = new java.util.Scanner(System.in);

		int num1;
		int num2;
		int num3;
		int num4;
		int num5;

		System.out.print("Please enter a number: ");
		num1 = sc.nextInt();

		System.out.print("Please enter another number: ");
		num2 = sc.nextInt();

		System.out.print("Please enter another number: ");
		num3 = sc.nextInt();

		System.out.print("Please enter another number: ");
		num4 = sc.nextInt();

		System.out.print("Please enter another number: ");
		num5 = sc.nextInt();

		System.out.println(num1 + " " + num2 + " " + num3 + " " + num4 + " " + num5);
		System.out.println(num1 + "\t" + num2 + "\t" + num3 + "\t" + num4 + " \t" + num5);
		System.out.println(num1 + "\n" + num2 + "\n" + num3 + "\n" + num4 + "\n" + num5);

		scanner.close();
	}
}
```
```java
//Lab2 - ThreeVariables.java
public class ThreeVariables {

	public static void main(String[] args) {
		java.util.Scanner sc = new java.util.Scanner(System.in);

		System.out.println("Enter a Department Code: ");
		String departmentCode;
		departmentCode = sc.next();

		System.out.println("Enter a Salary: ");
		float salary;
		salary = sc.nextFloat();

		System.out.println("Enter an Employee Id: ");
		int employeeId;
		employeeId = sc.nextInt();

		System.out.println(departmentCode + " " + salary + " " + employeeId);
		System.out.println(departmentCode + "\t" + salary + "\t" + employeeId);
		System.out.println(departmentCode + "\n" + salary + "\n" + employeeId);

		scanner.close();
	}
}

```
6. Eclipse
```java
//To see a list of all of the shortcut keys, use Cmd-Shift-L.
```
Day 2
1. Eclipse
2. Expressions
	1. Expressions: Where the Work Gets Done
 	2. Expression Evaluation: The Result
 	3. Assignment Expressions
```java
//Expressions/src/drills/Assignment.java
public class Assignment {

	public static void main(String[] args) {
		intAssignment();
		booleanAssignment();
	}

	static void intAssignment() {
		int myAge = 12;
		System.out.println("myAge is " + myAge);
		System.out.println(myAge = 99);
		System.out.println("myAge is now " + myAge);
	}

	static void booleanAssignment() {
		boolean value = false;
		System.out.println("value is " + value);
		System.out.println(value = true);
		System.out.println("value is now " + value);
	}
}
```
```java
System.out.println(Math.abs(variableName)); //.abs allows for -/+ numbers to be +
System.out.println(Math.abs(methodName()));
```
*
   	4. Arithmetic Expressions
```java
//Expressions/src/drills/Arithmetic.java
public class Arithmetic {

	public static void main(String[] args) {
		// Run this program with several numbers. What happens to the remainder when you do
		// integer division?
			doDivision();
		
		// Comment out the call to doDivision();
		// Uncomment the call to doModulus();
		 	//doModulus();
	}
	
	static void doDivision() {
		Scanner sc = new Scanner(System.in);
		System.out.println("Refresher:\n\tDivision:\tquotient = dividend / divisor");
		System.out.print("Enter the dividend: ");
		int dividend = sc.nextInt();
		System.out.print("Enter the divisor: ");
		int divisor = sc.nextInt();
		int quotient = dividend / divisor;
		System.out.println("quotient = " + quotient);
		sc.close();
	}
	
	static void doModulus() {
		Scanner sc = new Scanner(System.in);
		
		System.out.println("Refresher:\n\tDivision:\tquotient = dividend / divisor");
		System.out.println("\tRemainder: amount left over from division");

		// Complete the method and use the modulus operator to find the remainder.		
		System.out.print("Enter the dividend: ");
		int dividend = sc.nextInt();
		System.out.print("Enter the divisor: ");
		int divisor = sc.nextInt();
		int remainder = dividend % divisor;
		System.out.println("remainder = " + remainder);
		sc.close();
	}
}
```
```java
//Expressions/src/drills/MilesPerGallon.java
public class MilesPerGallon {
	public static void main(String[] args) {
		java.util.Scanner scanner = new java.util.Scanner(System.in);
		
		double milesTraveled = 0.0;
		double gallonsUsed = 0.0;
		double milesPerGallon = 0.0;
		
		System.out.print("Please enter the number of miles" + " traveled: ");
		//TODO: get the miles traveled
		milesTraveled = scanner.nextDouble();
		
		System.out.print("Please enter the number of gallons" + " used: ");
		//TODO: get the gallons used
		gallonsUsed = scanner.nextDouble();
		
		//TODO: calculate miles per gallon
		milesPerGallon = milesTraveled / gallonsUsed;
		
		System.out.print("You traveled " + milesPerGallon);
		System.out.println(" miles for every gallon of fuel" + " used.");
		scanner.close();
	}
}
```
*	
  	5. Relational Expressions
```java
//Expressions/src/drills/Relational.java
public class Relational {

	public static void main(String[] args) {
		Scanner keyboard = new Scanner(System.in);
		System.out.print("Enter the first number: ");
		int first = keyboard.nextInt();
		System.out.print("Enter the second number: ");
		int second = keyboard.nextInt();

		boolean result = first >= second;
		System.out.println("Is first greater than or equal to second? " + result);

		// Add additional tests with the other logical operators.
		// boolean result = first <= second;
		// boolean result = first == second;
		// boolean result = first != second;

		keyboard.close();
	}
}
```
*
 	6. Logical Expressions
```java
//Expressions/src/drills/Logical.java
public class Logical {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);

		int min, max, salary;

		System.out.println("Let's see if the salary you've been offered is what you expected.");

		System.out.print("Enter your minimum salary requirement: ");
		min = sc.nextInt();

		System.out.print("Enter the maximum you would ask for: ");
		max = sc.nextInt();

		System.out.print("Enter the salary offered: ");
		salary = sc.nextInt();

		boolean isExpectedSalary = false;

		// Add code to check if the salary is in the range of min and max and assign
		// that value to isExpectedSalary
		isExpectedSalary = ((salary >= min) && (salary <= max));
		System.out.println("Is this salary what you expect for the position? " + isExpectedSalary);

		// Add code to check and output whether the salary is "dreamy," where dreamy
		// means it is more than $10,000 greater than your max.
		boolean isDreamy = (salary) > (10000 + max);
		System.out.println("Is the salary more than $10000 over your max? " + isDreamy);

		// Add code to check and output whether the salary is "laughable," where
		// laughable means it is at least $5,000 less than your minimum salary
		// requirement.
		boolean isLaughable = (salary) <= (min - 5000);
		System.out.println("Is the salary laughable? " + isLaughable);

		sc.close();
	}
}
```
* 	
  	7. Short-Circuit Operators
 	8. Associativity
 	9. Precedence
```java
//Expressions/src/drills/Precedence.java
public class Precedence {

	public static void main(String[] args) {
		// The methods in this program have bugs. Uncomment methods one at a time to see
		// output.
		// Change the statements in each method to produce the expected result.
		// You can only use parentheses.

		// result1Method();
		// result2Method();
		// result3Method();
	}

	// Group expressions with parentheses to get the expected result.
	static void result1Method() {
		int result = (2 + 1) * 4;
		// Expected: 12
		System.out.println(result);
	}

	static void result2Method() {
		int a = 2, b = 1, c = 3;
		int result = a * (c + 3) % 2;
		// Expected: 0
		System.out.println(result);
	}

	static void result3Method() {
		int a = 2, b = 1, c = 3;
		boolean result = c % a == 0 && (c > 2 || b > 0);
		// Expected: false
		System.out.println(result);
	}
}
```
*
  	10. Precedence Order
 	11. [Labs](https://github.com/SkillDistillery/SD41/blob/main/jfop/Expressions/labs.md)
```java
//Lab1 - Circle1.java
public class Circle1 {

	public static void main(String[] args) {
		java.util.Scanner scanner = new java.util.Scanner(System.in);

		double radius;
		double circumference;

		System.out.print("Enter a radius: ");
		radius = scanner.nextFloat();

		circumference = 2 * 3.141592653589793 * radius;

		System.out.println("Radius: " + radius);
		System.out.println("Circumference: " + circumference);

		scanner.close();
	}
}
```
```java
//Lab2 - Circle2.java
public class Circle2 {

	public static void main(String[] args) {
		java.util.Scanner scanner = new java.util.Scanner(System.in);

		double radius;
		double circumference;
		double area;

		System.out.print("Enter a radius: ");
		radius = scanner.nextFloat();

		circumference = 2 * 3.141592653589793 * radius;
		area = (radius * radius) * 3.141592653589793;

		System.out.println("Radius: " + radius);
		System.out.println("Circumference: " + circumference);
		System.out.println("Area: " + area);

		scanner.close();
	}
}
```
```java
//Lab3 - FahrToCels.java
public class FahrToCels {

	public static void main(String[] args) {
		java.util.Scanner scanner = new java.util.Scanner(System.in);

		double fahrenheit;
		double celsius;

		System.out.print("Enter Degree Fahrenheit: ");
		fahrenheit = scanner.nextDouble();

		celsius = 5.0 / 9.0 * (fahrenheit - 32);

		System.out.println("Celsius: " + celsius);

		scanner.close();
	}
}
```
```java
//Lab4 - CalculateTip.java
public class CalculateTip {

	public static void main(String[] args) {
		java.util.Scanner scanner = new java.util.Scanner(System.in);

		double check;

		System.out.print("Enter Check Amount: ");
		check = scanner.nextDouble();

		double check10 = check * .1;
		double check15 = check * .15;
		double check20 = check * .20;

		System.out.println("10% Tip " + check10 + " -- Total: $" + (check10 + check));
		System.out.println("15% Tip " + check15 + " -- Total: $" + (check15 + check));
		System.out.println("20% Tip " + check20 + " -- Total: $" + (check20 + check));

		scanner.close();
	}
}
```
```java
//Lab5 - DailyRainfall.java
public class DailyRainfall {

	public static void main(String[] args) {
		java.util.Scanner scanner = new java.util.Scanner(System.in);

		System.out.println("Enter the rainfall level for Sunday: ");
		double sunday = scanner.nextDouble();

		System.out.println("Enter the rainfall level for Monday: ");
		double monday = scanner.nextDouble();

		System.out.println("Enter the rainfall level for Tuesday: ");
		double tuesday = scanner.nextDouble();

		System.out.println("Enter the rainfall level for Wednesday: ");
		double wednesday = scanner.nextDouble();

		System.out.println("Enter the rainfall level for Thursday: ");
		double thursday = scanner.nextDouble();

		System.out.println("Enter the rainfall level for Friday: ");
		double friday = scanner.nextDouble();

		System.out.println("Enter the rainfall level for Saturday: ");
		double saturday = scanner.nextDouble();

		// Calculate the total rainfall and the average rainfall for the week
		double total = sunday + monday + tuesday + wednesday + thursday + friday + saturday;
		double average = total / 7;

		// Print the results of the processing
		System.out.println("Total rainfall for the Week: " + total);
		System.out.println("Average rainfall for the Week: " + average);

		scanner.close();
	}
}
```
3. Conditionals: if and else
	1. Sequential Execution
 	2. if Statement
 	3. if Syntax
 	4. Code Blocks
```java
//IfElse/src/drills/SalaryDecisions.java
public class SalaryDecisions {
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);

		int min, max, salary;

		System.out.println("Let's see if the salary you've been offered is acceptable.");

		System.out.print("Enter your minimum salary requirement: ");
		min = sc.nextInt();

		System.out.print("Enter the maximum you would ask for: ");
		max = sc.nextInt();

		System.out.print("Enter the salary offered: ");
		salary = sc.nextInt();

//			System.out.println("Is this salary acceptable? " + isAcceptableSal);
		boolean isAcceptableSal = false;
		// TODO: Change the code to print "The salary is acceptable." if isAcceptableSal
		// is true. Use a code block for the if statement.
		// Comment out the old System.out.println statement
		isAcceptableSal = salary >= min && salary <= max;
		if (isAcceptableSal == true) {
			System.out.println("The salary acceptable! ");
		}

		// TODO: Change the code to print "The salary is more than $10000 over max" if
		// the condition is true.
		// Do not use the condition "isDreamy == true". You can just use the variable
		// itself because it is a boolean.
		// Comment out the old System.out.println statement
//			System.out.println("Is the salary more than $10000 over your max? " + isDreamy);
		boolean isDreamy = salary > 10000 + max;
		if (isDreamy) {
			System.out.println("The salary is more than $10000 over max");
		}

		// TODO: Change the code to print "The salary is $5000 or more below min" if the
		// condition is true.
		// Do not use the isLaughable variable. Just use the condition itself inside
		// your if statement.
		// Comment out the old System.out.println statement and the isLaughable
		// variable.
//			System.out.println("Is the salary laughable? " + isLaughable);
		boolean isLaughable = salary <= min - 5000;
		if (salary <= min - 5000) {
			System.out.println("The salary is $5000 or more below min");
		}
		sc.close();
	}
}
```
*
   	5. if and else if
```java
//IfElse/src/drills/SalaryDecisions2.java
public class SalaryDecisions2 {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);

		int min, max, salary;

		System.out.println("Let's see if the salary you've been offered is acceptable.");

		System.out.print("Enter your minimum salary requirement: ");
		min = sc.nextInt();

		System.out.print("Enter the maximum you would ask for: ");
		max = sc.nextInt();

		System.out.print("Enter the salary offered: ");
		salary = sc.nextInt();

		boolean isAcceptableSal = false;
		boolean isDreamy = salary > 10000 + max;

		// TODO: Change this code to use "else if" statements for the other conditions
		isAcceptableSal = salary >= min && salary <= max;

		if (isAcceptableSal == true) {
			System.out.println("The salary is acceptable.");
		} else if (isDreamy) {
			System.out.println("The salary is more than $10000 over max");
		} else if (salary <= min - 5000) {
			System.out.println("This salary is a joke.");
		}
		sc.close();
	}
}
```
* 	
  	6. if and else
```java
//IfElse/src/drills/SalaryDecisions3.java
public class SalaryDecisions3 {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);

		int min, max, salary;

		System.out.println("Let's see if the salary you've been offered is acceptable.");

		System.out.print("Enter your minimum salary requirement: ");
		min = sc.nextInt();

		System.out.print("Enter the maximum you would ask for: ");
		max = sc.nextInt();

		System.out.print("Enter the salary offered: ");
		salary = sc.nextInt();

		// TODO: add an else statement to print the message "At least I got an offer."
		// What salary range causes the else block to execute? Add it as a comment in
		// your else block.
		// salary < min && salary > (min - 5000)
		// salary > max && salary < (max + 10000)
		boolean isAcceptableSal = false;
		isAcceptableSal = (salary >= min) && (salary <= max);
		if (isAcceptableSal == true) {
			System.out.println("The salary is acceptable.");
		} else if (salary > (10000 + max)) {
			System.out.println("The salary is more than $10000 over max");
		} else if (salary <= (min - 5000)) {
			System.out.println("This salary is a joke.");
		} else {
			System.out.println("At least I got an offer.");
		}
		sc.close();
	}
}
```
*
  	7. Nested Control Statements
 	8. Comparing Strings in Java
```java
//IfElse/src/drills/StringComparison.java
public class StringComparison {

	public static void main(String[] args) {
		compareNames();
	}

	public static void compareNames() {
		Scanner sc = new Scanner(System.in);

		System.out.println("Short, hungry, hairy - you're my kind of lad.");
		System.out.println("What is your name?");
		String name = sc.next();

		// Run the program with a proper name.
		// Fix the code to no longer use `==`.
		if (name.equals("Frodo")) {
			System.out.println("And brave, too!");
		} else if (name.equals("Sam")) {
			System.out.println("And so loyal!");
		} else if (name.equals("Merry")) {
			System.out.println("Oh, a hungry one!");
		} else if (name.equals("Pippin")) {
			System.out.println("A sidekick, huh? At least you know rings.");
		} else {
			System.out.println("Hmmm. Doesn't ring a bell.");
		}
		sc.close();
	}
}
```
*	
  	9. [Labs](https://github.com/SkillDistillery/SD41/blob/main/jfop/IfElse/labs.md)
```java
//Lab 1 - NumSign.java
public class NumSign {

	public static void main(String[] args) {
		// Write a program that accepts a number as input and prints a message stating
		// whether the number is positive or negative.

		Scanner sc = new Scanner(System.in);

		System.out.print("Give me a number: ");
		int number = sc.nextInt();
		sc.nextLine();

		if (number > 0) {
			System.out.println("This number is positive");
		} else {
			System.out.println("This number is negative");
		}
		sc.close();
	}
}
```
```java
//Lab 2 - NumSignZero.java
public class NumSignZero {

	public static void main(String[] args) {
		// Write a program that accepts a number as input and prints a message stating
		// whether the number is positive or negative.

		Scanner sc = new Scanner(System.in);

		System.out.print("Give me a number: ");
		int number = sc.nextInt();
		sc.nextLine();

		if (number > 0) {
			System.out.println("This number is positive");
		} else if (number == 0) {
			System.out.println("This number is 0");
		} else {
			System.out.println("This number is negative");
		}
		sc.close();
	}
}
```
```java
//Lab 3 - NumFactors.java
public class NumFactors {

	public static void main(String[] args) {
		// Write a program that accepts a number as input and prints a message stating
		// whether the number is positive or negative.

		Scanner sc = new Scanner(System.in);

		System.out.print("Give me a number: ");
		int number = sc.nextInt();
		sc.nextLine();

		if (number % 2 == 0) {
			System.out.println("This number is even!");
			if (number % 100 == 0) {
				System.out.println("...And divisible by 100!");
			} else if (number % 10 == 0) {
				System.out.println("...And divisible by 10!");
			} else {
			}
		} else {
			System.out.println("This number is odd!");
		}
		sc.close();
	}
}
```
```java
//Lab 4 - IfCelsFahr.java
public class IfCelsFahr {
	public static void main(String[] args) {
		java.util.Scanner scanner = new java.util.Scanner(System.in);

		double fahrenheit = 0.0;
		double celsius = 0.0;
		double inputNum = 0.0;
		String scale = "";

		System.out.print("Please Enter your Temperature: ");
		inputNum = scanner.nextDouble();
		scanner.nextLine();

		System.out.print("Please Enter the Scale: ");
		scale = scanner.nextLine();
		scanner.close();

		if (scale.equals("F") || scale.equals("f") || scale.equals("Fahrenheit") || scale.equals("fahrenheit")) {
			fahrenheit = inputNum;
			celsius = 5.0 / 9.0 * (fahrenheit - 32);
			System.out.print(fahrenheit + " degrees Fahrenheit is ");
			System.out.println(celsius + " degrees Celsius.");
		} else if (scale.equals("C") || scale.equals("c") || scale.equals("Celsius") || scale.equals("celsius")) {
			celsius = inputNum;
			fahrenheit = (9.0 / 5.0 * celsius) + 32;
			System.out.print(celsius + " degrees Celsius is ");
			System.out.println(fahrenheit + " degrees Fahrenheit.");
		} else {
			System.err.println("Invalid Scale.");
		}
	}
}
```
4. Pair Programming
5. Project: Simple Calculator
6. Project: Mad Libs (6.)

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

[Operator Precedence in Java](https://introcs.cs.princeton.edu/java/11precedence/)

-----
### Project List
1. [Make Change]() 
2. [Deaf Grandma]()
3. [Food Truck]()
4. 
5. 
6. 
7. 
8. 
9. 
10. 
