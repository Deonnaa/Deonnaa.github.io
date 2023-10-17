Week 1 Notes.md

## [Week 1](https://github.com/SkillDistillery/SD41/blob/main/jfop/README.md)

## Day 1

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

### Day 2

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

### Day 3

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

#### Project: Hi/Lo

#### Project: Remote Control Simulator

### Day 4

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

#### for Loops
1. for Loops
2. A for Loop Diagram
3. for Loop Parts
4. for Loop Body
5. break and continue Statements
6. For Loop - When and Why
7. Labs

#### Project: Fizz Buzz

#### Project: Fibonacci Series

### Day 5

#### Numeral Systems
1. Counting and Tallying
2. Positional Notation
3. Numeral Systems for Programming
4. Numeric Literals in Java
5. The printf() Method

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

#### Casting Data Types
1. Implicit Type Conversions
2. Promotion of Data Types in Arithmetic
3. Promotion in Integer Arithmetic
4. The Cast Operator
5. Casting Hints
6. Labs

#### Homework Project: Make Change (Cash Register)

### Day 6

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

#### Introduction to Objects
1. Classes
2. Creating Objects
3. Reference Variables
4. State and Behavior
5. Field Initialization
6. The static Keyword *
7. Some Objects You've Already Met
8. Labs

#### Project: Deaf Grandma

### Day 7

#### Advanced For Loops
1. Nested for Loops
2. Enhanced For Loops
3. Break and Continue With Enhanced For Loops
4. Labs

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

#### Project: Tic Tac Toe
