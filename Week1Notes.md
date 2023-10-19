## [Week 1](https://github.com/SkillDistillery/SD41/blob/main/jfop/README.md)

## Week 1 - Day 1

#### Day One System Setup

#### Simple Programs
1. Programming
2. The Programming Process
3. Programming Languages
4. Compiler Errors and Runtime Errors
5. Input - Process - Output
6. Labs

`simpleprograms/drills/Hello.java`
```java
public class Hello {

	public static void main(String[] args) {
		System.out.println("Hello, SD41!");
	}
}
```

`Lab 1 - HelloName.java`
```java
public class HelloName {

	public static void main(String[] args) {
		System.out.println("Hello, Deonna!");
	}
}
```

`Lab 2 - TwoPrints.java`
```java
public class TwoPrints {

	public static void main(String[] args) {

		System.out.println("Hello,");
		System.out.println("Deonna!");
	}
}
```

`Lab 3 - HelloTabs.java`
```java
public class HelloTabs {

	public static void main(String[] args) {

		System.out.println("Hello,");
		System.out.println("\t\tDeonna!");
	}
}
```

`Lab 4 - HelloStars.java`
```java
public class HelloStars {

	public static void main(String[] args) {

		System.out.println("****************");
		System.out.println("*     Hello,   *");
		System.out.println("*    Deonna!   *");
		System.out.println("****************");
	}
}
```

`Lab 5 - Testing123.java`
```java
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

#### Variables and Constants
1. Data Types
2. Variables
3. Variable Naming Rules
4. Literals
5. Assignment
6. Printing Variables
7. Labs

`variablesandconstants/drills/VariableNaming.java`
```java
public class VariableNaming {

	public static void main(String[] args) {
		int distanceTraveled;
		int radius;
		String fullName;
	}
}
```

`variablesandconstants/drills/Assign.java`
```java
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

`variablesandconstants/drills/PrintingExample.java`
```java
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

`variablesandconstants/drills/VariablePrinting.java`
```java
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

`Lab 1 - AgeInitial.java`
```java
public class AgeInitial {

	public static void main(String[] args) {
		int age = 31;
		char mi;
		mi = 'H';

		System.out.println("James " + mi + " Bond" + ": Age: " + age);
	}
}
```

`Lab 2 - StudentScores.java`
```java
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

#### Introduction to Methods
1. Methods
2. Calling Methods
3. The main Method
4. Why Use Methods?
5. Labs

`introtomethods/drills/CallingMethods.java`
```java
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

`Lab 1 - MyName.java`
```java
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

#### Screen Output and Keyboard Input
1. Screen Output
2. Formatting Output
3. String Output
4. Reading from the Keyboard
5. Labs

`screenoutputkeyboardinput/drills/Formatting.java`
```java
public class Formatting {

	public static void main(String[] args) {
		System.out.println("\\\\ His name was \"Robert Paulson.\" \nYou cry now. //");
	}
}
```

`screenoutputkeyboardinput/drills/StringOutput.java`
```java
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

`screenoutputkeyboardinput/drills/ScannerInput.java`
```java
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

`screenoutputkeyboardinput/drills/ScannerInput.java`
```java
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

`Lab 1 - FiveIntegers.java`
```java
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

`Lab 2 - ThreeVariables.java`
```java
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

#### Eclipse

### Week 1 - Day 2

#### Eclipse

#### Expressions
1. Expressions: Where the Work Gets Done
2. Expression Evaluation: The Result
3. Assignment Expressions
4. Arithmetic Expressions
5. Relational Expressions
6. Logical Expressions
7. Short-Circuit Operators
8. Associativity *
9. Precedence *
10. Precedence Order
11. Labs

`Expressions/src/drills/Assignment.java`
```java
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

`Expressions/src/drills/Arithmetic.java`
```java
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

`Expressions/src/drills/MilesPerGallon.java`
```java
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

`Expressions/src/drills/Relational.java`
```java
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

`Expressions/src/drills/Logical.java`
```java
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

`Expressions/src/drills/Precedence.java`
```java
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

`Lab 1 - Circle1.java`
```java
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

`Lab 2 - Circle2.java`
```java
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

`Lab 3 - FahrToCels.java`
```java
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

`Lab 4 - CalculateTip.java`
```java
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

`Lab 5 - DailyRainfall.java`
```java
public class DailyRainfall {

	public static void main(String[] args) {
		java.util.Scanner scanner = new java.util.Scanner(System.in);

		System.out.println("Enter the rainfall level for SunWeek 1 - Day: ");
		double sunWeek 1 - Day = scanner.nextDouble();

		System.out.println("Enter the rainfall level for MonWeek 1 - Day: ");
		double monWeek 1 - Day = scanner.nextDouble();

		System.out.println("Enter the rainfall level for TuesWeek 1 - Day: ");
		double tuesWeek 1 - Day = scanner.nextDouble();

		System.out.println("Enter the rainfall level for WednesWeek 1 - Day: ");
		double wednesWeek 1 - Day = scanner.nextDouble();

		System.out.println("Enter the rainfall level for ThursWeek 1 - Day: ");
		double thursWeek 1 - Day = scanner.nextDouble();

		System.out.println("Enter the rainfall level for FriWeek 1 - Day: ");
		double friWeek 1 - Day = scanner.nextDouble();

		System.out.println("Enter the rainfall level for SaturWeek 1 - Day: ");
		double saturWeek 1 - Day = scanner.nextDouble();

		// Calculate the total rainfall and the average rainfall for the week
		double total = sunWeek 1 - Day + monWeek 1 - Day + tuesWeek 1 - Day + wednesWeek 1 - Day + thursWeek 1 - Day + friWeek 1 - Day + saturWeek 1 - Day;
		double average = total / 7;

		// Print the results of the processing
		System.out.println("Total rainfall for the Week: " + total);
		System.out.println("Average rainfall for the Week: " + average);

		scanner.close();
	}
}
```

#### Conditionals: if and else
1. Sequential Execution
2. if Statement
3. if Syntax
4. Code Blocks
5. if and else if
6. if and else
7. Nested Control Statements *
8. Comparing Strings in Java
9. Labs

`IfElse/src/drills/SalaryDecisions.java`
```java
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

`IfElse/src/drills/SalaryDecisions2.java`
```java
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

`IfElse/src/drills/SalaryDecisions3.java`
```java
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

`IfElse/src/drills/StringComparison.java`
```java
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

`Lab 1 - NumSign.java`
```java
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

`Lab 2 - NumSignZero.java`
```java
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

`Lab 3 - NumFactors.java`
```java
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

`Lab 4 - IfCelsFahr.java`
```java
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

#### Pair Programming

#### Project: Simple Calculator

#### Project: Mad Libs

### Week 1 - Day 3

#### More Expressions
1. Using Boolean Variables
2. Boolean Expressions
3. Assignment Operators
4. Auto-increment
5. The Ternary Conditional Operator
6. Labs

`AdvancedExpressions/src/drills/PrePostIncrement.java`
```java
public class PrePostIncrement {

	public static void main(String[] args) {
		int count = 0;

		while ((count = count + 1) < 10) {
			System.out.println(count);
		}

//    while ( ( count += 1 ) < 10 ) {
//        System.out.println(count);
//      }

//    while ( ( ++count ) < 10 ) {
//    	System.out.println(count);
//    }

//    while ( ( count++ ) < 10 ) {
//        System.out.println(count);
//      }
	}

}
```

`Lab 1 - OddOrEven.java`
```java
public class OddOrEven {

	public static void main(String[] args) {
		java.util.Scanner scanner = new java.util.Scanner(System.in);

		System.out.print("Please enter a number: ");
		int userNumber = scanner.nextInt();

		if (userNumber % 2 == 0) {
			System.out.println("This number is even.");
		} else {
			System.out.println("This number is odd.");
		}
		scanner.close();
	}
}
```

`Lab 2 - Multiply.java`
```java
public class Multiply {

	public static void main(String[] args) {
		java.util.Scanner scanner = new java.util.Scanner(System.in);

		System.out.print("Please enter a number: ");
		int userNumber1 = scanner.nextInt();

		System.out.print("Please enter a number: ");
		int userNumber2 = scanner.nextInt();

		System.out.print("Please enter a number: ");
		int userNumber3 = scanner.nextInt();

		System.out.print("Please enter a number: ");
		int userNumber4 = scanner.nextInt();

		System.out.print("Please enter a number: ");
		int userNumber5 = scanner.nextInt();

		System.out.println(userNumber1);
		System.out.println(userNumber1 *= userNumber2);
		System.out.println(userNumber1 *= userNumber3);
		System.out.println(userNumber1 *= userNumber4);
		System.out.println(userNumber1 *= userNumber5);

		scanner.close();
	}
}
```

`Lab 3 - PosNegZero.java`
```java
public class PosNegZero {

	public static void main(String[] args) {

		int userNumber = getNumber();

		String result = userNumber > 0 ? "Positive" : userNumber < 0 ? "Negative" : "Zero";
		System.out.println(result);
	}

	public static int getNumber() {
		Scanner scan = new Scanner(System.in);
		System.out.println("Enter a Number: ");
		int input = scan.nextInt();
		scan.close();
		return input;
	}
}
```

#### Conditionals: switch
1. switch Statements: Multi-Way Decisions
2. break; and default: in switch Statements
3. When to Use a switch Control Statement
4. Labs

`Switch/src/drills/SwitchInvestigation.java`
```java
public class SwitchInvestigation {

	public static void main(String[] args) {
		System.out.println("We are going to investigate what break; " + "and default: do in a switch statement");
		investigate();
	}

	public static void investigate() {
		java.util.Scanner sc = new java.util.Scanner(System.in);
		System.out.print("Enter a grade: ");
		String grade = sc.next();

		// 1. Comment out the break; statements for case "A" and "B".
		// Run the program. What output do you notice?
		// 2. Move the entire default case before case "A":
		// Run the program. What output do you notice?
		switch (grade) {
		case "A":
			System.out.println("Keep it up");
			break;
		case "B":
			System.out.println("Good job");
			break;
		case "C":
			System.out.println("Doing alright");
			break;
		case "D":
			System.out.println("Let's talk");
			break;
		case "F":
			System.out.println("You should come to class");
			break;
		default:
			System.out.println("That's not a grade");
		}
		sc.close();
	}
}
```

`Switch/src/drills/SwitchFallthrough.java`
```java
public class SwitchFallthrough {

	public static void main(String[] args) {
		System.out.println("We can now handle uppercase and lowercase grades, thanks to fall through.");
		investigate();

	}

	public static void investigate() {
		java.util.Scanner sc = new java.util.Scanner(System.in);
		System.out.print("Enter a grade: ");
		String grade = sc.next();
		
		// "A" falls through to "a" so they both print the same message
		switch (grade) {
		case "A": 
		case "a":
			System.out.println("Keep it up");
			break;
		case "B":
		case "b":
			System.out.println("Good job");
			break;
		case "C": case "c":
			System.out.println("Doing alright");
			break;
		case "D":
		case "d":
			System.out.println("Let's talk");
			break;
		case "F":
		case "f":
			System.out.println("You should come to class");
			break;
		default:
			System.out.println("That's not a grade");
		}
		sc.close();
	}
}
```

`Lab 1 - IfCelsFahrSwitch.java`
```java
public class IfCelsFahrSwitch {

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

		switch (scale) {
		case "F":
		case "f":
		case "fahrenheit":
		case "Fahrenheit":
			fahrenheit = inputNum;
			celsius = 5.0 / 9.0 * (fahrenheit - 32);
			System.out.println(inputNum + " F");
			System.out.println(celsius + " C");
			break;
		case "C": case "c": case "celsius": case "Celsius":
			celsius = inputNum;
			fahrenheit = (9.0 / 5.0 * celsius) + 32;
			System.out.println(inputNum + " C");
			System.out.println(fahrenheit + " F");
			break;
		default:
			System.out.println("That's not a scale!");
		}
	}
}
```

`Lab 2 - CalculatorSwitch.java`
```java
public class CalculatorSwitch {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		
		System.out.println("Welcome to the world's greatest calculator app!");
		System.out.println("Please enter the first number you'd like to do some math with:");
		double firstNum = sc.nextDouble();

		System.out.println("Please enter the second number you'd like to do some math with:");
		double secondNum = sc.nextDouble();
		sc.nextLine(); // Needed to run next String.
		System.out.println("What kind of math would you like to do? +, -, *, /, %");
		String operator = sc.nextLine(); // Can also just use '.next' instead of nextLine. Comment out 'sc.nextline();'.
		
		switch (operator) {
		case "+": System.out.println(firstNum + secondNum);
			break;
		case "-": System.out.println(firstNum - secondNum);
			break;
		case "*": System.out.println(firstNum * secondNum);
			break;
		case "/": System.out.println(firstNum / secondNum);
			break;
		case "%": System.out.println(firstNum % secondNum);
			break;
		default: System.out.println("Invalid operator.");
		}
	}
}
```

#### while Loops
1. Looping
2. while Loops
3. while Loops - Details
4. Steps in a while Loop
5. Scope
6. do-while Loops
7. Infinite Loops *
8. break and continue Statements
9. Labs

`WhileLoops/src/drills/WhileLoop.java`
```java
public class WhileLoop {

	public static void main(String[] args) {
		// printNumbers();
		mathRandomWhile();
	}

	public static void printNumbers() {
		// Write a while loop to print the numbers 1 to 10 to the screen.
		int num = 1;
		while (num <= 10) {
			System.out.println(num);
			num++;
		}
	}

	public static void mathRandomWhile() {
		// Use Math.random() to write a while loop that will execute as long as a random
		// number is less than 0.7. Print the number inside the loop.
		// Example: double d = Math.random();
		// Make sure to reassign d with a new Math.random() value in the loop body.
		// After the loop, add a statement to print the final value of d.
		double d = Math.random();
		while (d < 0.7) {
			d = Math.random();
			System.out.println(d);
			d = Math.random();
		}
	}
}
```

`WhileLoops/src/drills/WhileLoopSteps.java`
```java
public class WhileLoopSteps {

	public static void main(String[] args) {
		// Write a `while` loop that will accept a number from the user, multiply it by
		// 2, and print the value to the screen. The program should accept data from the
		// user until the user enters zero.
		Scanner sc = new Scanner(System.in);

		System.out.println("Please enter a number: ");
		int num = sc.nextInt();

		// while loop to multiply and get more input...
		while (num != 0) {
			System.out.println(num + " * 2 = " + (num * 2));
			System.out.print("Enter a number: ");
			num = sc.nextInt();
		}
		System.out.println("Finished.");
	}
}
```

`WhileLoops/src/drills/DoWhileLoop.java`
```java
public class DoWhileLoop {

	public static void main(String[] args) {
		// Write a do-while loop to print the numbers 1 to 10 to the screen.
		int x = 1;
		do {
			System.out.println(x);
			x++;
		} while (x <= 10);

		// Use Math.random() to write a do-while loop that will execute as long as a
		// random number is less than 0.7. Print the number inside the loop.
		// Declare a variable outside the loop, and assign a new Math.random() value in
		// the loop body. Then print the number to the screen.
		// Example: double d = Math.random();
		double d;
		do {
			d = Math.random();
			System.out.println(d);
		} while (d < 0.7);
	}
}
```

`WhileLoops/src/drills/WhileLoopBreakContinue.java`
```java
public class WhileLoopBreakContinue {

	public static void main(String[] args) {
		Scanner scan = new Scanner(System.in);
		// Try the loops in the content examples in code.
		// Write a do-while loop that accepts an int from a user, and exits when the
		// user types 0.
//		int num;
//		System.out.print("Enter int numbers. Enter 0 to quit: ");
//
//		// Loop here...
//		do {
//			num = scan.nextInt();
//			System.out.println(num);
//
//		} while (num != 0);
//		System.out.println("Finished");

		// Write an infinite loop that accepts String values from the user.
		// Exit when the user types 'quit'. If the user types a different word, output
		// it to the screen.
		// Hint: check if the user's input equals 'quit' by using the
		// if("quit".equals(YOUR_INPUT_VARIABLE)).
		String userInput;
		System.out.println("Enter a word, 'quit' to exit.");

		while (true) {
			userInput = scan.nextLine();
			if (userInput.equals("quit")) {
				break;
			}
			System.out.println(userInput);
		}
		System.out.println("Infinite loop Finished");
	}
}
```

`Lab 1 - LoopMenu.java`
```java
public class LoopMenu {

	public static void main(String[] args) {
		printMenu();
		java.util.Scanner sc = new java.util.Scanner(System.in);
		String choice = "";

		do {
			choice = sc.next();
			switch (choice) {
			case "1":
				printGreeting();
				printMenu();
				break;
			case "2":
				printAdvice();
				printMenu();
				break;
			case "3":
				printWisdom();
				printMenu();
				break;
			case "4":
				printHelp();
				printMenu();
				break;
			case "5":
				printQuit();
			}
		} while (!choice.equals("5"));
	}

	public static void printMenu() {
		System.out.println("***************************");
		System.out.println("*      Choose a Number:   *");
		System.out.println("* \t1 - Greeting      *");
		System.out.println("* \t2 - Advice        *");
		System.out.println("* \t3 - Wisdom        *");
		System.out.println("* \t4 - Help          *");
		System.out.println("* \t5 - Quit          *");
		System.out.println("***************************");
	}

	public static void printGreeting() {
		System.out.println("Hello!");
	}

	public static void printAdvice() {
		System.out.println("Here is some advice.");
	}

	public static void printWisdom() {
		System.out.println("Here is some wisdom.");
	}

	public static void printHelp() {
		System.out.println("Here is some help.");
	}

	public static void printQuit() {
		System.out.println("Goodbye.");
	}
}
```

`Lab 2 - CalculatorLoop.java`
```java
public class SimpleCalculator {

	public static void main(String[] args) {
		Scanner input = new Scanner(System.in);
		System.out.println("Welcome to Calculator!");
		boolean keepGoing = true;
		do {
			System.out.print("Enter a number: ");
			double num1 = input.nextDouble();
			System.out.print("Enter another number: ");
			double num2 = input.nextDouble();
			System.out.print("What calculation do you want to do? ");
			String op = input.next();

			double result;
			switch (op) {
			case "+":
			case "add":
			case "plus":
				result = num1 + num2;
				System.out.println(num1 + " + " + num2 + " = " + result);
				break;
			case "-":
			case "subtract":
			case "minus":
			case "less":
				result = num1 - num2;
				System.out.println(num1 + " - " + num2 + " = " + result);
				break;
			case "*":
			case "multiply":
			case "times":
				result = num1 * num2;
				System.out.println(num1 + " * " + num2 + " = " + result);
				break;
			case "/":
			case "divide":
			case "over":
				result = num1 / num2;
				System.out.println(num1 + " / " + num2 + " = " + result);
				break;
			case "%":
			case "mod":
			case "modulo":
				result = num1 % num2;
				System.out.println(num1 + " % " + num2 + " = " + result);
				break;
			case "QUIT":
			case "EXIT":
				System.out.println("Exiting.");
				keepGoing = false;
				break;
			default:
				System.out.println("Operation not valid.");
			}
		} while (keepGoing);

		input.close();
	}
}
```

#### Project: Hi/Lo

#### Project: Remote Control Simulator

### Week 1 - Day 4

#### Methods
1. Method Review
2. Methods Instead of Repeating Code
3. Returning Values from Methods
4. Using a Method's return value
5. Sending Data to Methods
6. Defining Parameters
7. Local Variables * (Additional Drill)
8. Pass-by-value *
9. Method Overloading *
10. Labs

`Methods/src/drills/ClassWithMethodsLoop.java`
```java
public class ClassWithMethodsLoop {
	public static void main(String[] args) {

		System.out.println("Calling method1()");

		int counter = 0;
		while (counter < 5) {
			counter++;
			method1();
		}
		System.out.println("main finishing");
	}

	public static void method1() {
		System.out.println("     method1 executing");
	}
}
```

`Methods/src/drills/CalculateBalanceRefactor.java`
```java
public class CalculateBalanceRefactor {
	public static void main(String[] args) {
		double cost = 307.32;
		double balance = cost;

		double payment1 = 42.40;
		balance = balance - payment1;

		printHeader();

//		System.out.println("-----------------");
//		System.out.println("---- BALANCE ----");
//		System.out.println("-----------------");
		System.out.println(balance);
		System.out.println();

		double payment2 = 39.31;
		balance = balance - payment2;

//		System.out.println("-----------------");
//		System.out.println("---- BALANCE ----");
//		System.out.println("-----------------");

		printHeader();

		System.out.println(balance);
		System.out.println();
	}

	public static void printHeader() {
		System.out.println("////////////////////");
		System.out.println("/      BALANCE    /");
		System.out.println("///////////////////");
	}
}
```

`Methods/src/drills/CalculateBalanceReturn.java`
```java
public class CalculateBalanceReturn {
	public static void main(String[] args) {
		double cost = 307.32;
		double balance = cost;

		double payment1 = 42.40;
		balance = balance - payment1;

		printHeader();
		System.out.println(balance);
		System.out.println();

		double payment2 = 39.31;
		balance = balance - payment2;

		printHeader();
		System.out.println(balance);
		System.out.println();
	}

	/*
	 * Refactor printHeader(): Remove its System.out.println statements. Call
	 * buildHeader() and assign its return value to a variable. Output that variable
	 * to the screen.
	 */
	public static void printHeader() {
		System.out.println(buildHeader());
	}

	// Create a method called buildHeader that returns a String
	public static String buildHeader() {
		String header = "/////////////////\n" + "//// BALANCE ////\n" + "/////////////////";
		return header;
	}
}
```

`Methods/src/drills/CalculateTemp.java`
```java
public class CalculateTemp {

	public static void main(String[] args) {
		// 2. Call the method to calculate temperature.
		// Be sure to pass arguments in the correct order.
		// Print the returned value to the screen.
		double theFinalValue = calculateTemp(32.0, 'C');
		System.out.println(theFinalValue);

		theFinalValue = calculateTemp(15.0, 'F');
		System.out.println(theFinalValue);

		theFinalValue = calculateTemp(100.0, 'K');
		System.out.println(theFinalValue);
	}
	// 1. Define a method with the following signature:
	// name: calculateTemp
	// return type: double
	// parameter 1: floating point temperature
	// parameter 2: a character denoting the temperature scale,
	// where 'C' means Celsius and 'F' means Fahrenheit
	//
	// Be sure to put "public static" in front of the method return type and name
	//
	// The method will calculate the alternate temperature
	// using the formulas
	//
	// celsius = (fahrenheit - 32) / 1.8
	// fahrenheit = (celsius * 1.8) + 32
	//
	// If the scale is not 'C' or 'F', print a message to the screen and
	// return the value -999.

	public static double calculateTemp(double theTemp, char scale) {
		double convertedTemp = 999;

		if (scale == 'C') {
			convertedTemp = (theTemp - 32) / 1.8;
		} else if (scale == 'F') {
			convertedTemp = (theTemp * 1.8) + 32;
		} else {
			System.out.println("RTFM!!!!!");
		}
		return convertedTemp;
	}
}
```

`Methods/src/drills/StringManipulation.java`
```java
public class StringManipulation {

	public static void main(String[] args) {
		java.util.Scanner scanner = new java.util.Scanner(System.in);

		System.out.print("Enter a word or phrase: ");
		String phrase = scanner.nextLine();

		System.out.print("Enter a number: ");
		int num = scanner.nextInt();

		// 2. Call addCharacter, passing phrase and num, and assign its return
		// value to a local variable.
		String concatenated = addCharacter(phrase, num);
		// 3. Output the value of the local variable.
		System.out.println(concatenated);
	}

	public static String addCharacter(String input, int numExc) {
		// 1. Declare a local variable "output". Initialize it to the parameter input..
		String output = input;
		// Using a loop, concatenate _numExc_ "!" characters to the local variable
		// output.
		int counter = 0;
		while (counter < numExc) {
			output = output + "!";
			counter = counter + 1;
		}

		// return "output" instead of "input"
		return output;
	}
}
```

`Methods/src/drills/PassByValue.java`
```java
public class PassByValue {

	public static void main(String[] args) {
		int x = 42;
		System.out.println("In main, x is " + x);

		// Call the changeIt method, passing local variable x and another value.
		changeIt(x, 13);

		// Add a System.out.println statement to output this method's
		// local variable x.
		System.out.println("In main, x is " + x);
	}

	public static void changeIt(int x, int y) {
		System.out.println("In changeIt, x is " + x); 
		x = y; // reassigns x from 42 to 13
		System.out.println("In changeIt, x is now " + x);
	}
}
```

`Lab 1 - PowerMethod.java`
```java
public class PowerMethod {

	public static void main(String[] args) {
		// prepare for reading input
		java.util.Scanner scanner = new java.util.Scanner(System.in);

		// prompt the user for the base value
		System.out.print("Enter the base: ");
		double base = scanner.nextDouble();

		// prompt the user for the exponent value
		System.out.print("\nEnter the exponent: ");
		int exp = scanner.nextInt();

		// call the power method
		double value = power(base, exp);

		// display the result
		System.out.println("The result of " + base + " raised to the " + exp + " power is " + value);
		scanner.close();
	}

	public static double power(double base, int exp) {
		double result = 1.0;
		for (int i = 0; i < exp; i++) {
			result = result * base;
		}
		return result;
	}
}
```

`Lab 2 - MPGCalculator.java`
```java
public class MPGCalculator {
	public static void main(String[] args) {
		System.out.println(mpgMethod(16, 100, 150));
		System.out.println(mpgMethod(18, 80383, 80723));
	}

	public static double mpgMethod(double addGal, double prevOdometer, double newOdometer) {
		double mpg = (newOdometer - prevOdometer) / addGal; // miles driven divided by gallons of gas used
		return mpg;
	}
}
```

#### for Loops
1. for Loops
2. A for Loop Diagram
3. for Loop Parts
4. for Loop Body
5. break and continue Statements
6. For Loop - When and Why
7. Labs

`ForLoops/src/drills/ForLoop.java`
```java
public class ForLoop {

	public static void main(String[] args) {
		// Write a for loop to print the numbers 1 to 10 to the screen.
		int i = 0;
		for (i = 1; i <= 10; i++) {
			System.out.println(i);
		}

		// Write the same loop with the loop control variable starting at 0.
		for (i = 0; i <= 10; i++) {
			System.out.println(i);
		}
	}
}
```

`ForLoops/src/drills/ForLoopBody.java`
```java
public class ForLoopBody {

	public static void main(String[] args) {
		//Write a for loop to print the numbers 10 to 1 to the screen.
		for (int i = 10 ; i >= 1; i--) {
			System.out.println(i);
		}
		
		//Write a for loop to find the sum of the values 1 to 10. Print the sum to the screen.
		int sum = 0; 
		for (int a = 1 ; a <= 10; a++) {
			sum += a;
		}
		System.out.println(sum);
		
		//Write a for loop to print the values 1 to 5. Output should be comma-separated: 1, 2, 3, 4, 5.
		//Hint: the loop will need to check which iteration it is on to prevent a comma showing after 5.
		for (int i = 1 ; i <= 5; i++) {
			System.out.print(i);
			
			if (i != 5) {
				System.out.print(", ");
			}
		}
	}
}
```

`Forloops/src/drills/ForLoopBody2.java`
```java
public class ForLoopBody2 {
	public static void main(String[] args) {
		/*
		 * The for loops below have errors. Copy each loop and paste below the block
		 * comment. Fix the code so that it can compile.
		 */
		// Loop 1
		// int x = 0; // Can't declare x both here and in the for().
		for (int y = 0, x = 10; x + y < 15; x++, y++) {
			System.out.println(x + y);
		}

		// Loop 2
		// Can't declare two different type in the initialization.
		// for(int a = 0, short b = 4; a < 5; a++, b++) {
		for (int a = 0, b = 4; a < 5; a++, b++) {
			System.out.println("a is " + a + ", b is " + b);
		}

		// Loop 3
		// If q is declared in the for(), it will be out of scope after the loop body.
		// for (int q = 5; q < 10; q++) {
		int q = 5;
		for (q = 5; q < 10; q++) {
			System.out.println(q);
		}
		System.out.println("q is now " + q);
	}
}
```

`ForLoops/src/drills/ForLoopBreakContinue.java`
```java
public class ForLoopBreakContinue {

	public static void main(String[] args) {
		// Try the loops in the examples above in code.
//		System.out.println("Loop 1...");
//		// COPY-PASTE LOOP 1 HERE
//		// Exit the loop the first time i % 2 == 0
//		for (int i = 1; i <= 10; i += 1) {
//			if (i % 2 == 0) {
//				break;
//			}
//			System.out.println(i);
//		}

//		System.out.println("Loop 2...");
//		// COPY-PASTE LOOP 2 HERE
//		// Go to the next iteration every time i % 2 == 0
//		for (int i = 0; i <= 10; i += 1) {
//			if (i % 2 == 0) {
//				continue;
//			}
//			System.out.println(i);
//		}

		System.out.println("Loop 3...");
		// Write a loop that prints the numbers from 1 to 30, skipping
		// multiples of 3.
		for (int i = 1; i <= 30; i += 1) {
			if (i % 3 == 0) {
				continue;
			}
			System.out.println(i);
		}
	}
}
```

`Lab 1 - Mult2.java`
```java
public class Mult2 {

	public static void main(String[] args) {
		for (int i = 1; i <= 16; i += 1) {
			if (i % 2 != 0) {
				continue;
			}
			System.out.println(i);
		}
	}
}
```

`Lab 2 - Pow2.java`
```java
public class Pow2 {

	public static void main(String[] args) {
		int i = 0;
		for (i = 1; i <= 16; i += 1) {
			if (i % 2 != 0) {
				continue;
			}
			System.out.println(i + " * " + i + " = " + (i * i));
		}
	}
}
```

`Lab 3 - Factorial.java`
```java
public class Factorial {

	public static void main(String[] args) {

		int i = 0;
		int factorial = 1;

		// A integer overflows after 13!
		// for(i = 1; i <= 20; i = i + 1)

		for (i = 1; i <= 10; i = i + 1) {
			factorial = factorial * i;
			System.out.println(i + "! = " + factorial);
		}
	}
}
```

#### Project: Fizz Buzz

#### Project: Fibonacci Series

### Week 1 - Day 5

#### Numeral Systems
1. Counting and Tallying
2. Positional Notation
3. Numeral Systems for Programming
4. Numeric Literals in Java
5. The printf() Method

```java
11001 - (1 * 16) + (1 * 8) + (0 * 4) + (0 * 2) + (1 * 1)
//25

00011001 - (0*128) + (0*64) + (0*32) + (1*16) + (1*8) + (0*4) + (0*2) + (1*1)
//still 25
```

```java
int i = 012 // Ocatal (1*8 + 2*1)

int i = 0x12 // Hexadecimal (1*16 + 2*1)
int i = 0xa // Hexadecimal (10)

int i = 0b12 // Binary (No 2 in Binary)
int i = 0b10 // Binary (1*2 + 0*1)
```

```java
double num1 = 23.785;
double num2 = 34.64443;
System.out.printf("%.2f  %n", num1+num2);

%% - literal %
n - new line
d - as a decimal integer
o - as an octal integer
x - as a hexadecimal integer
f - as a floating-point number
a - as a floating-point number in hexadecimal
s - as a string
```

#### Data Types in Java
1. Data Types You've Used
2. Memory and Java
3. Bits and Bytes
4. Counting in Binary
5. Most Significant Bit
6. Primitive Data Types
7. Primitives and Memory
8. Variable Types Tell Java What to Do
9. Declaring and Assigning Primitive Values
10. Floating Point Literals
11. long for Large Numbers
12. switch and Data Types
13. Labs

`DataTypes/com.skilldistillery.datatypes.drills.CharAsInteger`
```java
public class CharAsInteger {

	public static void main(String[] args) {
		// Declare a char variable and assign it the value 65.
		// Print it to the screen.
		char start = 65;
		System.out.println(start);

		// Use the += operator to add 25 to your variable.
		// Now print it to the screen.
		start += 25;
		System.out.println(start);
	}
}
```

`DataTypes/com.skilldistillery.datatypes.drills.CharPrinting`
```java
public class CharPrinting {

	public static void main(String[] args) {
		char variable = 'A';
		System.out.println(variable);
		// Add the line System.out.println(variable + 1); to main().
		// What is the output?
		System.out.println(variable + 1);

		// Based on its output, what does the `+` operator appear to do?
		// Add
	}
}
```

`DataTypes/com.skilldistillery.datatypes.drills.DeclaringPrimitives`
```java
public class DeclaringPrimitives {

	public static void main(String[] args) {
		// Declare a byte variable and assign the value 128. What happens? Assign it a
		// valid value.
		byte hello = 127; // type mismatch convert to int

		// Create a switch statement for your variable.
		// Have a case for each of the values 127, -128, 0, 'A', 128, '\u0000'.
		// Which values cause compiler errors?
		switch (hello) {
		case 127:
		case -128:
//    	case 0:
		case 'A':
		case '\u0000':
		}

		// Declare a int variable and assign it a value.
		int value = 127;

		// Again create a switch statement.
		// Have a case for each of the values 127, -128, 'A', 128, '\u0000'.
		switch (value) {
		case 127:
		case -128:
//		case 0:
		case 'A':
		case 128:
		case '\u0000':
		}
	}
}
```

`DataTypes/com.skilldistillery.datatypes.drills.FloatValues`
```java
public class FloatValues {

	public static void main(String[] args) {
		// Copy f1 to f8 in text here. Comment out values that do not work.
		float f1 = 0.0f; //
		float f2 = 1f; //
		float f3 = 1; //
		float f4 = 0b10101; // binary number - an int
//	  float f5 = 0b10101f; // NO, don't use F with binary numbers
		float f6 = 0xF16F; // F doesn't do anything here, it is a hex digit
		float f7 = 0761; // octal number
		float f8 = 0761F; // octal number with F
	}
}
```

`Lab 1 - Overflow.java`
```java
public class Overflow {

	public static void main(String[] args) {
		int big = 2_147_483_647;
		int bigger = big + 1;

		System.out.println(big);
		System.out.println(bigger);
	}
}
```

`Lab 2 - ValidInt.java`
```java
public class ValidInt {

	public static void main(String[] args) {
		int validInt = 12;
		long longInt = validInt;
		System.out.println(longInt);
	}
}
```

#### Casting Data Types
1. Implicit Type Conversions
2. Promotion of Data Types in Arithmetic
3. Promotion in Integer Arithmetic
4. The Cast Operator
5. Casting Hints
6. Labs

```java
// byte converted to short;
byte b1 = 16;
short s1 = b1;

// short converted to float
short s2 = 14;
float f2 = s2;

// int converted to float
int i3 = 2105;
float f3 = i3;

// long converted to float
long l4 = 10000L;
float f4 = l4;

// char converted to double
char c5 = 'A';
double d5 = c5;

// converting byte to char does not work
byte b6 = 5;
char c6 = b6;  // DOES NOT COMPILE per JLS 5.1.4

// short and char do not convert because short is signed while char is not
short s7 = 55;
char c7 = s7;  // DOES NOT COMPILE
```

`CastingDataTypes/com.skilldistillery.casting.drills.Promotion`
```java
public class Promotion {

	public static void main(String[] args) {
		// Try changing the types of the variables resultIF, resultID, and resultCI
		// to the smaller or less-precise type, e.g. int resultIF.
		// What compiler errors do you see?
		int i = 0;
		float f = 1.0f;

		float resultIF = i * f; // int*float promoted to float*float
		double resultID = i * 2.0; // int*double promoted to double*double

		System.out.println(resultIF);
		System.out.println(resultID);
		char c = 'A';
		int resultCI = c + 1; // char+int promoted to int+int
	}
}
```

`CastingDataTypes/com.skilldistillery.casting.drills.Division`
```java
public class Division {

	public static void main(String[] args) {
		// This drill is divided into methods so that you can run one at a time.

		// For each method, add answers to the questions
		// "Necessary variable type?" and "Expected value?"
		// Then uncomment the arithmetic operation and change "xxx" to the type you
		// expect.
		// Was your type legal?
		// Uncomment the print statements and run the program to see the actual value.
		// Note: necessary data type means the smallest necessary type.
		method1();
//		method2();
//		method3();
	}

	static void method1() {
		short s1 = 5;
		byte b1 = 3;
		int result1 = s1 / b1;
		System.out.println("result1 is " + result1);
		// Necessary variable type? int
		// Expected value? result1 is 1 (.6)
		// Actual value: result1 is 1
		// Promotion that occurred: byte>int
	}

	static void method2() {
		char c2 = 3;
		byte b2 = 6;
		int result2 = c2 / b2;
		System.out.println("result2 is " + result2);
		// Necessary variable type? int
		// Expected value? result2 is 0 (.5)
		// Actual value: result2 is 0
		// Promotion that occurred: byte>int
	}

	static void method3() {
		// This operation does not require you to choose a result type.
		int i3 = 4;
		int i4 = 8;
		double result3 = i3 / i4;
		System.out.println("result3 is " + result3);
		// Expected value? result3 is 0.0
		// Actual value: result3 is 0.0
		// Promotion that occurred: int>double
	}
}
```

`Lab 1 - Floor.java`
```java
public class Floor {

	public static void main(String[] args) {
		java.util.Scanner scanner = new java.util.Scanner(System.in);

		System.out.println("Please enter a floating point number: ");
		double variable = scanner.nextDouble();

		if (variable < 0 && variable % 1 != 0) {
			variable -= 1; // use += for positive number round up
		}
		int result = (int) variable;
		System.out.println(result);

		scanner.close();
	}
}
```

`Lab 2 - Ceiling.java`
```java
public class Ceiling {

	public static void main(String[] args) {
		java.util.Scanner scanner = new java.util.Scanner(System.in);

		System.out.println("Please enter a floating point number: ");
		double variable = scanner.nextDouble();

		if (variable < 0 && variable % 1 != 0) {
			variable -= 1; // use += for positive number round up
		}
		if (variable > 0) {
			variable += 1; // use += for positive number round up
		}
		int result = (int) variable;
		System.out.println(result);

		scanner.close();
	}
}
```

`Lab 3 - Round.java`
```java
public class Round {

	public static void main(String[] args) {
		java.util.Scanner scanner = new java.util.Scanner(System.in);

		float variable = 0.0f;

		System.out.println("Please give a float number: ");
		variable = scanner.nextFloat();
		int result = (int) variable;

		System.out.println(result);
		scanner.close();
	}
}
```

#### Homework Project: Make Change (Cash Register)

### Week 1 - Day 6

#### Arrays
1. Variables - Single vs. Collections
2. Arrays
3. Declaring an Array
4. Creating an Array
5. Array Element Default Values
6. Reading and Storing Data
7. Array Initialization Shortcuts
8. Iterating Arrays
9. Passing Arrays to Methods
10. Three Ways of Creating Arrays
11. Labs

`Arrays/src/drills/ArrayDeclare.java`
```java
public class ArrayDeclare {

	public static void main(String[] args) {
		// Declare a variable for an array of String objects to hold the name of each
		// weekWeek 1 - Day.
		String[] weekWeek 1 - Days;
		weekWeek 1 - Days = new String[7];

		// Declare a variable to hold letter grades for each of a student's six classes.
		char[] grades = new char[6];

		// Declare a variable to hold the average monthly precipitation for a year.
		double[] monthlyPrecipitation = new double[12];
	}
}
```

`Arrays/src/drills/ArrayCreate.java`
```java
public class ArrayCreate {

	public static void main(String[] args) {
		// Declare a variable for an array of String objects to hold the name of each
		// weekWeek 1 - Day.
		// Initialize the variable to hold 7 Strings.
		String[] weekWeek 1 - Days;
		weekWeek 1 - Days = new String[7];

		// Declare a variable to hold letter grades for each of a student's six classes.
		// Initialize the variable to hold 6 chars.
		char grades[];
		grades = new char[6];

		// Declare a variable to hold the average monthly precipitation for a year.
		// Initialize the variable to have the correct number of double slots.
		double[] avgMonthlyPrecip;
		avgMonthlyPrecip = new double[12];

		// NOTE: as you can see above, whitespace does not matter.
	}
}
```

`Arrays/src/drills/ArrayAccess.java`
```java
public class ArrayAccess {

	public static void main(String[] args) {
		// Store the name of each weekWeek 1 - Day at the correct index.
		String[] weekWeek 1 - Days = new String[7];
		weekWeek 1 - Days[0] = "SunWeek 1 - Day";
		weekWeek 1 - Days[1] = "MonWeek 1 - Day";
		weekWeek 1 - Days[2] = "TuesWeek 1 - Day";
		weekWeek 1 - Days[3] = "WednesWeek 1 - Day";
		weekWeek 1 - Days[4] = "ThursWeek 1 - Day";
		weekWeek 1 - Days[5] = "FriWeek 1 - Day";
		weekWeek 1 - Days[6] = "SaturWeek 1 - Day";

		// Store the grade A in the FIRST index of the array,
		// and C in the LAST index of the array.
		char grades[] = new char[6];
		grades[0] = 'A';
		grades[5] = 'C';

		// Run the program and check the output to see if you were correct.
		System.out.println("WeekWeek 1 - Days:");
		for (int i = 0; i < 7; i++) {
			System.out.println(i + ":" + weekWeek 1 - Days[i]);
		}
		System.out.println("Grades:");
		for (int i = 0; i < 6; i++) {
			System.out.println(i + ":" + grades[i]);
		}
	}
}
```

`Arrays/src/drills/ArrayAccess2.java`
```java
public class ArrayAccess2 {

	public static void main(String[] args) {
		// Access all the B grades in the grades array and output them to the screen.
		char[] grades = { 'C', 'F', 'B', 'A', 'C', 'B' };
		System.out.println(grades[2]); // B
		System.out.println(grades[5]); // B

		// Use values from the firstNames and lastNames arrays to create the names
		// Sarah Dobbs and Davey Jones.
		// Output the names to the screen.
		String firstNames[] = { "Matthew", "Mark", "Davey", "Sarah", "Linda" };
		String lastNames[] = { null, "Dobbs", "Cool", "Symbol", "Longshanks", "Jones" };
		System.out.println(firstNames[3] + " " + lastNames[1]); // Sarah Dobbs
		System.out.println(firstNames[2] + " " + lastNames[5]); // Davey Jones

		// Declare and initialize an array containing your
		// pet's name and the street you grew up on.
		// (If you do not have a pet, use the value null.)
		String petNames[] = { "Spot", "Max" };
		String street[] = { "Main St.", "1st St." };
		System.out.println(petNames[0] + " " + street[1]); // Spot 1st St.

		// Reassign the same array and initialize it with your middle
		// name and a U.S. President's last name.
		// (Use the array shortcut. If you do not have a middle name, use the value
		// null.)
		petNames = new String[] { "Spot", "Julie" };
		System.out.println(petNames[1] + " " + street[0]); // Julie Main St.
	}
}
```

`Arrays/src/drills/Iterating.java`
```java
public class Iterating {

	public static void main(String[] args) {
		// Iterate through the names array to print the index of the name,
		// and the name, e.g. 0 : Mike.
		String[] names = { "Mike", "Davey", "Peter", "Mickey" };
		for (int idx = 0; idx < names.length; idx++) {
			System.out.println(names[idx]);
		}

		// Iterate through the precip array, but only print
		// values greater than 2.5.
		double[] precip = new double[] { 3.2, 0.5, 1.7, 2.8, 2.0, 3.1, 0.0, 0.2, 9.0 };
		for (int i = 0; i < precip.length; i++) {
			if (precip[i] >= 2.5) {
				System.out.println(precip[i]);
			}
		}

		// Iterate through the Week 1 - DaysOfWeek array, but do not print
		// SunWeek 1 - Day or SaturWeek 1 - Day.
		String[] Week 1 - DaysOfWeek = { "SunWeek 1 - Day", "MonWeek 1 - Day", "TuesWeek 1 - Day", "WednesWeek 1 - Day", "ThursWeek 1 - Day", "FriWeek 1 - Day", "SaturWeek 1 - Day" };
		for (int i = 0; i < Week 1 - DaysOfWeek.length; i++) {
			if (Week 1 - DaysOfWeek[i].equals("SunWeek 1 - Day") || Week 1 - DaysOfWeek[i].equals("SaturWeek 1 - Day")) {
				continue;
			}
			System.out.println(Week 1 - DaysOfWeek[i]);
		}

		// After iterating, print the Week 1 - DaysOfWeek array itself:
		// System.out.println(Week 1 - DaysOfWeek).
		// Note the format, and what doesn't get printed.
		System.out.println(Week 1 - DaysOfWeek);
	}
}
```

`Arrays/src/drills/ArrayReferences.java`
```java
public class ArrayReferences {

	public static void main(String[] args) {
		String[] Week 1 - DaysOfWeek = new String[7];
		Week 1 - DaysOfWeek[0] = "SunWeek 1 - Day";
		Week 1 - DaysOfWeek[1] = "MonWeek 1 - Day";
		Week 1 - DaysOfWeek[2] = "TuesWeek 1 - Day";
		Week 1 - DaysOfWeek[3] = "WednesWeek 1 - Day";
		Week 1 - DaysOfWeek[4] = "ThursWeek 1 - Day";
		Week 1 - DaysOfWeek[5] = "FriWeek 1 - Day";
		Week 1 - DaysOfWeek[6] = "SaturWeek 1 - Day";

		// Print the array
		for (int i = 0; i < Week 1 - DaysOfWeek.length; i++) {
			System.out.print(Week 1 - DaysOfWeek[i]);
			if (i != Week 1 - DaysOfWeek.length - 1) { // don't do this for the last index
				System.out.print(", ");
			}
		}
		System.out.println();

		// * Call the changeArray method and pass the Week 1 - DaysOfWeek array reference.
		ArrayReferences test = new ArrayReferences();
		test.changeArray(Week 1 - DaysOfWeek);

		// Print the array again to see that its elements have changed,
		// but it is the same array.
		for (int i = 0; i < Week 1 - DaysOfWeek.length; i++) {
			System.out.print(Week 1 - DaysOfWeek[i]);
			if (i != Week 1 - DaysOfWeek.length - 1) { // don't do this for the last index
				System.out.print(", ");
			}
		}

		// * Refactor the printing of the array into a method and pass it the Week 1 - DaysOfWeek
		// array reference.
//		test.printArray(Week 1 - DaysOfWeek);
	}

	public void changeArray(String[] inputArr) {
		// * Change WednesWeek 1 - Day to "HUMPWeek 1 - Day" and FriWeek 1 - Day to "Viernes".
		// * (There is no need to iterate, just change the right index.)
		inputArr[3] = "HUMPWeek 1 - Day";
		inputArr[5] = "Viernes";

		// * Reassign inputArr to a new array containing the values
		// * "Su", "M", "T", "W", "Th", "F", "Sa"
		inputArr = new String[] { "Su", "M", "T", "W", "Th", "F", "Sa" };
	}

	public void printArray(String[] arr) {
		for (int i = 0; i < arr.length; i++) {
			System.out.print(arr[i]);
			if (i != arr.length - 1) { // don't do this for the last index
				System.out.print(", ");
			}
		}
	}
}
```

`Labs 1 - Week 1 - DayOfWeekIterating1.java`
```java
public class Week 1 - DayOfWeekIterating1 {
	public static void main(String[] args) {
		String[] Week 1 - DaysOfWeek = { "SunWeek 1 - Day", "MonWeek 1 - Day", "TuesWeek 1 - Day", "WednesWeek 1 - Day", "ThursWeek 1 - Day", "FriWeek 1 - Day", "SaturWeek 1 - Day" };

		for (int i = 0; i < Week 1 - DaysOfWeek.length; i++) {
			if (i != 0 && i != Week 1 - DaysOfWeek.length - 1) {
				System.out.println(Week 1 - DaysOfWeek[i]);
			}
		}
	}
}
```

`Labs 1 - Week 1 - DayOfWeekIterating2.java`
```java
public class Week 1 - DayOfWeekIterating2 {
	public static void main(String[] args) {
		String[] Week 1 - DaysOfWeek = { "SunWeek 1 - Day", "MonWeek 1 - Day", "TuesWeek 1 - Day", "WednesWeek 1 - Day", "ThursWeek 1 - Day", "FriWeek 1 - Day", "SaturWeek 1 - Day" };

		for (int i = 0; i < Week 1 - DaysOfWeek.length; i++) {
			if (Week 1 - DaysOfWeek[i].equals("SunWeek 1 - Day") || Week 1 - DaysOfWeek[i].equals("SaturWeek 1 - Day")) {
				continue;
			}
			System.out.println(Week 1 - DaysOfWeek[i]);
		}
	}
}
```

`Labs 2 - AverageScores.java`
```java
public class AverageScores {

	public static void main(String[] args) {
		int[] scores = new int[5];

		java.util.Scanner scanner = new java.util.Scanner(System.in);

		System.out.println("Enter scores:");
		for (int i = 0; i < scores.length; i++) {
			int scoreNum = i + 1;
			System.out.print("Score " + scoreNum + ": ");
			scores[i] = scanner.nextInt();
		}

		// Call the test method
		AverageScores test = new AverageScores();
		test.testCalculateAverage();

		// Test calculateAverage(); Non-Static Instance
		AverageScores aveScore = new AverageScores();
		double average = aveScore.calculateAverage(scores);

//		double average = new AverageScores().calculateAverage(scores); //DO NOT CODE LIKE THIS

		System.out.println("The average score is: " + average);
		scanner.close();

	}

	public double calculateAverage(int[] scores) {
		double theAverage = 0.0;

		// variable to hold the sum of all scores
		double sum = 0.0;
		for (int i = 0; i < scores.length; i++) {
			sum += scores[i];
		}

		theAverage = sum / scores.length; // divide by the length because
											// we don't know how long the passed-in
											// array is (even though we're the ones passing it)
		return theAverage;
	}

	public void displayAverage(double average) {
		System.out.println(average);
	}

	public void testCalculateAverage() {
		int[] ints = { 70, 65, 80, 97 };

		double expected = 78.0;

		// Calculate the average to see what the method produces
		double result = calculateAverage(ints); // Non-Static to Non-Static

		// Now test the result
		if (expected == result) {
			System.out.println("Passed");
		} else {
			System.out.println("Failed, expected " + expected + " but got " + result);
		}
	}
}
```

`Labs 3 - RandomString.java`
```java
public class RandomString {
	public static void main(String[] args) {
		String[] animals = { "Bear", "Fox", "Bobcat" };

		for (int i = 0; i < 10; i++) {
			int index = (int) (Math.random() * animals.length);
			System.out.println(animals[index]);
		}
	}
}
```

#### Introduction to Objects
1. Classes
2. Creating Objects
3. Reference Variables
4. State and Behavior
5. Field Initialization
6. The static Keyword *
7. Some Objects You've Already Met
8. Labs

`IntroToObjects/src/drills/SphereCreation.java`
```java
public class SphereCreation {

	public static void main(String[] args) {
		// Create three Sphere "objects."
		// 1. A baseball, radius 3.7
		Sphere baseball = new Sphere();
		baseball.radius = 3.7;

		// 2. A basketball, radius 12.0
		Sphere basketball = new Sphere();
		basketball.radius = 12.0;

		// 3. Mercury, radius 244 million centimeters
		// Try writing this as 244_000_000.0 or 244e5
		Sphere mercury = new Sphere();
		mercury.radius = 244_000_000.0;

		// Print each object's volume to the screen using System.out.println.
		System.out.println(baseball.radius);
		System.out.println(basketball.radius);
		System.out.println(mercury.radius);
	}
}
```

`IntroToObjects/src/drills/SphereReferences.java`
```java
public class SphereReferences {

	public static void main(String[] args) {
		// Create another reference called otherSphereRef and assign sphRef to it,
		// so that both references refer to the same Sphere object.

		Sphere sphRef = new Sphere();
		sphRef.radius = 10.0;
		System.out.println("Original sphRef radius: " + sphRef.radius);

		// Change otherSphereRef's radius.
		Sphere otherSphereRef = sphRef;
		otherSphereRef.radius = 20.0;

		// Output otherSphereRef's radius to the screen.
		System.out.println("Second sphRef radius: " + otherSphereRef.radius);

		// Output sphRef's radius to the screen. It should have changed.
		System.out.println("Changed original sphRef: " + sphRef.radius);
	}
}
```

`IntroToObjects/src/drills/SphereWithColor.java`
```java
Example
```

`IntroToObjects/src/drills/SphereWithColorTest.java`
```java
Example
```

```java
//Static CarManufacturer.java
public class CarManufacturer {
	public static void main() {
		Car.test2Understanding();
	}
}

//Static Car.java
public class Car {
	public static void test2Understanding() {
		System.out.println("Test");
	}

}

//Non-Static CarManufacturer.java
public class CarManufacturer {
	public static void main () {
		Car anotherCar = new Car();
		anotherCar.test1Understanding(); 
	}
}

//Non-Static Car.java
public class Car {
	public void test1Understanding() {
		System.out.println("Test");
	}

}
```

```java
//java.util.Scanner
java.util.Scanner scanner = new java.util.Scanner(System.in);
System.out.print("Enter the radius of the sphere: ");
double radius = scanner.nextDouble();
scanner.close();

//String: We often do not see new, this is because Strings are so important there are shortcuts to create instances.

//System.out.println()
//The System class has a static field out, which has a method println
```

`Lab 1 - Car.java`
```java
public class Car {
	public String make;
	public String model;
	public String color;
	public int numberOfWheels;
	public int purchasePrice;

	public String getCarData() {
		return "Make: " + make + "\n Model: " + model + "\n Color: " + color + "\n Number of Wheels: " + numberOfWheels
				+ "\n Purchase Price: " + purchasePrice;
	}

	public void displayCar() {
		System.out.println(getCarData());
	}
}
```

`Lab 2 - CarTester.java`
```java
public class CarTester {

	public static void main(String[] args) {
		Car newCar = new Car();
		newCar.make = "Jeep";
		newCar.model = "Rubicon";
		newCar.color = "White";
		newCar.numberOfWheels = 4;
		newCar.purchasePrice = 80000;

		newCar.displayCar();

		Car car2 = new Car();
		car2.make = "Tesla";
		car2.model = "Model Y";
		car2.color = "White";
		car2.numberOfWheels = 4;
		car2.purchasePrice = 53000;
		System.out.println(car2.getCarData());
	}
}
```

`Lab 3 - DMVSimulator.java`
```java
public class DMVSimulator {
	public static void main(String[] args) {
		java.util.Scanner scanner = new java.util.Scanner(System.in);

		System.out.print("Enter Make: ");
		String make = scanner.next();

		System.out.print("Enter Model: ");
		String model = scanner.next();

		System.out.print("Enter Color: ");
		String color = scanner.next();

		System.out.print("Enter Number of Wheels: ");
		int wheels = scanner.nextInt();

		System.out.print("Enter Purchase Price: $");
		int price = scanner.nextInt();

		System.out.println(make + " " + model + " " + color + " " + wheels + " " + price);

		System.out.print("Calculate tax 'C' or Exit 'E': ");
		String calculateTax = scanner.next();

		if (calculateTax.equals("C") || calculateTax.equals("c")) {
			System.out.println("Price: $" + price + " Tax: $" + (price * 0.01 * wheels));
		} else if (calculateTax.equals("E") || calculateTax.equals("e")) {
			System.out.println("Goodbye!");
			scanner.close();
		}
	}
}
```

#### Project: Deaf Grandma

### Week 1 - Day 7

#### Advanced For Loops
1. Nested for Loops
2. Enhanced For Loops
3. Break and Continue With Enhanced For Loops
4. Labs

`AdvancedForLoops/src/drills/NestedFor1.java`
```java
public class NestedFor1 {

	public static void main(String[] args) {
		for (int outer = 1; outer <= 2; outer++) {
			for (int inner = 1; inner <= 10; inner++) {
				int product = outer * inner;
				System.out.print(product + "\t");
			}
			System.out.println();
		}
		// Run the above code.
		// How many times does the the second output statement execute? 2*10
	}
}
```

`AdvancedForLoops/src/drills/NestedFor2.java`
```java
public class NestedFor2 {

	public static void main(String[] args) {
		for (int outer = 0; outer < 5; outer++) {
			for (int inner = 0; inner < 10; inner++) {
				System.out.print(inner + " "); // prints our space in nest loop
			}
			System.out.println(); // inside for loop will make a new line
		}

		// Write a nested for loop to print the numbers 0 to 9 five times.
		// Output:
		// 0 1 2 3 4 5 6 7 8 9
		// 0 1 2 3 4 5 6 7 8 9
		// 0 1 2 3 4 5 6 7 8 9
		// 0 1 2 3 4 5 6 7 8 9
		// 0 1 2 3 4 5 6 7 8 9
	}
}
```

`AdvancedForLoops/src/drills/ForEach.java`
```java
public class ForEach {

	// Use the code in each "forLoop" method to write a foreach loop
	// in the corresponding "forEachLoop" method. Verify that the loop outputs
	// are the same.
	public static void main(String[] args) {
		forLoop1();
		forEachLoop1();
		forLoop2();
		forEachLoop2();
		forLoop3();
		forEachLoop3();
	}

	static void forLoop1() {
		int[] intArr = { 10, 20, 30, 40 };
		for (int i = 0; i < intArr.length; i++) {
			int num = intArr[i];
			System.out.print(num + " ");
		}
		System.out.println("--end forLoop1");
	}

	static void forEachLoop1() {
		int[] intArr = { 10, 20, 30, 40 };
		for (int num : intArr) {
			System.out.print(num + " ");
		}
		System.out.println("--end forEachLoop1");
	}

	static void forLoop2() {
		String[] strings = new String[4];
		strings[0] = "First";
		strings[1] = "Second";
		strings[2] = "Third";
		strings[3] = "Fourth";
		for (int i = 0; i < strings.length; i++) {
			String s = strings[i];
			System.out.print(s + " ");
		}
		System.out.println("--end forLoop2");
	}

	static void forEachLoop2() {
		String[] strings = new String[4];
		strings[0] = "First";
		strings[1] = "Second";
		strings[2] = "Third";
		strings[3] = "Fourth";
		for (String s : strings) {
			System.out.print(s + " ");
		}
		System.out.println("--end forEachLoop2");
	}

	static void forLoop3() {
		double doubleArr[] = { 1.1, 2.2, 3.3, 4.4 };
		for (int i = 0; i < doubleArr.length; i++) {
			System.out.print(doubleArr[i] + " ");
		}
		System.out.println("--end forLoop3");
	}

	static void forEachLoop3() {
		double doubleArr[] = { 1.1, 2.2, 3.3, 4.4 };
		// foreach loop here
		for (double d : doubleArr) {
			System.out.print(d + " ");
		}
		System.out.println("--end forEachLoop3");
	}
}
```

`AdvancedForLoops/src/drills/ForEachBreakContinue.java`
```java
public class ForEachBreakContinue {

	public static void main(String[] args) {
		// Write a foreach loop to display only odd numbers.
		// Output: 55 105 99 71 39 43
		int[] odds = new int[] { 55, 105, 99, 71, -100, 39, 43 };
		for (int num : odds) {
			if (num % 2 == 0) {
				continue;
			}
			System.out.print(num + " ");
		}

		System.out.println();

		// Change the loop to break if -100 is found.
		// Output: 32 154 34 54
		int[] wow = new int[] { 32, 154, 34, 54, -100, 39, 43 };
		for (int num : wow) {
			if (num == -100) {
				break;
			}
			System.out.print(num + " ");
		}
	}
}
```

`Lab 1 - MinMaxFor.java`
```java
public class MinMaxFor {
	public static void main(String[] args) {
		// Write a program that declares an array of five integers, int[] numbers = {28,
		// 33, 55, 21, 35};.
		int numbers[] = { 28, 33, 55, 21, 35 }; 
		int min = numbers[0];
		int max = numbers[0];

		// Use a for loop to determine the smallest and largest number in the array, and
		// print them.
		for (int i = 1; i < numbers.length; i++) {
			if (min > numbers[i]) {
				min = numbers[i];
			}
			if (max < numbers[i]) {
				max = numbers[i];
			}
		}
		System.out.println("Min: " + min);
		System.out.println("Max: " + max);
	}
}
```

`Lab 2 - MinMaxForEach.java`
```java
public class MinMaxForEach {
	public static void main(String[] args) {
		int numbers[] = { 28, 33, 55, 21, 35 };
		int min = numbers[0];
		int max = numbers[0];

		for (int num : numbers) {
			if (min > num) {
				min = num;
			}
			if (max < num) {
				max = num;
			}
		}
		System.out.println("Min: " + min);
		System.out.println("Max: " + max);
	}
}
```

`Lab 3 - MinMaxWhile.java`
```java
public class MinMaxWhile {
	public static void main(String[] args) {
		int numbers[] = { 28, 33, 55, 21, 35 };
		int min = numbers[0];
		int max = numbers[0];

		int i = 0;
		while (i < numbers.length) {
			if (min > numbers[i]) {
				min = numbers[i];
			}
			if (max < numbers[i]) {
				max = numbers[i];
			}
			i++;
		}
		System.out.println("Min: " + min);
		System.out.println("Max: " + max);
	}
}
```

`Lab 4 - MinMaxPrompt.java`
```java
public class MinMaxPrompt {
  public static void main(String[] args) {
    java.util.Scanner keyboard = new java.util.Scanner(System.in);

    int numValues = 5;
    int[] numbers = new int[numValues];

    for (int i = 0; i < numbers.length; i++) {
      System.out.print("Enter an integer: ");
      numbers[i] = keyboard.nextInt();
    }
    keyboard.close();

    int min = numbers[0];
    int max = numbers[0];

    for (int num : numbers) {
      if (min > num) {
        min = num;
      }
      if (max < num) {
        max = num;
      }
    }
    System.out.println("Min: " + min);
    System.out.println("Max: " + max);
  }
}
```

#### Advanced Arrays
1. Array Syntax
2. Returning Array References from Methods
3. Arrays of Arrays
4. Accessing Elements of Multidimensional Arrays
5. Iterating Multidimensional Arrays
6. ForEach Loops for Iterating Arrays
7. Multidimensional Array Shortcuts
8. Variable Arguments Arrays *
9. Labs

`AdvancedArrays/com.skilldistillery.advancedarrays.drills.ArrayOfObjects`
```java
//PopStar.java
public class PopStar {
	public String name;

	public void sing() {
		// Have the PopStar print their name to the screen, as part of some kind of
		// lyric.
		// Be creative.
		System.out.print("My name is " + name);
		int numVowels = name.length();
		System.out.print(", h");
		for (int i = 0; i < numVowels; i++) {
			System.out.print("o");
		}
		System.out.println("!!");
	}
}

//ArrayOfObjects.java
public class ArrayOfObjects {

	public static void main(String[] args) {
		// Instantiate an Array to hold PopStar objects
		PopStar[] theBeatles = new PopStar[4];

		// Create PopStar instances and add them to the array
		PopStar songWriter1 = new PopStar();
		songWriter1.name = "Paul";
		theBeatles[0] = songWriter1;

		PopStar songWriter2 = new PopStar();
		songWriter2.name = "John";
		theBeatles[1] = songWriter2;

		PopStar anotherBeatle = new PopStar();
		anotherBeatle.name = "George";
		theBeatles[2] = anotherBeatle;

		theBeatles[3] = new PopStar();
		theBeatles[3].name = "Ringo";

		// Call the method allSing
		ArrayOfObjects objects = new ArrayOfObjects();
		objects.allSing(theBeatles);
	}

	public void allSing(PopStar[] stars) {
		// Loop through the array and call each PopStar's sing() method.
		for (PopStar currentSingingPopstar : stars) {
			currentSingingPopstar.sing();
		}
		for (int i = 0; i < stars.length; i++) {
			stars[i].sing();
		}
	}
}
```

`AdvancedArrays/com.skilldistillery.advancedarrays.drills.ReturningArrays`
```java
public class PopStar {
	public String name;

	public void sing() {
		// Have the PopStar print their name to the screen, as part of some kind of
		// lyric.
		// Be creative.
		System.out.print("My name is " + name);
		int numVowels = name.length();
		System.out.print(", h");
		for (int i = 0; i < numVowels; i++) {
			System.out.print("o");
		}
		System.out.println("!!");
	}
}
```

`ReturningArrays.java`
```java
public class ReturningArrays {
	public static void main(String[] args) {
//		Non-Static Method Call
//		createBand();

		ReturningArrays ra = new ReturningArrays();
		ra.createBand();
		PopStar[] output = ra.createBand();
		
		//Print out each name
		for (int i = 0; i < output.length; i++) {
			System.out.println(output[i].name); // Justin Lance...
		}

		// for each loop
//		for (PopStar popStar : output) {
//		    System.out.println(popStar.name);
//		}
		
		ra.allSing(output); //My name is Justin, hoooooo!! My name is Lance, hooooo!!...		

	}

	public PopStar[] createBand() {
		// Move the code that creates and fills a PopStar array into this method.
		// Be sure to return the array from the method
		// (since it's return type is PopStar[]).

		// Instantiate an Array to hold PopStar objects
		PopStar[] sync = new PopStar[5];

		// Create PopStar instances and add them to the array
		PopStar jt = new PopStar();
		sync[0] = jt;
		jt.name = "Justin";

		PopStar l = new PopStar();
		l.name = "Lance";
		sync[1] = l;

		PopStar jc = new PopStar();
		sync[2] = jc;
		jc.name = "JC";

		PopStar jf = new PopStar();
		jf.name = "Joey";
		sync[3] = jf;

		PopStar c = new PopStar();
		c.name = "Chris";
		sync[4] = c;
		return sync;
	}

	public void allSing(PopStar[] sync) {
		// Loop through the array and call each PopStar's sing() method
		for (int i = 0; i < sync.length; i++) {
			PopStar popStar = sync[i];
			popStar.sing();
		}
	}
}
```

`AdvancedArrays/com.skilldistillery.advancedarrays.drills.MultiDeclare`
```java
public class MultiDeclare {
	public static void main(String[] args) {
		// Declare a two-dimensional array of char values to represent a
		// tic-tac-toe board.
		char[][] board = new char[3][3];

		board[0][0] = 'X';
		board[0][1] = 'O';
		board[0][2] = 'X';
		board[1][0] = 'O';
		board[1][1] = 'X';
		board[1][2] = 'O';
		board[2][0] = 'X';
		board[2][1] = 'O';
		board[2][2] = 'X';

		for (int row = 0; row < 3; row++) {
			for (int col = 0; col < 3; col++) {
				System.out.print(board[row][col] + " ");
			}
			System.out.println();
		}
	}
}
```

`AdvancedArrays/com.skilldistillery.advancedarrays.drills.MultiDeclare`
```java
public class MultiDeclare {
	public static void main(String[] args) {
		// Declare a two-dimensional array of char values to represent a
		// tic-tac-toe board.
		char[][] board = new char[3][3];

		board[0][0] = 'X';
		board[0][1] = 'O';
		board[0][2] = 'O';
		board[1][0] = 'O';
		board[1][1] = 'X';
		board[1][2] = 'O';
		board[2][0] = 'O';
		board[2][1] = 'O';
		board[2][2] = 'X';

		for (int row = 0; row < 3; row++) {
			for (int col = 0; col < 3; col++) {
				System.out.print(board[row][col] + " ");
			}
			System.out.println();
		}
	}
}
```

`AdvancedArrays/com.skilldistillery.advancedarrays.drills.MultiDeclare`
```java
public class MultiDeclare {
	public static void main(String[] args) {
		// Declare a two-dimensional array of char values to represent a
		// tic-tac-toe board.
		char[][] board = new char[3][3];

		board[0][0] = 'X';
		board[0][1] = 'X';
		board[0][2] = 'X';
		board[1][0] = 'X';
		board[1][1] = 'X';
		board[1][2] = 'O';
		board[2][0] = 'X';
		board[2][1] = 'O';
		board[2][2] = 'O';

		for (int row = 0; row < 3; row++) {
			for (int col = 0; col < 3; col++) {
				System.out.print(board[row][col] + " ");
			}
			System.out.println();
		}
	}
}
```

`AdvancedArrays/com.skilldistillery.advancedarrays.drills.VarArgsBand`
```java
public class VarArgsBand {

  public static void main(String[] args) {
    
    // Run the program, passing a band name and list of members. 
    // Is the output what you expected?
    bandMembers("The Copyrightles", "George", "Paul", "Ringo", "John");
    
    // Can you call the method with zero parameters? Why or why not?
    // No. The first parameter is a String, so there must always be at least
    // one String. There can be zero or more members.
    int numMembers = bandMembers("Nobody"); // Passing zero members after the bandName
    System.out.println("The number of members in Nobody is " + numMembers);
  }
  
  public static int bandMembers(String bandName, String... members) {
    int numMembers = members.length;
    System.out.println("Members of " + bandName);
    for (String m : members) {
      System.out.println("\t" + m);
    }
    return numMembers;
  }

}
```

`Lab 1 - SBScores.java`
```java
public class SBScores {
	public static void main(String[] args) {
		int[][] superBowlScores = { { 35, 10 }, { 33, 14 }, { 16, 7 }, { 23, 7 }, { 16, 13 }, { 24, 3 }, { 14, 7 },
				{ 24, 7 }, { 16, 6 }, { 21, 17 } };
		String[][] superBowlTeams = { { "Green Bay", "Kansas City" }, { "Green Bay", "Oakland" },
				{ "NY Jets", "Baltimore" }, { "Kansas City", "Minnesota" }, { "Baltimore", "Dallas" },
				{ "Dallas", "Miami" }, { "Miami", "Washington" }, { "Miami", "Minnesota" },
				{ "Pittsburgh", "Minnesota" }, { "Pittsburgh", "Dallas" } };
		for (int i = 0; i < superBowlScores.length; i++) {
			int[] scores = superBowlScores[i];
			String[] teams = superBowlTeams[i];
			printScore(teams, scores);
		}
	}

	public static void printScore(String[] teams, int[] scores) {
		System.out.println(teams[0] + " " + scores[0] + " - " + teams[1] + " " + scores[1]);
	}
}
```

#### Project: Tic Tac Toe

## [Week 2](https://github.com/SkillDistillery/SD41/blob/main/java1/README.md)

### Week 2 - Day 1

#### Packages
1. Namespaces
2. Introduction to Java Packages
3. Creating Packages
4. Package Names
5. Imports
6. Static Imports
7. Labs

```java
package com.skilldistillery.directorypath; //To minimize the chance of package name collisions.
```

```java
import com.skilldistillery.utilities.parsing.Parser; //To be able to use Parser.
import com.skilldistillery.utilities.parsing.*; //To be able to use all objects, does not use memory.

//main method
Parser parser = new Parser();
parser.parse();
```

`Lab 1 - ProductMain`
```java
package com.skilldistillery.packages.labs;

public class ProductMainStatics {

  Product product;

  public static void main(String[] args) {
    ProductMainStatics app = new ProductMainStatics();
    app.go();
  }

  public ProductMainStatics() {
    product = new Product();
  }

  public void go() {
    utilMethod();
    helperMethod();
  }
}
```

#### String and StringBuilder
1. The String Class
2. The String Pool
3. String Methods
4. The StringBuilder Class
5. StringBuilder Methods
6. Writing toString() Methods
7. Labs

`StringAndStringBuilder/com.skilldistillery.stringstringbuilder.drills.StringPoolTesting`
```java
class OtherClass {
	public static String coding = "AlwaysCoding";
}

public class StringPoolTesting {
	private String coding = "Always" + "Coding";

	public static void main(String[] args) {
		StringPoolTesting tester = new StringPoolTesting();
		tester.test();
	}

	private void test() {
		String coding = "AlwaysCoding";
		String coding2 = new String("AlwaysCoding");
		String always = "Always";

//     true or false: false
		System.out.println(coding == coding2);
//     true or false: true
		System.out.println(coding == this.coding);
//     true or false: true
		System.out.println(coding == OtherClass.coding);
//     true or false: true
		System.out.println(coding == "AlwaysCoding");
//     true or false: true
		System.out.println(coding == "Always" + "Coding");
//     true or false: flase
		System.out.println(coding == always + "Coding");
//     true or false: true
		System.out.println(coding == "Al" + "waysCoding");
//     true or false:true
		System.out.println(coding == (always + "Coding").intern());
	}
}
```

`StringAndStringBuilder/src/com.skilldistillery.stringstringbuilder.drills.SSNMasker`
```java
public class SSNMasker {

	/**
	 * Returns an SSN (Social Security Number) string with the first five digits
	 * replaced with 'X'.
	 * 
	 * @param ssn An SSN sting in the format 123-45-6789
	 * @return A masked SSN string in the format XXX-XX-6789
	 */
	public String maskSSN(String ssn) {
		String maskedSSN = null;

		// CODE HERE
		// use substring and concatenation to return a masked SSN.
		String lastFour = ssn.substring(7, 11);
		maskedSSN = "XXX-XX-" + lastFour;
		return maskedSSN;
	}
}
```

`StringAndStringBuilder/test/com.skilldistillery.stringstringbuilder.drills.SSNMaskerTests`
```java
public class SSNMaskerTests {
  SSNMasker masker;

	@Before
	public void setUp() throws Exception {
		masker = new SSNMasker();
	}

	@After
	public void tearDown() throws Exception {
		masker = null;
	}

	@Test
	public void test_maskSSN_returns_ssn_with_first_five_digits_masked_with_X() {
		String ssn = "123-45-6789";
		String masked = masker.maskSSN(ssn);
		String expected = "XXX-XX-6789";
		assertEquals(expected, masked);
		ssn = "666-55-4321";
		masked = masker.maskSSN(ssn);
		expected = "XXX-XX-4321";
	}

}
```

`StringAndStringBuilder/com.skilldistillery.stringstringbuilder.drills.UserCommentDriver`
```java
public class UserCommentDriver {

	public static void main(String[] args) {
		UserCommentDriver driver = new UserCommentDriver();
		driver.go();
	}

	private void go() {
		UserComment comment1 = new UserComment(42, null, "2018-01-04", "14:59:23", "bdobbs", "I love coding in Java!");

		UserComment comment2 = new UserComment(47, comment1, "2018-01-04", "15:03:12", "jsmith", "Me too!");

		System.out.println(comment1);
		System.out.println(comment2);

	}
}
```
```java
//UserComment.java

@Override
	public String toString() {
		return "UserComment [commentId=" + commentId + ", inReplyToComment=" + inReplyToComment + ", date=" + date
				+ ", time=" + time + ", userName=" + userName + ", commentText=" + commentText + "]";
	}
```

`Lab 1 - StringLab.java`
```java
public class StringLab {

	public static void main(String[] args) {
		StringLab lab = new StringLab();
		lab.go();
	}

	private void go() {
		// Using String methods, determine and print whether 'testString':
		// 1. Starts with 'abc'
		// 2. Ends with 'ld!'
		// 3. Contains 'wor'
		String testString = "Hello world!";

		System.out.println(testString.startsWith("abc"));
		System.out.println(testString.endsWith("ld!"));
		System.out.println(testString.contains("wor"));

		// Using String methods, print the following information
		// about 'testString2':
		// 1. The character at index 3
		// 2. The number of characters in the String
		// 3. The contents of the String in all uppercase
		// 4. The contents of the String without white space on either side

		String testString2 = "   Hello Java Coding World!   ";

		System.out.println(testString2.charAt(3));
		System.out.println(testString2.length());
		System.out.println(testString2.toUpperCase());
		System.out.println(testString2.trim());
	}
}
```

`Lab 2 - StringBuilderLab.java`
```java
public class StringBuilderLab {

	public static void main(String[] args) {
		StringBuilderLab lab = new StringBuilderLab();
		lab.go();
	}

	private void go() {
		String original = "Java world.";

		StringBuilder sb = new StringBuilder(original);
		System.out.println(sb);

		// Use only StringBuilder methods on sb to change the text to:
		// Hello, Java coding world! Always Be Coding!
		// Print out sb after each step.

		sb.setCharAt(sb.length() - 1, '!');
		System.out.println(sb);

		sb.insert(5, "coding ");
		System.out.println(sb);

		sb.insert(0, "Hello, ");
		System.out.println(sb);

		sb.append(" Always Be Coding!");
		System.out.println(sb);

		String result = sb.toString();
		System.out.println(result);
	}
}
```

`Lab 3 - UserComment.java`
```java
@Override
  public String toString() {
    String result = "On " + date + " at " + time + ", " + userName + " posted this comment: ["
                    + commentText + "]";
    return result;
  }
```

`Lab 4 - UserComment2.java`
```java
@Override
  public String toString() {
    StringBuilder sb = new StringBuilder("On ");
    sb.append(date)
      .append(" at ")
      .append(time)
      .append(", ")
      .append(userName)
      .append(" posted this comment: [")
      .append(commentText)
      .append("]");
    return sb.toString();
  }
```

`Lab 5 - UserComment3.java`
```java
@Override
  public String toString() {
    StringBuilder builder = new StringBuilder();
    builder.append("UserComment3 [commentId=").append(commentId).append(", ");
    if (inReplyToComment != null)
      builder.append("inReplyToComment=").append(inReplyToComment).append(", ");
    if (date != null)
      builder.append("date=").append(date).append(", ");
    if (time != null)
      builder.append("time=").append(time).append(", ");
    if (userName != null)
      builder.append("userName=").append(userName).append(", ");
    if (commentText != null)
      builder.append("commentText=").append(commentText);
    builder.append("]");
    return builder.toString();
  }
```

#### Project: Mad Libs

### Week 2 - Day 2

#### ASCII and Unicode Data
1. Standards
2. ASCII
3. Unicode
4. Labs

`ASCIIData/com.skilldistillery.characters.drills.ASCIICharacters`
```java
public class ASCIICharacters {

	public static void main(String[] args) {
		// In a for loop, iterate through the number 0 to 127,
		// printing each number and the char representation
		// of that number (by casting it to a char) on a separate line.
		for (int i = 0; i < 128; i++) {
			char ASCIIi = (char) i;
			System.out.println("Numeral Value:" + i + " ASCII Value:" + ASCIIi);
		}
	}
}
```

`ASCIIData/com.skilldistillery.characters.drills.UnicodeOutput`
```java
public class UnicodeOutput {

	public static void main(String[] args) {
		// Write the characters
		// '\u261d', '\u270a', '\u270b', '\u270c'
		// to the screen.
		System.out.println('\u261d' + "" + '\u270a' + "" + '\u270b' + "" + '\u270c');
	}
}
```

`ASCIIData/com.skilldistillery.characters.drills.SuppChars`
```java
public class SuppChars {

	public static void main(String[] args) {
		// Write the String "\uD83C\uDCA1" to the screen.
		System.out.println("\uD83C\uDCA1");

		// Add the statement System.out.println(Character.toChars(0x1f0a1));
		System.out.println(Character.toChars(0x1f0a1));

		// Use Character.toChars() to output the code points 0x1F600 through 0x1F64F
		// Add a newline every 16 characters.
		int counter = 0;
		for (int i = 0x1F600; i <= 0x1F64F; i++) {
			System.out.print(Character.toChars(i));
			counter++;
			if (counter % 16 == 0) {
				System.out.println();
				counter = 0;
			}
		}
	}
}
```

`Lab 1 - AlphaNumCheck.java`
```java
public class AlphaNumCheck {

	public static void main(String[] args) {
		run();
	}

	public static void run() {
		Scanner sc = new Scanner(System.in);

		// Make an instance of this class
		AlphaNumCheck anc = new AlphaNumCheck();

		System.out.print("Enter a word or sentence: ");
		String input = anc.getSentence(sc);

		boolean result = anc.checkAlphaSentence(input);

		if (result) {
			System.out.println("The sentence contains only letters.");
		} else {
			System.out.println("The sentence contains non-letters.");
		}
		sc.close();
	}

	public String getSentence(Scanner sc) {
		return sc.nextLine();
	}

	public boolean checkAlphaSentence(String input) {
		char[] chars = input.toCharArray();
		boolean result = true;
		for (int i = 0; i < chars.length; i++) {
			char c = chars[i];
			if (c >= 65 && c <= 90 || c >= 'a' && c <= 'z') {
				continue;
			}
			result = false;
			break;
		}
		return result;
	}
}
```

`Lab 2 - AlphaNumCheck.java`
```java
public boolean checkAlphaNumSpaceSentence(String input) {
    char[] chars = input.toCharArray();
    boolean result = true;
    for (int i = 0; i < chars.length; i++) {
      char c = chars[i];
      if(c >= 65 && c <= 90 
          || c >= 'a' && c <= 'z'
          || c == 32
          || c >= '0' && c <= '9') {
        continue;
      }
      result = false;
      break;
    }
    
    return result;
  }
```

#### Objects and Classes
1. Classes and Objects
2. Constructors
3. The Default Constructor
4. Objects in Memory
5. Imagining the Heap
6. Visibility

`Objects/com.skilldistillery.objs.drills.Dog`
```java
public class Dog {
	public String breed;
	public String name;
	public int weight;

	// Add a constructor with parameters to initialize breed and weight.
	public Dog(String breedDog, int weightDog) {
		breed = breedDog;
		weight = weightDog;
	}

	// Add a constructor with parameters to initialize name, breed, and weight.
	public Dog(String name, String someBreed, int howManyLbs) {
		this.name = name;
		breed = someBreed;
		weight = howManyLbs;
	}

	public void displayDogInfo() {
		System.out.println("Dog [breed=" + breed + ", name=" + name + ", weight=" + weight + "]");
	}

	public static void main(String[] args) {
		// Create three dog instances and call the displayDogInfo method on each Dog
		// object.
		Dog newDog = new Dog("Poodle", 30);
		newDog.displayDogInfo();

		Dog myDog = new Dog("Pit Mix", 60);
		myDog.displayDogInfo();

		Dog yourDog = new Dog("Lab", 100);
		yourDog.displayDogInfo();

		Dog fredsDog = new Dog("Spot", "mutt", 10);
		fredsDog.displayDogInfo();
	}
}
```

`Objects/com.skilldistillery.objs.drills.BankApp`
```java
public class BankApp {

	public static void main(String[] args) {
		BankApp b = new BankApp();
		b.run();
	}

	void run() {
		Account acc1 = new Account("ACC-10001", 305.32);
		Account acc2 = new Account("ACC-10002", 9053.23);

		printAccountData(acc1);
		printAccountData(acc2);
//    	acc1.setBalance(305.32 + 100);
	}

	void printAccountData(Account account) {
		System.out.println(account.getAccountId() + " balance: " + account.getBalance());
	}
}
//cmd + opt + s
//generate getters and setters
```

#### Drawing Objects and Their Relationships
1. Representing Objects with Diagrams
2. UML Class Diagram
3. Classes and Their Associations
4. Labs

#### Introduction to JUnit
1. Testing Java Applications
2. Building and Deploying Software
3. JUnit
4. Test Classes
5. Writing @Test Methods
6. assert Methods
7. @Before and @After
8. Test-Driven Development (TDD)
9. Labs

#### Project: Caesar Cipher

### Week 2 - Day 3

#### Encapsulation
1. Changing Instance Fields
2. Visibility and Access Modifiers
3. Encapsulation
4. Getters and Setters
5. The this Keyword
6. Labs

`Encapsulation/com.skilldistillery.encapsulation.drills.BankApp`
```java
public class BankApp {

  public static void main(String[] args) {
    BankApp b = new BankApp();
    b.run();
  }
  
  void run(){
    Account acc1 = new Account("ACC-10001", 305.32);
    Account acc2 = new Account("ACC-10002", 9053.23);
    
    printAccountData(acc1);
    printAccountData(acc2); 
  }
  
  void printAccountData(Account account) {
    System.out.println(account.accountId + " balance: " + account.balance); //Can't access private data (accountId, balance)
  }
}
```

`Encapsulation/com.skilldistillery.encapsulation.drills.Account`
```java
	private double balance;
	private String accountId;

	public Account(String aId) {
		accountId = aId;
	}

	public Account(String aId, double initialBalance) {
		balance = initialBalance;
		accountId = aId;
	}

	public void deposit(double amount) {
		balance = balance + amount;
	}

	public void withdraw(double amount) {
		balance = balance - amount;
	}
}
```

`Encapsulation/com.skilldistillery.encapsulation.drills.BankApp`
```java
public class BankApp {

	public static void main(String[] args) {
		BankApp b = new BankApp();
		b.run();
	}

	void run() {
		Account acc1 = new Account("ACC-10001", 305.32);
		Account acc2 = new Account("ACC-10002", 9053.23);

		printAccountData(acc1);
		printAccountData(acc2);
	}

	void printAccountData(Account account) {
		System.out.println(account.getAccountId() + " balance: " + account.getBalance());
	}
}
```

`Encapsulation/com.skilldistillery.encapsulation.drills.Account`
```java
public class Account {
	  private double balance;
	  private String accountId;

	  public Account(String aId) {
	    accountId = aId;
	  }

	  public Account(String aId, double initialBalance) {
	    balance = initialBalance;
	    accountId = aId;
	  }
	  
	  // "getter" and "setter" methods
	  public double getBalance() {
	    return balance;
	  }

	  public void setBalance(double bal) {
	    balance = bal;
	  }

	  public String getAccountId() {
	    return accountId;
	  }

	  public void setAccountId(String id) {
	    accountId = id;
	  }

	  public void deposit(double amount) {
	    balance = balance + amount;
	  }

	  public void withdraw(double amount) {
	    balance = balance - amount;
	  }
	}
```

`Encapsulation/com.skilldistillery.encapsulation.drills.Student`
```java
public class Student {

	private int[] scores;
	private double average;

	public int[] getScores() {
		return scores;
	}

	public double getAverage() {
		return average;
	}

	private void computeAverage() {
		// valid code to compute average
		// average = update average value
		if (scores != null && scores.length > 0) {
			int sum = 0;
			for (int score : scores) {
				sum += score;
			}
			average = (double) sum / scores.length;
		} else {
			average = 0; // Handle the case when there are no scores.
		}
	}

	public Student() {
		computeAverage();
	}
}
```

`Encapsulation/com.skilldistillery.encapsulation.drills.Account`
```java
public class Account {
	private double balance;
	private String accountId;

	public Account(String aId) {
		accountId = aId;
	}

	public Account(String aId, double initialBalance) {
		balance = initialBalance;
		accountId = aId;
	}

	// "getter" and "setter" methods
	public double getBalance() {
		return balance;
	}

	public void setBalance(double bal) {
		this.balance = balance;
	}

	public String getAccountId() {
		return accountId;
	}

	public void setAccountId(String id) {
		this.accountId = accountId;
	}

	public void deposit(double amount) {
		balance = balance + amount;
	}

	public void withdraw(double amount) {
		balance = balance - amount;
	}
}
```

`Lab 1 - Car.java`
```java
public class Car {
	private String make;
	private String model;
	private String color;
	private int numberOfWheels;
	private double purchasePrice;


	public Car() {
		
	}

	public Car(String make1, String model1, String color1, int wheels, double price) {
		this.make = make1;
		this.model = model1;
		this.color = color1;
		this.numberOfWheels = wheels;
		this.purchasePrice = price;
	}

	public Car(String make1, String model1, String color1, int wheels) {
		this.make = make1;
		this.model = model1;
		this.color = color1;
		this.numberOfWheels = wheels;
	}

	public String getMake() {
		return make;
	}

	public void setMake(String make) {
		this.make = make;
	}

	public String getModel() {
		return model;
	}

	public void setModel(String model) {
		this.model = model;
	}

	public String getColor() {
		return color;
	}

	public void setColor(String color) {
		this.color = color;
	}

	public int getNumberOfWheels() {
		return numberOfWheels;
	}

	public void setNumberOfWheels(int numberOfWheels) {
		this.numberOfWheels = numberOfWheels;
	}

	public double getPurchasePrice() {
		return purchasePrice;
	}

	public void setPurchasePrice(double purchasePrice) {
		this.purchasePrice = purchasePrice;
	}

	public void displayCar() {
		String carData = toString();
		System.out.println(carData);
	}

	public String toString() {
		String output = "make= " + make + ", model= " + model + ", color= " + color + ", numberOfWheels= "
				+ numberOfWheels + ", purchasePrice= " + purchasePrice;
		return output;
	}
}
```

`Lab 1 - CarTester.java`
```java
public class CarTester {

	public static void main(String[] args) {
		// Create two Cars and assign fields
		Car car1 = new Car("Dodge", "Stratus", "Blue", 4, 15412);
		Car car2 = new Car("Ford", "F-950", "Neon", 10, 70000);
		Car car3 = new Car();

		// Have the cars display themselves
		car1.displayCar();
		car2.displayCar();
		car3.displayCar();

		String car1Data = car1.toString();
		String car2Data = car2.toString();
		String car3Data = car3.toString();

		// Get the cars' data and display that
		System.out.println("Car 1 data: " + car1Data);
		System.out.println("Car 2 data: " + car2Data);
		System.out.println("Car 3 data: " + car3Data);
	}
}
```

`Lab 2 - ParkingLot.java`
```java
public class ParkingLot {
	private int numCars;
	private Car[] cars;
	private int MAX_CARS = 10;

	public ParkingLot() {
		cars = new Car[MAX_CARS];
	}

	public void addCar(Car aCar) {
		if (numCars == MAX_CARS) {
			System.out.println("SOL! Good luck making your flight!");
		} else {
			for (int i = 0; i < cars.length; i++) {
				if (cars[i] == null) {
					cars[i] = aCar;
					numCars++;
					break;
				}
			}
		}
	}

	public Car[] getCars() {
		Car[] allParkedCars = new Car[numCars];
		for (int i = 0; i < cars.length; i++) {
			if (cars[i] != null) {
				allParkedCars[i] = cars[i];
			}
		}
		return allParkedCars;
	}
}
```

`Lab 2 - ParkingLotTester.java`
```java
public class ParkingLotTester {

	public static void main(String[] args) {
		ParkingLotTester crt = new ParkingLotTester();
		crt.run();
	}

	private void run() {
		ParkingLot cr = new ParkingLot();

		Car[] cars = cr.getCars();

		System.out.println("Number of initial cars: " + cars.length);

		Car car1 = new Car("Black", "Dodge", "Stratus", 4, 15412.0);

		Car car2 = new Car();
		car2.setColor("Neon");
		car2.setMake("Ford");
		car2.setModel("F950");
		car2.setNumberOfWheels(10);
		car2.setPurchasePrice(74999.0);

		cr.addCar(car1);
		cr.addCar(car2);

		// Get the car array
		cars = cr.getCars();

		// Print it
		printCars(cars);

		System.out.println("Total cars returned: " + cars.length);
	}

	private void printCars(Car[] cars) {
		for (Car car : cars) {
			car.displayCar();
		}
	}
}
```

#### Object Initialization
1. this vs. this()
2. Initializing Static Fields
3. Initializing Instance Fields
4. Order of Initialization
5. Constant Fields and Variables
6. private Methods
7. Labs

#### Inheritance in Java
1. Inheritance
2. The extends Keyword
3. final Classes *
4. UML and extends
5. Inheriting Fields *
6. Inheriting Methods *
7. Lab - Creating a Class Hierarchy

`Inheritance/com.skilldistillery.inheritance.drills.Employee`
```java
public class Employee extends Person {

	private String title;
	private double Salary;
}
```

`Inheritance/com.skilldistillery.inheritance.drills`
```java
public class TestClass extends Object{

}
//Try to make TestClass extend System by adding extends System.
//Try to make TestClass extend String.
//Try to make TestClass extend StringBuilder.
//Try to make TestClass extend Integer.
//It didn't work. Make TestClass extend Object.
```

`Inheritance/com.skilldistillery.inheritance.drills.Employee`
```java
public class Employee extends Person {

	private String title;
	private double Salary;

	// Add a no-arg constructor to Employee.
	public Employee() {
	
	}

	// Add a constructor to Employee with parameters for firstName, lastName, age,
	// title, and salary.
	// Set the fields firstName, lastName, and age the same way as title and salary
	// - using the . operator.
	public Employee(String firstName, String lastName, int age, String title, double Salary) {
		this.firstName = firstName;
		this.lastName = lastName;
		this.age = age;
		this.title = title;
		this.Salary = Salary;
	}

	// Add a method to Employee called public String getInfo()
	// Return a String containing the object's information in the format firstName
	// lastName age title salary.
	public String getInfo() {
		return firstName + " " + lastName + " " + age + " " + title + " " + salary;
	}
}
```

`Inheritance/com.skilldistillery.inheritance.drills.EmployeeApp`
```java
public class EmployeeApp {

	public static void main(String[] args) {
		EmployeeApp app = new EmployeeApp();
		app.run();
	}

	private void run() {
		Person pers = null;
		// Create a Person object and assign it to pers. Give the person a firstName,
		// lastName, and age using either the constructor or setters.
		pers = new Person();
		pers.setFirstName("Anthony");
		pers.setLastName("King");
		pers.setAge(31);

		// Call getInfo() and print the Person's information to the screen.
		System.out.println(pers.getInfo());

		Employee emp2 = null;

		// Create an Employee object using the five-argument constructor, and
		// assign it to emp2.
		emp2 = new Employee("Dee", "G", 25, "Instructor", 100); // creating new object using ctor from Employee class

		// Call getInfo() and print the Employee's information to the screen.
		System.out.println(emp2.getInfo());
	}
}
```

`Inheritance/com.skilldistillery.inheritance.drills.Employee`
```java
public String getInfo() {
		return getName() + " " + age + " " + title + " " + Salary;
	}
```

`Lab 1 - Vehicle.java`
```java
public class Vehicle {

	protected double purchasePrice;

	public Vehicle() {
	}

	public Vehicle(double purchasePrice) {
		this.purchasePrice = purchasePrice;
	}

	public double getPurchasePrice() {
		return purchasePrice;
	}

	public void setPurchasePrice(double purchasePrice) {
		this.purchasePrice = purchasePrice;
	}

	@Override
	public String toString() {
		return "Vehicle [purchasePrice=" + purchasePrice + "]";
	}
}
```

`Lab 2 - Automobile.java`
```java
public class Automobile extends Vehicle {

	private String make;
	private String model;
	private int year;
	private int numberOfWheels;
	private double speedInMph;

	public Automobile() {
	}

	public Automobile(String make, String model, int year, int numberOfWheels, double speedInMph,
			double purchasePrice) {
		super(purchasePrice);
		this.make = make;
		this.model = model;
		this.year = year;
		this.numberOfWheels = numberOfWheels;
		this.speedInMph = speedInMph;
		this.purchasePrice = purchasePrice;
	}
	
	public String getMake() {
		return make;
	}

	public void setMake(String make) {
		this.make = make;
	}

	public String getModel() {
		return model;
	}

	public void setModel(String model) {
		this.model = model;
	}

	public int getYear() {
		return year;
	}

	public void setYear(int year) {
		this.year = year;
	}

	public int getNumberOfWheels() {
		return numberOfWheels;
	}

	public void setNumberOfWheels(int numberOfWheels) {
		this.numberOfWheels = numberOfWheels;
	}

	public double getSpeedInMph() {
		return speedInMph;
	}

	public void setSpeedInMph(double speedInMph) {
		this.speedInMph = speedInMph;
	}

	@Override
	public String toString() {
		return "Automobile [make=" + make + ", model=" + model + ", year=" + year + ", numberOfWheels=" + numberOfWheels
				+ ", speedInMph=" + speedInMph + ", purchasePrice=" + purchasePrice + "]";
	}
}
```

`Lab 3 - Boat.java`
```java
public class Boat extends Vehicle {

	protected String name;
	protected double speedInKnots;
	protected int lengthInFeet;

	public Boat() {

	}

	public Boat(String name, double speedInKnots, int lengthInFeet, double purchasePrice) {
		this.name = name;
		this.speedInKnots = speedInKnots;
		this.lengthInFeet = lengthInFeet;
		this.purchasePrice = purchasePrice;
	}

	@Override
	public String toString() {
		return "Boat [name=" + name + ", speedInKnots=" + speedInKnots + ", lengthInFeet=" + lengthInFeet
				+ ", purchasePrice=" + purchasePrice + "]";
	}
}
```

`Lab 4 - Truck.java`
```java
public class Truck extends Automobile {
	protected int bedSizeInCubicFeet;

	public Truck() {

	}

	public Truck(double purchasePrice, String make, String model, int year, int numberOfWheels, double speedInMph,
			int bedSizeInCubicFeet) {
		this.purchasePrice = purchasePrice; // Vehicle field
		this.make = make; // Automobile fields
		this.model = model;
		this.year = year;
		this.numberOfWheels = numberOfWheels;
		this.speedInMph = speedInMph;
		this.bedSizeInCubicFeet = bedSizeInCubicFeet;
	}
}
```

`Lab 5 - VehicleTestApp.java`
```java
public class VehicleTestApp {

	public static void main(String[] args) {
		Automobile sc = new Automobile();
		System.out.println(sc.toString());

		Boat bobber = new Boat();
		System.out.println(bobber.toString());

		Truck coalRoller = new Truck();
		System.out.println(coalRoller.toString());

	}
}
```

#### Visibility
1. Field and Method Visibility
2. Getters and Setters
3. Lab - Improving Encapsulation

#### Project: Food Trucks

### Week 2 - Day 4

#### Superclasses
1. Using a Superclass's Methods and Fields
2. Constructors and Inheritance
3. Rules for super()
4. The Object Class
5. Labs

`SuperClasses/com.skilldistillery.inheritance.drills.Employee`
```java
public class Employee extends Person {
  private String title;
  private double salary;

  public Employee() {
  }

  public Employee(String firstName, String lastName, int age,
      String title, double salary) {
    this.firstName = firstName;
    this.lastName = lastName;
    this.age = age;
    this.title = title;
    this.salary = salary;
  }
  
  // Call the parent method
  public String getInfo() {
    return super.getInfo() + " " + title + " " + salary;
  }

  public String getTitle() {
    return title;
  }

  public void setTitle(String title) {
    this.title = title;
}

public double getSalary() {
	return salary;
}

public void setSalary(double salary) {
	this.salary = salary;
}
}
```

`SuperClasses/com.skilldistillery.inheritance.drills.DataAnalyst`
```java
import com.skilldistillery.superclasses.drills.Employee;

public class DataAnalyst extends Employee {
  private String securityClearance;
  
  public DataAnalyst(String securityClearance, String firstName, String lastName, int age, String title, double salary) {
    this.setSecurityClearance(securityClearance);
    this.setFirstName(firstName);
    this.setLastName(lastName);
    this.setAge(age);
	this.setTitle(title);
	this.setSalary(salary);
}

public String getSecurityClearance() {
	return securityClearance;
}

public void setSecurityClearance(String securityClearance) {
	this.securityClearance = securityClearance;
}

// Call the parent method
public String getInfo() {
	return super.getInfo() + " " + securityClearance;
}
}
```

`SuperClasses/com.skilldistillery.inheritance.drills.EmployeeApp`
```java
import com.skilldistillery.superclasses.drills.Person;

public class EmployeeApp {

	public static void main(String[] args) {
		EmployeeApp app = new EmployeeApp();
		app.run();
	}

	private void run() {
		Person pers = null;
		pers = new Person("Ronnie", "Dobbs", 34);
		System.out.println(pers.getInfo());

		Employee6 emp = null;
		emp = new Employee6("Bob", "Dobbs", 55, "VP of Sales", 138_000.00);
		System.out.println(emp.getInfo());

		DataAnalyst dataAnalyst = new DataAnalyst("TOP SECRET", "James", "Java", 45, "Analyst IV", 120_000.00);
		System.out.println(dataAnalyst.getInfo());
	}
}
```

`Lab 1 - Vehicle.java`
```java
public class Vehicle {

	private double purchasePrice;

	public Vehicle(double purchasePrice) {
		this.purchasePrice = purchasePrice;
	}

	public double getPurchasePrice() {
		return purchasePrice;
	}

	public void setPurchasePrice(double purchasePrice) {
		this.purchasePrice = purchasePrice;
	}

	public String toString() {
		return "Vehicle [purchasePrice=" + purchasePrice + "]";
	}
}
```

`Lab 1 - Automobile.java`
```java
import com.skilldistillery.superclasses.labs.vehicles.Vehicle;

public class Automobile extends Vehicle {
	private String make;
	private String model;
	private int year;
	private int numberOfWheels;
	private double speedInMph;

	public Automobile(double purchasePrice, String make, String model, int year, int numberOfWheels,
			double speedInMph) {
		super(purchasePrice);
		this.make = make;
		this.model = model;
		this.year = year;
		this.numberOfWheels = numberOfWheels;
		this.speedInMph = speedInMph;
	}

	public String toString() {
		return "Automobile [purchasePrice=" + getPurchasePrice() + ", make=" + make + ", model=" + model + ", year="
				+ year + ", numberOfWheels=" + numberOfWheels + ", speedInMph=" + speedInMph + "]";
	}

	public String getMake() {
		return make;
	}

	public void setMake(String make) {
		this.make = make;
	}

	public String getModel() {
		return model;
	}

	public void setModel(String model) {
		this.model = model;
	}

	public int getYear() {
		return year;
	}

	public void setYear(int year) {
		this.year = year;
	}

	public int getNumberOfWheels() {
		return numberOfWheels;
	}

	public void setNumberOfWheels(int numberOfWheels) {
		this.numberOfWheels = numberOfWheels;
	}

	public double getSpeedInMph() {
		return speedInMph;
	}

	public void setSpeedInMph(double speedInMph) {
		this.speedInMph = speedInMph;
	}
}
```

`Lab 1 - Truck.java`
```java
import com.skilldistillery.superclasses.labs.vehicles.Automobile;

public class Truck extends Automobile {
	protected int bedSizeInCubicFeet;

	public Truck(double purchasePrice, String make, String model, int year, int numberOfWheels, double speedInMph,
			int bedSizeInCubicFeet) {
		super(purchasePrice, make, model, year, numberOfWheels, speedInMph);
		this.bedSizeInCubicFeet = bedSizeInCubicFeet;
	}

	public int getBedSizeInCubicFeet() {
		return bedSizeInCubicFeet;
	}

	public void setBedSizeInCubicFeet(int bedSizeInCubicFeet) {
		this.bedSizeInCubicFeet = bedSizeInCubicFeet;
	}
}
```

`Lab 1 - Boat.java`
```java
import com.skilldistillery.superclasses.labs.vehicles.Vehicle;

public class Boat extends Vehicle {
	protected String name;
	protected double speedInKnots;
	protected int lengthInFeet;

	public Boat(double purchasePrice, String name, double speedInKnots, int lengthInFeet) {
		super(purchasePrice);
		this.name = name;
		this.speedInKnots = speedInKnots;
		this.lengthInFeet = lengthInFeet;
	}

	public String toString() {
		return "Boat [purchasePrice=" + getPurchasePrice() + ", name=" + name + ", speedInKnots=" + speedInKnots
				+ ", lengthInFeet=" + lengthInFeet + "]";
	}
}
```

`Lab 1 - VehicleTestApp`
```java
public class VehicleTestApp {

	public static void main(String[] args) {
		Automobile a = new Automobile3(90000.00, "Dundreary", "Stretch", 2008, 4, 105);
		Boat b = new Boat3(145000.00, "Reefer", 21, 25);
		Truck t = new Truck3(22_000, "Vapid", "Bobcat", 2006, 4, 88, 55);

		System.out.println(a.toString());
		System.out.println(b.toString());
		System.out.println(t.toString());
	}
}
```

#### Polymorphism and Overriding
1. Polymorphism in Java
2. Overriding Superclass Behavior
3. @Override
4. Rules for Overriding
5. Lab - Using Polymorphism

#### Abstract Classes
1. Abstract Classes
2. Abstract Methods
3. Using Abstract Classes
4. Labs

#### Polymorphism and Casting
1. Casting
2. Downcasting
3. Casting and Precedence
4. Hiding Instance Fields
5. Labs

#### Project: Animal Sanctuary

### Week 2 - Day 5

#### Equals and Hashcode
1. Comparing References
2. Object.equals()
3. Defining an equals() Method
4. Determining Equality
5. hashCode()
6. Labs

#### The Primitive-Type Wrapper Classes
1. Wrapper Classes
2. Important Wrapper Class Methods
3. Comparing Wrapper Objects
4. Autoboxing
5. Float and Double
6. Integer-type Wrappers
7. Character
8. Boolean
9. Labs

`WrapperClasses/com.skilldistillery.wrapperclasses.drills.ParseDrill`
```java
public class ParseDrill {

	public static void main(String[] args) {
		ParseDrill drill = new ParseDrill();
		drill.go();
	}

	private void go() {
		// Write statements to determine which strings can be parsed,
		// and if so print the result, when parsed to:

		// Example:
		System.out.println(Integer.parseInt("42")); // No problem, 42

		// int:
		// "1000000000"
		System.out.println(Integer.parseInt("1000000000")); // No problem, 1000000000
		// "-1000000000"
		System.out.println(Integer.parseInt("-1000000000")); // No problem, -1000000000
		// "+1000000000"
		System.out.println(Integer.parseInt("+1000000000")); // No problem, 1000000000
		// " 1000000000 "
//    System.out.println(Integer.parseInt("  1000000000   ")); // NumberFormatException
		// "0x123abc"
//    System.out.println(Integer.parseInt("0x123abc")); // NumberFormatException
		// Note that a hexadecimal (or other base integer) can be parsed by passing
		// a radix to the overloaded Integer.parseInt; omit the "0x" prefix.
		System.out.println(Integer.parseInt("123abc", 16)); // NumberFormatException
		// "1.0"
//    System.out.println(Integer.parseInt("1.0")); // NumberFormatException
		// "1,000,000,000"
//  System.out.println(Integer.parseInt("1,000,000,000")); // NumberFormatException
		// "1_000_000_000"
//  System.out.println(Integer.parseInt("1_000_000_000")); // NumberFormatException
		// "10000000000"
//  System.out.println(Integer.parseInt("10000000000")); // NumberFormatException
		// ""
//  System.out.println(Integer.parseInt("")); // NumberFormatException
		// null
//  System.out.println(Integer.parseInt(null)); // NumberFormatException

		// long:
		// "1000000000"
		System.out.println(Long.parseLong("1000000000")); // No problem, 1000000000
		// "10000000000"
		System.out.println(Long.parseLong("10000000000")); // No problem, 10000000000
		// "10000000000L"
		// 'l' or 'L' as a type indicator are not permitted here, unlike a literal
//    System.out.println(Long.parseLong("10000000000L")); // NumberFormatException

		// float:
		// "10000000000"
		System.out.println(Float.parseFloat("10000000000")); // No problem, 1.0E10
		// "10000000000F"
		System.out.println(Float.parseFloat("10000000000F")); // No problem, 1.0E10
		// "314e-2"
		System.out.println(Float.parseFloat("314e-2")); // No problem, 3.14
		// "3.14D"
		System.out.println(Float.parseFloat("3.14D")); // No problem, 3.14
		// " 3.14 \n"
		System.out.println(Float.parseFloat("  3.14   \n")); // No problem, 3.14
		// null
//    System.out.println(Float.parseFloat(null)); // NullPointerException

		// boolean:
		// "true"
		System.out.println(Boolean.parseBoolean("true")); // No problem, true
		// "TrUe"
		System.out.println(Boolean.parseBoolean("TrUe")); // No problem, true
		// "false"
		System.out.println(Boolean.parseBoolean("false")); // No problem, false
		// "no"
		System.out.println(Boolean.parseBoolean("no")); // No problem, false
		// "giraffe"
		System.out.println(Boolean.parseBoolean("giraffe")); // No problem, false
		// null
		System.out.println(Boolean.parseBoolean(null)); // No problem, false

	}
}
```

`Lab 1 - NaNTest.java`
```java
public class NaNTest {

	public static void main(String[] args) {
		double f = 0.0 / 0.0;
		System.out.println(f);
		Double fObj = 0.0 / 0.0;
		System.out.println(fObj);
	}
}
```

`Lab 2a - AutoboxOverloada.java`
```java
public class AutoboxOverloada {
  public static void method(Object o) { System.out.println("In Object method"); }
  // a.: The method call compiles even though no method takes int.
  //     The int value is autoboxed to Integer, which is a subclass of Number.
  public static void method(Number n) { System.out.println("In Number method"); }
  //     Java will NOT both widen the int to long, then autobox to Long.
  public static void method(Long l)   { System.out.println("In Long method"); }

  public static void main(String[] args) {
    int var = 17;
    method(var);
  }
}
```

`Lab 2b - AutoboxOverload.java`
```java
public class AutoboxOverloadb {
  public static void method(Object o) { System.out.println("In Object method"); }
  public static void method(Number n) { System.out.println("In Number method"); }
  public static void method(Long l)   { System.out.println("In Long method"); }
  // b.: Java chooses the method taking long, preferring to widen the int to long
  //     rather than autoboxing to an Integer object.
  public static void method(long l)   { System.out.println("In long method"); }

  public static void main(String[] args) {
    int var = 17;
    method(var);
  }
}
```

`Lab 2c - AutoboxOverload.java`
```java
public class AutoboxOverloadc {
  public static void method(Object o) { System.out.println("In Object method"); }
  public static void method(Number n) { System.out.println("In Number method"); }
  public static void method(Long l)   { System.out.println("In Long method"); }
  public static void method(long l)   { System.out.println("In long method"); }
  // c.: Even with a method that takes Integer available, Java still chooses
  //     to widen int to long instead of autoboxing.
  public static void method(Integer i){ System.out.println("In Integer method"); }

  public static void main(String[] args) {
    int var = 17;
    method(var);
  }
}
```

`Lab 2d - AutoboxOverload.java`
```java
public class AutoboxOverloadd {
  public static void method(Object o) { System.out.println("In Object method"); }
  public static void method(Number n) { System.out.println("In Number method"); }
  public static void method(Long l)   { System.out.println("In Long method"); }
  public static void method(long l)   { System.out.println("In long method"); }
  public static void method(Integer i){ System.out.println("In Integer method"); }
  // d.: Of course now Java will choose the method taking int.
  public static void method(int i)    { System.out.println("In int method"); }

  public static void main(String[] args) {
    int var = 17;
    method(var);
  }
}
```

`Lab 3 - CountUpOrDown.java`
```java
public class CountUpOrDown {

	public static void main(String[] args) {

		Scanner input = new Scanner(System.in);

		System.out.print("Please enter a whole number: ");
		int count = input.nextInt();
		System.out.print("Please enter true or false: ");
		boolean b = input.nextBoolean();

		if (b) {
			for (int i = 0; i <= count; i++) {
				System.out.println(i);
			}
		} else {
			for (int i = count; i >= 0; i--) {
				System.out.println(i);
			}
		}

		input.close();
	}
}
```

`Lab 4 - IntegerReferences.java`
```java
public class IntegerReferences {
	public static void main(String[] args) {
		Integer i = Integer.valueOf(1000);
		increment(i);
		// This prints 1000. The local variable i in main still refers
		// to the immutable Integer object created on line 5.
		System.out.println(i);

		// If we assign the Integer reference returned by increment()
		// to our local variable, it will print 1001.
		i = increment(i);
		System.out.println(i);

	}

	private static Integer increment(Integer i) {
		// This statement does not modify the contents of the passed Integer,
		// which is immutable. Instead, it unboxes the value to an in, increments,
		// then autoboxes the result as a new Integer.
		i++;
		return i;
	}
}
```

`Lab 5 - TestLetters.java`
```java
public class TestLetters {

	public static void main(String[] args) {
		Scanner input = new Scanner(System.in);
		System.out.print("Enter some text: ");
		String text = input.nextLine();
		input.close();
		TestLetters tester = new TestLetters();
		tester.test(text);
	}

	private void test(String text) {
		char[] chars = text.toCharArray();
		for (char c : chars) {
			System.out.print(c);
			if (Character.isUpperCase(c)) {
				System.out.print(" is uppercase.");
			} else if (Character.isLowerCase(c)) {
				System.out.print(" is lowercase.");
			} else if (Character.isDigit(c)) {
				System.out.print(" is a digit.");
			}
			System.out.println();
		}
	}
}
```

#### Interfaces
1. Interfaces
2. Declaring an Interface
3. Using Interfaces
4. Labs - Declaring and Using Interfaces

`Lab 1 - Drawable.java`
```java

```

`Lab 2 - Circle.java`
```java

```

`Lab 3 - Rectangle.java`
```java

```

`Lab 4 - DrawableTester.java `
```java

```

`Lab 5 - Text.java`
```java

```

#### Project: Lord of the Objects

## [Week 3](https://github.com/SkillDistillery/SD41/blob/main/java1/README.md)

### Java Libraries

### Week 3 - Day 1

#### Generics and ArrayList
1. Arrays Revisited
2. The ArrayList Class
3. Generic <Types>
4. ArrayList - Adding and Getting
5. Replacing, Inserting, and Removing
6. Array vs. ArrayList
7. ArrayList - Size vs. Capacity *
8. Labs

`GenericsAndArrayList/com.skilldistillery.generics.drills.ArrayListExample`
```java
import java.util.ArrayList;

public class ArrayListExample {

	public static void main(String[] args) {
		ArrayListExample ex = new ArrayListExample();
		ex.run();
	}

	private void run() {
		// Declare and instantiate an ArrayList to hold Strings.
		// Use the type argument <String> in the constructor call.
		ArrayList<String> strings = new ArrayList<String>();

		// Declare and instantiate an ArrayList to hold Double objects.
		// This time use the <> shortcut in the constructor call.
		ArrayList<Double> doubles = new ArrayList<>();

		// Try to declare an ArrayList to hold double primitives (not Double objects).
		// What happens?
		// ArrayList<double> dubs;

		// Now try declaring an ArrayList without type arguments.
		ArrayList noType = new ArrayList();

		// What is the warning Eclipse gives you?
		// "ArrayList is a raw type. References to generic type ArrayList<E> should be
		// parameterized"

		// What combinations of <> and <String> can you put on either side of the =, and
		// still have the code compile?
		ArrayList<String> list1 = new ArrayList();
		ArrayList list2 = new ArrayList<>();
	}
}
```

`GenericsAndArrayList/com.skilldistillery.generics.drills.Container`
```java
public class Container<E> {
	private E field;

	public void set(E obj) {
		this.field = obj;
	}

	public E get() {
		return field;
	}
}
```

`GenericsAndArrayList/com.skilldistillery.generics.drills.GenericContainer`
```java
import java.util.ArrayList;

import com.skilldistillery.generics.solutions.Container;

public class GenericContainer {

	public static void main(String[] args) {

		// Declare and instantiate a Container to hold a Character object.
		Container<Character> cont = new Container<>();

		// Call the object's set method and pass in 'A'.
		cont.set('A'); // autoboxing

		// get the Character from the object and pass it to printChar.
		printChar(cont.get());

		// Try to set an Integer or String into the object.
		// cont.set("a"); // String will not work
		// cont.set(new Integer(1)); // Integer will not work

		// Create an ArrayList to hold Integer objects.
		ArrayList<Integer> list = new ArrayList<Integer>();

		// Optional: can you create an ArrayList to hold Container<Character> objects?
		ArrayList<Container<Character>> contList = new ArrayList<>();
	}

	private static void printChar(Character c) {
		System.out.println("The character is " + c);
	}
}
```

`GenericsAndArrayList/com.skilldistillery.generics.drills.AddingAndGetting`
```java
import java.util.ArrayList;

public class AddingAndGetting {

	public static void main(String[] args) {
		AddingAndGetting ag = new AddingAndGetting();
		ag.run();
	}

	private void run() {
		ArrayList<String> strings = new ArrayList<>();

		// Output the list's size.
		System.out.println("Size is " + strings.size());

		// Add first names of several of your classmates.
		strings.add("Belinda");
		strings.add("Jane");
		strings.add("Charlotte");
		strings.add("Gina");

		// Output the list's size again.
		System.out.println("Size is now " + strings.size());

		// Use a for loop and get(index) to iterate through the list and print each name
		// in uppercase letters.
		for (int i = 0; i < strings.size(); i++) {
			String n = strings.get(i);
			System.out.println(n.toUpperCase());
		}

		outputLastItem(strings); // Stretch goal: Finish the method below.

	}

	private void outputLastItem(ArrayList<String> list) {
		// Finish this method to output the last item in the list in lowercase.
		String last = list.get(list.size() - 1);
		System.out.println(last.toLowerCase());
	}
```

`GenericsAndArrayList/com.skilldistillery.generics.drills.ChangingArrayList`
```java
import java.util.ArrayList;

public class ChangingArrayList {
	public static void main(String[] args) {
		ChangingArrayList cal = new ChangingArrayList();
		cal.run();
	}

	private void run() {
		ArrayList<String> namesList = new ArrayList<>();

		namesList.add("Alice");
		namesList.add("Queen of Hearts");
		namesList.add("Cheshire Cat");
		namesList.add("Mad Hatter");
		namesList.add("Tweedle Dee");
		namesList.add("Tweedle Dum");

		System.out.println("There are " + namesList.size() + " elements in the list.");
		System.out.println(namesList); // calls toString() for each element

		// Remove Queen of Hearts and store the String in a variable.
		String queen = namesList.remove(1);

		// Output the contents of namesList with System.out.println()
		System.out.println(namesList);

		// Output the size of namesList
		System.out.println("List size is " + namesList.size());

		// Insert Queen of Hearts between Tweedle Dee and Tweedle Dum
		namesList.add(4, queen);

		// Output the contents of namesList
		System.out.println(namesList);

		// Replace Mad Hatter with Dormouse
		namesList.set(2, "Dormouse");

		// Output the contents of namesList
		System.out.println(namesList);

		// Remove Cheshire Cat
		namesList.remove(1);

		System.out.println(namesList);

		printMessage(namesList);
	}

	// This method uses the contents of your ArrayList
	private void printMessage(ArrayList<String> list) {
		if (list.size() != 5) {
			return;
		}
		String output = "";
		int i = 0, index[] = { 0, 7, 4, 2, 7 };
		int delta[] = { 5, 0, 1, -1, 0 };
		for (String string : list) {
			output += (char) (string.charAt(index[i]) + delta[i++]);
		}
		for (int j = 0; j < list.size(); j++) {
			char c = '\u0000';
			switch (j) {
			case 0:
				c = (char) (list.get(j).charAt(0) + 24);
				break;
			case 1:
				c = list.get(j).charAt(4);
				break;
			case 2:
				c = (char) (list.get(j).charAt(1) - 2);
				break;
			case 3:
				c = (char) (list.get(j).charAt(1) - 3);
				break;
			case 4:
				c = (char) (list.get(j).charAt(12 - 5));
				break;
			}
			output += c;
		}
		i = 0;
		index = new int[] { 2, 7, 3, 11, 0 };
		delta = new int[] { -33, 0, -4, 3, -38 };
		for (String s : list) {
			output += (char) (s.charAt(index[i]) + delta[i++]);
		}
		System.out.println(output);
	}
}
```

`Lab 3 - Stack.java`
```java
import java.util.ArrayList;

/**
 * Note: this Stack implementation has an issue, in that we could add nulls, but
 * we also return null for an empty list. We will have to live with this.
 * 
 */
public class Stack<E> {
	private ArrayList<E> list = new ArrayList<>();

	public Stack() {

	}

	public E push(E item) {
		list.add(item);
		return item;
	}

	public E pop() {
		if (list.size() == 0) {
			return null;
		}
		return list.remove(list.size() - 1);
	}

	public E peek() {
		if (list.size() == 0) {
			return null;
		}
		return list.get(list.size() - 1);
	}

	public int search(Object o) {
		int index = -1;
		for (int i = 0; i < list.size(); i++) {
			E item = list.get(i);
			if (item.equals(o)) {
				index = i;
				break;
			}
		}
		return index;
	}
}
```

`Lab 3 - StackTests.java`
```java
import static org.junit.Assert.*;

import org.junit.After;
import org.junit.Before;
import org.junit.Test;

public class StackTests {

  private Stack<String> stack;
  
  @Before
  public void setUp() throws Exception {
    stack = new Stack<>();
  }

  @After
  public void tearDown() throws Exception {
    stack = null;
  }

  @Test
  public void test_push_adds_to_stack_and_pop_removes_in_order() {
    stack.push("A");
    stack.push("B");
    stack.push("C");
    assertEquals("C", stack.pop());
    assertEquals("B", stack.pop());
    stack.push("D");
    assertEquals("D", stack.pop());
    assertEquals("A", stack.pop());
  }
  
  @Test
  public void test_push_adds_to_stack_and_peek_twice_shows_same_object_on_top_of_stack() {
    stack.push("A");
    stack.push("B");
    stack.push("C");
    assertEquals("C", stack.peek());
    assertEquals("C", stack.peek());
    assertEquals("C", stack.peek());
  }
  
  @Test
  public void test_pop_empty_stack_returns_null() {
    assertNull(stack.pop());
  }
  
  @Test
  public void test_peek_empty_stack_returns_null() {
    assertNull(stack.peek());
  }
}
```

#### The List Interface
1. The List Interface
2. List Methods
3. LinkedList
4. Vector
5. Using List - Best Practices
6. Labs

`ListInterface/com.skilldistillery.listinterface.drills.PlanetList`
```java
//Planet.java
import java.util.Objects;

public class Planet {
	private String name;
	private long orbit;
	private int diameter;

	public Planet(String name, long orbit, int diameter) {
		this.name = name;
		this.orbit = orbit;
		this.diameter = diameter;
	}

	public String getName() {
		return name;
	}

	public long getOrbit() {
		return orbit;
	}

	public int getDiameter() {
		return diameter;
	}

	@Override
	public int hashCode() {
		return Objects.hash(diameter, name, orbit);
	}

	@Override
	public boolean equals(Object obj) {
		if (this == obj)
			return true;
		if (obj == null)
			return false;
		if (getClass() != obj.getClass())
			return false;
		Planet other = (Planet) obj;
		return diameter == other.diameter && Objects.equals(name, other.name) && orbit == other.orbit;
	}

	@Override
	public String toString() {
		return "Planet [Name=" + name + ", Orbit=" + orbit + ", Diameter=" + diameter + "]";
	}
}
```

```java
//PlanetList.java
import java.util.List;

public class PlanetList {

	public static void main(String[] args) {
		PlanetList p = new PlanetList();
		p.run();
	}

	private void run() {
		List<Planet> planets = PlanetUtilities.getPlanets();
		System.out.println(planets);

		// Create a new Planet object using the Planet constructor call below.
		Planet jupiter = new Planet("Jupiter", 778_330_000, 142_984);

		// Print true or false for whether the List contains this planet
		System.out.println(planets.contains(jupiter));

		// If this was not what you expected, change the Planet class to support
		// comparison to other Planets. (Hint: what method does Java use to see if
		// one Object equals another Object?)

		// Try to find the index of this planet in the List, and print out that index.
		System.out.println(planets.indexOf(jupiter));

		// Now remove Jupiter by passing the object reference you created, and
		// print true or false for whether removing worked.
		boolean didRemove = planets.remove(jupiter);
		System.out.println(didRemove);
		
		for (Planet planet : planets) {
			System.out.println(planet);
		}
	}
}
```

```java
//PlanetUtilities.java
import java.util.ArrayList;
import java.util.List;

public class PlanetUtilities {
	public static List<Planet> getPlanets() {
		List<Planet> planets = new ArrayList<>();

		planets.add(new Planet("Mercury", 57_910_000, 4_880));
		planets.add(new Planet("Venus", 108_200_000, 12_103));
		planets.add(new Planet("Earth", 149_600_000, 12_756));
		planets.add(new Planet("Mars", 227_940_000, 6_794));
		planets.add(new Planet("Jupiter", 778_330_000, 142_984));
		planets.add(new Planet("Saturn", 1_429_400_000, 120_536));
		planets.add(new Planet("Uranus", 2_870_990_000L, 51_118));
		planets.add(new Planet("Neptune", 4_504_000_000L, 49_532));

		return planets;
	}
}
```

`ListInterface/com.skilldistillery.listinterface.drills.LinkedListAdding`
```java
import java.time.Duration;
import java.time.LocalDateTime;
import java.util.ArrayList;
import java.util.LinkedList;
import java.util.List;

public class LinkedListAdding {

  public static void main(String[] args) {
    LinkedListAdding app = new LinkedListAdding();
    app.run();
  }
  
  private void run() {
    // Run the program with ArrayList, and note the time taken.
    // Then change myList refer to a LinkedList, and run again.
    List<Planet> myList = new LinkedList<>();
    fillLargeList(myList);
  }
  
  
  /**
   * This method will fill a List, alternating between adding to the
   * beginning and end. It will also calculate and print the time this
   * operation takes.
   */
  private void fillLargeList(List<Planet> list){
    
    // Get the start time
    LocalDateTime start = LocalDateTime.now();  // You will learn about this class
    
    // fill the list, alternating between beginning and end.
    int numElements = 100_000;
    System.out.println("Adding to " + list.getClass().getSimpleName() + "...");
    for(int i=0; i < numElements; i++) {
      if(i % 2 == 0) {
        list.add(0, new Planet("EvenPlanet", 100, 100));
      }
      else {
        list.add(new Planet("OddPlanet", 100, 100));
      }
    }
    
    // Get the end time
    LocalDateTime end = LocalDateTime.now();
    
    // Duration can calculate time elapsed
    Duration d = Duration.between(start, end);
    System.out.println(d.toMillis() + " milliseconds");
  }
}
```

`ListInterface/com.skilldistillery.listinterface.drills.LinkedListPositionalAccess`
```java
import java.time.Duration;
import java.time.LocalDateTime;
import java.util.ArrayList;
import java.util.LinkedList;
import java.util.List;

public class LinkedListPositionalAccess {

	public static void main(String[] args) {
		LinkedListPositionalAccess app = new LinkedListPositionalAccess();
		app.run();

	}

	private void run() {
		// Run the program with ArrayList, and note the time taken.
		// Then change myList refer to a LinkedList, and run again.
		List<Planet> list = new LinkedList<>();

		fillLargeList(list);

		// Get an element
		getFromList(list);
	}

	private void getFromList(List<Planet> list) {
		int size = list.size();
		int index = size * 3 / 4;
		System.out.println("Getting element from " + list.getClass().getSimpleName() + " index " + index);

		// Get the start time
		LocalDateTime start = LocalDateTime.now(); // You will learn about this class

		list.get(index);

		// Get the end time
		LocalDateTime end = LocalDateTime.now();

		// Duration can calculate time elapsed
		Duration d = Duration.between(start, end);
		System.out.println(list.getClass().getSimpleName() + " " + d.toMillis() + " milliseconds");
	}

	private void fillLargeList(List<Planet> list) {
		int numElements = 10_000_000;
		System.out.println("Adding to " + list.getClass().getSimpleName() + "...");
		for (int i = 0; i < numElements; i++) {
			list.add(new Planet("Planet", 100, 100));
		}
	}
}
```

`Lab 1 - NumbersList.java`
```java
import java.util.LinkedList;
import java.util.List;

public class NumbersList {
	public static void main(String[] args) {
		NumbersList nl = new NumbersList();
		nl.run();
	}

	private void run() {
		List<Integer> numbers = new LinkedList<>();

		for (int i = 0; i < 10; i++) {
			numbers.add((int) (10 + Math.random() * (90 + 1)));
		}

		System.out.println(numbers);
	}
}
```

`Lab 2 - SortNumbersList.java`
```java
import java.util.LinkedList;
import java.util.List;

public class SortNumbersList {
	public static void main(String[] args) {
		SortNumbersList snl = new SortNumbersList();
		snl.run();
	}

	private void run() {
		List<Integer> numbers = new LinkedList<>();

		for (int i = 0; i < 10; i++) {
			numbers.add((int) (10 + Math.random() * (90 + 1)));
		}

		System.out.println("Before Sort:");
		System.out.println(numbers);

		sortAndPrintList(numbers);
	}

	private void sortAndPrintList(List<Integer> numbers) {
		// bubbleSort(numbers);
		insertionSort(numbers);
		System.out.println("After sort");
		System.out.println(numbers);
	}

	private void bubbleSort(List<Integer> nums) {
		boolean swapped = true;
		while (swapped) {
			swapped = false;
			for (int i = 0; i < nums.size() - 1; i++) {
				if (nums.get(i) > nums.get(i + 1)) {
					// swap elements
					int temp = nums.get(i);
					nums.set(i, nums.get(i + 1));
					nums.set(i + 1, temp);
					swapped = true;
				}
			}
		}
	}

	private void insertionSort(List<Integer> nums) {
		for (int i = 1; i < nums.size(); i++) {
			int temp = nums.get(i);
			int j = i;

			while (j > 0 && nums.get(j - 1) > temp) {
				nums.set(j, nums.get(j - 1));
				j--;
			}
			nums.set(j, temp);
		}

	}
}
```

#### Exceptions
1. Introduction to Exceptions
2. The Exception Class
3. Checked Exceptions
4. Labs - Handling Exceptions
5. The Throwable Hierarchy *
6. Throwing Your Own Exceptions *
7. Exceptions and Inheritance *
8. finally
9. Labs *

`Exceptions/com.skilldistillery.exceptions.drills.TryCatchDrill`
```java
package com.skilldistillery.exceptions.drills;

import java.util.InputMismatchException;

import java.util.Scanner;

public class TryCatchDrill {

	public static void main(String[] args) {
		TryCatchDrill drill = new TryCatchDrill();
		Scanner scanner = new Scanner(System.in);
		drill.launch(scanner);
		scanner.close();

	}

	private void launch(Scanner scanner) {
		String keepGoing = "Y";
		while (keepGoing.toUpperCase().equals("Y")) {
			System.out.print("Enter a whole number: ");
			try {
				int number = scanner.nextInt();
				if (number % 2 == 0) {
					System.out.println(number + " is even.");
				} else {
					System.out.println(number + " is odd.");
				}
			} catch (InputMismatchException e) {
				System.out.println("Invalid input.");
				scanner.nextLine(); // Clear input buffer
			}
			System.out.print("Keep going? (Y/N)");
			keepGoing = scanner.next();
		}
	}
}
```

`Exceptions/com.skilldistillery.exceptions.drills.TryCatchDrill`
```java
package com.skilldistillery.exceptions.drills;

import java.util.InputMismatchException;

import java.util.Scanner;

public class TryCatchDrill {

	public static void main(String[] args) {
		TryCatchDrill drill = new TryCatchDrill();
		Scanner scanner = new Scanner(System.in);
		drill.launch(scanner);
		scanner.close();

	}

	private void launch(Scanner scanner) {
		String keepGoing = "Y";
		while (keepGoing.toUpperCase().equals("Y")) {
			System.out.print("Enter a whole number: ");
			try {
				int number = scanner.nextInt();
				if (number % 2 == 0) {
					System.out.println(number + " is even.");
				} else {
					System.out.println(number + " is odd.");
				}
			} catch (InputMismatchException e) {
				System.err.println("Invalid input.");
				scanner.nextLine(); // Clear input buffer
			}
			System.out.print("Keep going? (Y/N)");
			keepGoing = scanner.next();
		}
	}
}
```

`ErrorDrill.java`
```java
public class ErrorDrill {
	private static int callCount;

	public static void main(String[] args) {
		ErrorDrill drill = new ErrorDrill();
		drill.callMe();
	}

	private void callMe() {
		// 1. Increment callCount
		callCount++;

		// 2. Print out callCount
		System.out.println(callCount);

		// 3. Call callMe()
		this.callMe();

		// 4. Print "callMe finished."
		System.out.println("callMe finished.");
	}
}
```

`Exceptions/com.skilldistillery.exceptions.drills.TryCatchDrill`
```java
import java.util.InputMismatchException;
import java.util.Scanner;

public class TryCatchDrill {

	public static void main(String[] args) {
		TryCatchDrill drill = new TryCatchDrill();
		Scanner scanner = new Scanner(System.in);
		drill.launch(scanner);
		scanner.close();
	}

	private void launch(Scanner scanner) {
		String keepGoing = "Y";
		while (keepGoing.toUpperCase().equals("Y")) {
			System.out.print("Enter a whole number: ");
			try {
				int number = scanner.nextInt();
				if (number % 2 == 0) {
					System.out.println(number + " is even.");
				} else {
					System.out.println(number + " is odd.");
				}
			} catch (InputMismatchException e) {
				System.out.println("Invalid input.");
				scanner.nextLine(); // Clear input buffer
			}
			System.out.print("Keep going? (Y/N)");
			keepGoing = scanner.next();
		}
	}
}
```

`Lab 1 - Circle.java`
```java
import static java.lang.Math.*;

public class Circle extends Shape {
	double radius;

	public double getRadius() {
		return radius;
	}

	public void setRadius(double radius) {
		if (radius <= 0) {
			throw new IllegalArgumentException("Radius must be greater than zero.");
		}
		this.radius = radius;

	}

	@Override
	public double getArea() {
		return PI * pow(radius, 2);
	}

	public Circle(double radius) {
		super();
		this.setRadius(radius);
	}

	public Circle() {
		super();
	}

	public Circle(int xCoordinate, int yCoordinate) {
		super(xCoordinate, yCoordinate);
	}

	public Circle(int xCoordinate, int yCoordinate, double radius) {
		super(xCoordinate, yCoordinate);
		this.setRadius(radius);
	}

	@Override
	public String toString() {
		StringBuilder builder = new StringBuilder();
		builder.append("Circle [radius=").append(radius).append("]");
		return builder.toString();
	}
}
```

`Lab 1 - Rectangle.java`
```java
public class Rectangle extends Shape {
	double width;
	double height;

	public double getWidth() {
		return width;
	}

	public void setWidth(double width) {
		if (width <= 0) {
			throw new IllegalArgumentException("Width must be greater than zero.");
		}
	  this.width = width;
  }

	public double getHeight() {
		return height;
	}

	public void setHeight(double height) {
		if (height <= 0) {
			throw new IllegalArgumentException("Height must be greater than zero.");
		}
		this.height = height;
	}

	@Override
	public double getArea() {
		return width * height;
	}

	public Rectangle(double width, double height) {
		super();
		this.setWidth(width);
		this.setHeight(height);
	}

	public Rectangle() {
		super();
	}

	public Rectangle(int xCoordinate, int yCoordinate) {
		super(xCoordinate, yCoordinate);
	}

	public Rectangle(int xCoordinate, int yCoordinate, double width, double height) {
		super(xCoordinate, yCoordinate);
		this.setWidth(width);
		this.setHeight(height);
	}

	@Override
	public String toString() {
		StringBuilder builder = new StringBuilder();
		builder.append("Rectangle [width=").append(width).append(", height=").append(height).append("]");
		return builder.toString();
	}

	@Override
	public int hashCode() {
		final int prime = 31;
		int result = 1;
		long temp;
		temp = Double.doubleToLongBits(height);
		result = prime * result + (int) (temp ^ (temp >>> 32));
		temp = Double.doubleToLongBits(width);
		result = prime * result + (int) (temp ^ (temp >>> 32));
		return result;
	}

	@Override
	public boolean equals(Object obj) {
		if (this == obj)
			return true;
		if (obj == null)
			return false;
		if (getClass() != obj.getClass())
			return false;
		Rectangle other = (Rectangle) obj;
		if (Double.doubleToLongBits(height) != Double.doubleToLongBits(other.height))
			return false;
		if (Double.doubleToLongBits(width) != Double.doubleToLongBits(other.width))
			return false;
		return true;
	}
}
```

`Lab 1 - ShapeTester.java`
```java
public class ShapeTester {
  private Shape[] shapes;

  public static void main(String[] args) {
    ShapeTester tester = new ShapeTester();
    tester.test();
  }

  private void test() {
    shapes = new Shape[10];
    
    shapes[0] = new Circle(2.2);
    shapes[1] = new Rectangle(2.0, 4.0);
    shapes[2] = new Circle(0);  // Exception in thread "main" java.lang.IllegalArgumentException: Radius must be greater than zero.
    // Execution stops, and the exception propagates to main() and then to the JVM, which exits.
    shapes[3] = new Rectangle(3.0, -5.0);
    shapes[4] = new Rectangle(17.7, 31.1);
    
    printShapes(shapes);
  }

  private void printShapes(Shape[] shapes) {
    for (Shape shape : shapes) {
      if (shape != null) {
        System.out.println(shape + ", area="+shape.getArea());
      }
    }
  }
}
```

`Lab 2 - ShapeTester.java`
```java
public class ShapeTester {
	private Shape[] shapes;

	public static void main(String[] args) {
		ShapeTester tester = new ShapeTester();
		tester.test();
	}

	private void test() {
		shapes = new Shape[10];

		try {
			shapes[0] = new Circle(2.2);
			shapes[1] = new Rectangle(2.0, 4.0);
			shapes[2] = new Circle(0); // Exception in thread "main" java.lang.IllegalArgumentException: Radius must be
										// greater than zero.
			// Execution stops, and the exception propagates to main() and then to the JVM,
			// which exits.
			shapes[3] = new Rectangle(3.0, -5.0);
			shapes[4] = new Rectangle(17.7, 31.1);
		} catch (IllegalArgumentException e) {
			System.err.println(e.getMessage());
		}

		printShapes(shapes);
	}

	private void printShapes(Shape[] shapes) {
		for (Shape shape : shapes) {
			if (shape != null) {
				System.out.println(shape + ", area=" + shape.getArea());
			}
		}
	}
}
```

`Lab 3 - ShapeTester.java`
```java
public class ShapeTester {
	private Shape[] shapes;

	public static void main(String[] args) {
		ShapeTester tester = new ShapeTester();
		tester.test();
	}

	private void test() {
		shapes = new Shape[10];

		try {
			shapes[0] = new Circle(2.2);
		} catch (IllegalArgumentException e) {
			System.err.println(e.getMessage());
		}

		try {
			shapes[1] = new Rectangle(2.0, 4.0);
		} catch (IllegalArgumentException e) {
			System.err.println(e.getMessage());
		}

		try {
			shapes[2] = new Circle(0); // Exception in thread "main" java.lang.IllegalArgumentException: Radius must be
		} catch (IllegalArgumentException e) {
			System.err.println(e.getMessage());
		}

		// greater than zero.
		// Execution stops, and the exception propagates to main() and then to the JVM,
		// which exits.

		try {
			shapes[3] = new Rectangle(3.0, -5.0);
		} catch (IllegalArgumentException e) {
			System.err.println(e.getMessage());
		}

		try {
			shapes[4] = new Rectangle(17.7, 31.1);
		} catch (IllegalArgumentException e) {
			System.err.println(e.getMessage());
		}

		printShapes(shapes);
	}

	private void printShapes(Shape[] shapes) {
		for (Shape shape : shapes) {
			if (shape != null) {
				System.out.println(shape + ", area=" + shape.getArea());
			}
		}
	}
}
```

`Lab 4 - Circle.java`
```java

```

`Lab 4 - Rectangle.java`
```java

```

`Lab 4 - ShapeTester.java`
```java

```

#### Project: Data Entry with Exceptions

### Week 3 - Day 2

#### Testing Exceptions with JUnit
1. JUnit and Exceptions
2. Testing Exceptions with try and catch
3. Labs

``
```java

```

#### Input/Output Streams
1. Overview of Streams
2. File Object
3. BufferedReader
4. PrintStream and PrintWriter
5. Closing Streams
6. Labs

`Lab 1 - SearchEmployees.java`
```java

```

`Lab 2 - PlanetReader.java`
```java

```

`Lab 3 - PlanetReader2.java`
```java

```

`Lab 4 - SearchEmployees.java`
```java

```

#### The Set Interface
1. The Set Interface
2. Set Implementation Classes - HashSet and LinkedHashSet
3. Iterator Explained *
4. SortedSet Interface and TreeSet Class
5. Collection Superinterface
6. Labs

`SetInterface/com.skilldistillery.setinterface.drills.SetTest`
```java
import java.util.HashSet;
import java.util.Iterator;
import java.util.Set;

public class SetTest {

  public static void main(String[] args) {
    SetTest st = new SetTest();
    st.launch();
  }
  
  public void launch() {
    Album al1 = new Album(1, "The Beatles", "The Beatles 1");
    Album al2 = new Album(2, "Prince", "The Very Best of Prince");
    Album al3 = new Album(3, "AC/DC", "Let There Be Rock");
    Album al4 = new Album(3, "AC/DC", "Let There Be Rock");
    
    Set<Album> albumCollection = new HashSet<>();
    
    // Place each call to add in a System.out.println() and run
    // the application. 
    System.out.println(albumCollection.add(al1));
    System.out.println(albumCollection.add(al2));
    System.out.println(albumCollection.add(al3));
    System.out.println(albumCollection.add(al4));
    
//    albumCollection.add(al1);
//    albumCollection.add(al2);
//    albumCollection.add(al3);
//    albumCollection.add(al4); //Doesn't get added because duplicate only store unique elements.
    
    printAlbums(albumCollection);
  }
  
  private void printAlbums(Set<Album> collection) {
    Iterator<Album> it = collection.iterator();
    while (it.hasNext()) {
      System.out.println(it.next());
    }
  }
}
```

`SetInterface/com.skilldistillery.setinterface.drills.SportsTeamApp`
```java
import java.util.HashSet;
import java.util.Iterator;
import java.util.Set;

public class SportsTeamApp {

	public static void main(String[] args) {
		SportsTeamApp app = new SportsTeamApp();
		app.launch();
	}

	private void launch() {
		SportsTeam t1 = new SportsTeam("Denver", "Vampires");
		SportsTeam t2 = new SportsTeam("Michigan", "Werewolves");
		SportsTeam t3 = new SportsTeam("Derry", "Clowns");
		SportsTeam t4 = new SportsTeam("Derry", "Clowns");
		SportsTeam t5 = new SportsTeam("Houston", "Chupacabras");

		Set<SportsTeam> teams = new HashSet<>();
		addTeam(teams, t1);
		addTeam(teams, t2);
		addTeam(teams, t3);
		addTeam(teams, t4);
		addTeam(teams, t5);

		// Iterate through the contents of the Set using an iterator, and print them to
		// the screen.
		Iterator<SportsTeam> st = teams.iterator();
		while (st.hasNext()) {
			SportsTeam s = st.next();
			System.out.println(s);
		}

		// If the results are not as expected, fix SportsTeam.
	}

	// Change addTeam() to add the object to the Set.
	private void addTeam(Set<SportsTeam> set, SportsTeam t) {
		boolean added = set.add(t);
		System.out.println(t.getName() + " added: " + added);
	}
}
```

`SetInterface/com.skilldistillery.setinterface.drills.CollectionTest`
```java
import java.util.ArrayList;
import java.util.Collection;
import java.util.HashSet;

public class CollectionTest {

	public static void main(String[] args) {
		// Assign an ArrayList to c1
		Collection<String> c1 = new ArrayList<>();

		// Add four Strings to c1 - your choice of Strings.
		c1.add("A");
		c1.add("B");
		c1.add("C");
		c1.add("D");

		// Call addAll(c1) on c1; you are trying to add the elements of c1
		// to what is already in c1. Store the result of addAll in a variable
		// and print it to the screen.
		boolean result = c1.addAll(c1);

		// Collection classes have good toString() methods, so we will use
		// System.out.println() to see the contents.
		System.out.println("Contents of c1: " + c1);
		System.out.println("Result of addAll is " + result);

		// Repeat the process with c2, using a HashSet
		Collection<String> c2 = new HashSet<>();
		c2.add("D");
		c2.add("E");
		c2.add("F");
		c2.add("G");

		result = c2.addAll(c1);

		System.out.println("Contents of c2: " + c2);
		System.out.println("Result is " + result);
	}
}
```

`Lab 1 - NameApp.java`
```java
import java.io.BufferedReader;
import java.io.FileNotFoundException;
import java.io.FileReader;
import java.io.IOException;
import java.util.ArrayList;
import java.util.HashSet;
import java.util.List;
import java.util.Set;

public class NameApp {

	public static void main(String[] args) {
		NameApp nA = new NameApp();
		nA.run();
	}

	public void run() {
		// Initializes two collections: A List named 'listToFill' and a Set named
		// 'setToFill'
		List<String> listFill = new ArrayList<String>();
		Set<String> setFill = new HashSet<>();

		// Call the readNamesIntoCollections method, passing in the two collections
		// (listToFill and setToFill)
		// as arguments and assigns the returned number of lines to the variable
		// numLines.
		int numLines = namesInCollection(listFill, setFill);

		// Print the sizes of the List and Set to the console, as well as the number of
		// lines in the file.
		System.out.println("List Size: " + listFill.size());
		System.out.println("Set Size: " + setFill.size());
		System.out.println("Lines in File: " + numLines);
	}

	// Define a private method 2 args: 'List<String> namesList, Set<String>
	// namesSet'
	private int namesInCollection(List<String> namesList, Set<String> namesSet) {
		// Initialize a variable numLines to 0 and declare a BufferedReader named reader
		// and set it to null.
		BufferedReader reader = null;
		int numLines = 0;
		try {
			reader = new BufferedReader(new FileReader("names.txt"));
			String line;
			// While line !=null it adds each line to both namesList and namesSet, and
			// increments numLines.
			while ((line = reader.readLine()) != null) {
				namesList.add(line);
				namesSet.add(line);
				numLines++;
			}
			// When the program tries to open a file that doesn't exist at the specified
			// path.
		} catch (FileNotFoundException e) {
			e.printStackTrace();
			// General Exception.
		} catch (IOException e) {
			e.printStackTrace();
			// Object that is null.
		} finally {
			if (reader != null) {
				try {
					reader.close();
				} catch (IOException e) {
					e.printStackTrace();
				}
			}
		}
		return numLines;
	}
}
```

#### Project: Name Separator App

### Week 3 - Day 3

#### Garbage Collection
1. Objects on the Heap
2. Garbage Collection
3. Memory Management Strategies
4. The finalize method
5. Understanding Garbage Collection
6. Labs

``
```java

```

#### Debugging Programs
1. What is Debugging?
2. Commenting Out Code
3. Manual Output in Code
4. Making Debugging Print Statements Conditional
5. Tools to Debug Programs
6. Debugging in Eclipse
7. The Debug Perspective
8. Breakpoints
9. Examining Variables
10. Controlling Program Execution
11. Labs

``
```java

```

#### Homework Project: Jets

### Week 3 - Day 4

#### Regular Expressions
1. Introducing Regular Expressions
2. Options
3. Literals and Wild Cards
4. Assertions
5. Quantifiers
6. Labs 1
7. Grouping and Alternatives
8. Labs 2

``
```java

```

#### Regular Expressions in Java
1. Regular Expressions in Java
2. The Pattern Class
3. The Matcher Class
4. Capturing Groups
5. String Methods That Use Regular Expressions
6. Labs

``
```java

```

#### The Map Interface
1. The Map Collection
2. Map Implementation Class - HashMap
3. Map Implementation Classes - Hashtable, LinkedHashMap, and TreeMap
4. When to Use a Map *
5. Labs

``
```java

```

#### Project: Project: Pig Latin

#### Project: Project: Declaration of Independence

### Week 3 - Day 5

#### Collection Sorting and Tuning
1. Sorting with Comparable
2. Sorting with Comparator
3. Sorting Lists
4. Sorting Maps
5. Sorting Arrays
6. Collections Utility Methods
7. Labs

``
```java

```

#### Project: Lottery: NBA Draft

#### Project: Lottery: Powerball

### Week 3 - Day 6

#### HashMap Internals
1. Keys and hashCode
2. Hash Buckets
3. Map Entries
4. Tuning HashMap
5. Labs

``
```java

```

#### Project: Project: Mad Libs

### Week 3 - Day 7

#### The Java Virtual Machine
1. The Java Virtual Machine
2. The Java Runtime Environment
3. The Java Development Kit
4. The Java Language Specification
5. Labs

``
```java

```

#### The args Array
1. The main Method
2. The args Array
3. Handling Command-Line Arguments
4. Testing args In Eclipse
5. Labs

``
```java

```

#### Intermediate Interfaces
1. Smart Home - Part 2
2. Interface Fields
3. Interface Inheritance
4. Static Interface Methods
5. Interface Default Methods
6. Multiple Inheritance
7. Labs

``
```java

```

#### Project: Roman Numerals

#### Project: Project: White Rabbit

### Week 3 - Day 8

#### Enumerated Types
1. enum Types
2. enum Details
3. Using enum
4. enum Methods
5. enum Members
6. Labs

``
```java

```

#### Homework Project: Blackjack

### Week 3 - Day 9

#### Dates and Times
1. Temporal Data
2. LocalDate
3. LocalTime
4. Date-Times and Instant
5. Duration and Period
6. DateTimeFormatter
7. Labs

``
```java

```

#### Project: History

#### Project: Working with Dates and Times

#### Inner Classes
1. Inner Classes
2. Member Classes
3. Local Classes
4. Anonymous Classes
5. Anonymous Classes and Interfaces
6. Instance Initializers
7. Compiling Inner Classes
8. Labs

``
```java

```

#### Project: Sorting and Filtering with Inner Classes

### Week 3 - Day 10

#### Introduction to Lambda Expressions
1. Inner Classes Review
2. Lambda Expressions
3. Translating Inner Classes to Lambdas
4. Lambda Rules and Syntax
5. Lambdas and Interfaces
6. Predicate<T> Functional Interface *
7. Standard Functional Interfaces *
8. Labs *

#### Project: Sorting and Filtering with Lambdas

#### Lambda Examples

### Week 3 - Day 11

#### JUnit 5
1. Introduction
2. Test Cases
3. Test Case Setup
4. Test Method Names
5. Assertions
6. Testing Exceptions
7. Labs

``
```java

```
