# Java SE
## Table of Contents

- [What is Java?](#what-is-java)
- [Java and JDK versions](#java-and-jdk-versions)
- [The most used Java tools](#the-most-used-java-tools)
- [Hello world in Java](#hello-world-in-java)
- [Stages of Java programming](#stages-of-java-programming)
- [Declaring variables](#declaring-variables)
- [Java Naming Convention](#java-naming-convention)
- [Types of data](#types-of-data)
  - [Data types for integers](#data-types-for-integers)
  - [Data types for floating](#data-types-for-floating)
  - [Char and boolean data types](#char-and-boolean-data-types)
  - [Matching between data types](#matching-between-data-types)
- [Assignment, Increment and Decrement Operators](#assignment-increment-and-decrement-operators)
- [Cast](#cast)
  - [Estimate](#estimate)
  - [Accuracy](#accuracy)
- [JAR files](#jar-files)
- [Logical Operators and Boolean Expressions](#logical-operators-and-boolean-expressions)
- [Conditionals](#conditionals)
  - [If statement](#if-statement)
  - [ELSE IF](#else-if)
  - [Ternary operators](#ternary-operators)
- [Switch](#switch)
- [What are the functions for?](#what-are-the-functions-for)
  - [Scope](#scope)
- [Java Docs](#java-docs)
- [Loops](#loops)
  - [Do while loop](#do-while-loop)
  - [While loop](#while-loop)
  - [For loop](#for-loop)

## What is Java? 
Java is a high-level programming language that helps us build applications for different devices and operating systems.
It was created in 1991 by James Gosling while working at Sun Microsystems, a company that was later acquired by Oracle. This means that Java is very well maintained, but also has some changes that not everyone will agree with.


Java has two categories: Standard Edition for building desktop or console applications and Enterprise Edition for companies to build state-of-the-art web applications.


" Java follows the philosophy of Write Once, Run Anywhere (WORA). "

## Java and JDK versions

The JDK or Java Development Kit consists of the following elements:

- Java Runtime Environment (JRE): The Java virtual machine, which allows us to write the same code to work the same on all devices and operating systems.
- Java Compiler: The one in charge of translating our Java code into a language that can understand and interpret our virtual machine.
- Development APIs: A code base ready to help us develop.
The development APIs with Java have evolved over time, so there are different versions of Java that you can use. The version that raised the most popularity and job offers with Java was Java SE 6.

In Java SE 9 they announced that updates would occur every 6 months, but the LTS (Long Time Support) versions will have maintenance for 3 years.
Java SE 11 LTS, is the first version of Java with license. We can only use it for free when working in development and testing environments. Otherwise, we have to pay 2.5 USD per month per desktop user and 25 USD per processor for server applications.

Fortunately, OpenJDK is a free and open source version of using Java SE Platform Edition
## The most used Java tools
Java 8 (LTS) is the most used version of Java until the beginning of 2019, but it will only have support until December 2020, after this date we will have to pay a license fee to continue with its support.

The most used tool to build web projects with Java is Maven, but there are also other alternatives such as Gradle. There are also frameworks like Spring to work with Java EE and ORMs like Hibernate to work with databases.

IDEs are integrated development environments, tools that help us write our code with editors, compilers, debuggers and GUI builders, all in one place.

The IDE recommended by Oracle is NetBeans, but there are also Eclipse and IntelliJ IDEA, the latter being the one that has gained the most traction thanks to Kotlin. All three tools are free, but IntelliJ IDEA also has a paid version.

## Hello world in Java
Java files use the .java extension. Therefore, to create our first "Hello, world" we can do it from a HelloWorld.java file.

The main method is the entry point of an application in different languages like Java, Kotlin and C++. Without this method our application will not run and will show an error.

In Java we define this method as follows:

public static void main (String[] args) {
  // actions
}

Therefore, this will be the code of our HolaMundo.java and we will be able to execute it with Right Click > Run 'HolaMundo.main()':
```bash
public class HolaMundo {
  public static void main (String[] args) {
    System.out.println("Hola, mundo!");
  }
}
```
## Stages of Java programming
Write our .java files.
Compile, load and verify our files with javac (IDEs allow us to compile with the push of a button).
When compiling we obtain .class files with code that our computers can understand (Byte Code).
The JVM (Java Virtual Machine) is in charge of executing the code so that it works on any device or operating system.
Java is a compiled and interpreted language at the same time.

<br><img src="https://github.com/brendamrdz/week1-course4-java-basico/blob/main/images/Stages%20of%20Java%20programming.JPG?raw=true" alt="alt text" width="30%" height="auto"><br><br>
## Declaring variables
A variable is a memory space (RAM) that contains a numeric, Boolean, text or other slightly more complex data type.
Variables in Java consist of a unique name and a value that can change during program execution. When declaring variables we must define the type of data we are going to use and a semicolon at the end;
```bash
public class Variables {
  public static void main(String[] args) {
    // Declare the variable speed of type int (integers)
    int spped;

    // Update the content of the variable speed:
    spped = 10; // if you had already declared the variable.

    // Declare a variable and assign a value to it at the same time:
    int salary = 1000;

    // Create a String variable:
    String eployeeName = "Brenda";
  }
}
```
## Java Naming Convention
A naming convention is a pattern that variable names must follow so that the code is organized, understandable and without repetition.

- Java is case sensitive, this point is key when following a naming convention.

- Variables must always start with a letter symbol, $ or _.

- You cannot use the - symbol anywhere in the variable.

- Constant variables are variables whose value will never change, so they must be written in all uppercase and using the _ character.

- We must use Upper Camel Case in the names of classes and files. And Lower Camel Case in the names of variables or methods.

```bash
// Upper Camel Case:
class ImClass {};

// Lower Camel Case
int ImNumberInt = 10;
```

## Types of data 
### Data types for integers
- byte: Occupies 1 byte of memory and its range is from -128 to 127.
- short: Occupies 2 bytes of memory and ranges from -32,768 to 32,727.
- int: It occupies 4 bytes of memory and its range is -2,147,483,648 to 2,147,483,647. It is very convenient to use, since it is not so small that our numbers do not fit, nor so - big that it wastes a lot of memory. It can store up to 10 digits.
- long: It occupies 8 bytes of memory and its range is from -9,223,372,372,036,854,775,808 to 9,223,372,036,854,775,807. To differentiate it from a long data type we must end the number with the letter L.
For example:
```bash
// Int:
int n = 1234567890;

// Long:
long nL = 123456789012345L;
```
### Data types for floating

- float: they occupy 4 bytes of memory and range from 1.40129846432481707e-45 to 3.40282346636638528860e+38. As long, we must place a letter F at the end.
- double: They occupy 8 bytes of memory and their range is 4.9406564584124654446544e-324d to 1.79769313486231570e+308d.
For example:
```bash
// Double:
double nD = 123.456123456;

// Float
float nF = 123.456F;
```
### Char and boolean data types
- char: It occupies 2 bytes and can only store 1 digit, we must use single quotes instead of double quotes.
- boolean: They are a logical data type, they only accept true and false values. It also occupies 2 bytes and stores only 1 digit.
Surely you noticed that we must always write the data type of our variables before defining their name and value. But this changes from Java 10 onwards: we only have to write the reserved word var and Java will define the data type of our variables automatically:
```bash
var salary = 1000; // INT
var pension = salary * 0.03; // DOUBLE
var totalSalary = salary - pension; // DOUBLE
```
#### Matching between data types
<br><img src="https://github.com/brendamrdz/week1-course4-java-basico/blob/main/images/cast-datatype.JPG?raw=true" alt="alt text" width="30%" height="auto"><br><br>

## Assignment, Increment and Decrement Operators

### Assignment operators:
**+=: a += b** is equivalent to **a = a + b.**

**-=: a -= b** is equivalent to **a = a - b.**

*=: a *= b is equivalent to **a = a * b.**

**/=: a /= b** is equivalent to **a = a / b.**

**%=: a %= b** is equivalent to **a = a % b.**

### Increment operators:

**++: i++** is equivalent to **i = i + 1.**
**--: i--** is equivalent to **i = i - 1.**

We can use these operators prefixed (++i) or postfixed (i++). The difference is in which operation is executed first:

## Mathematical operations
```bash
Math is a Java class that helps us to execute different mathematical operations:
Math.PI // 3.141592653589793

Math.E // 2.71828182845459045


Math.ceil(2.1) // 3.0 (round up)

Math.floar(2.1) // 2.0 (round down)


Math.pow(2, 3) // 8.0 (number raised to a power)

Math.sqrt(3) // 1.73... (square root)


Math.max(2, 3) // 3.0 (largest number)


// Area of a circle (PI * r^2):

Math.PI * Math.pow(r, 2).


// Area of a sphere (4 * PI * r^2):

4 * Math.PI * Math.pow(r, 2)


// Volume of a sphere ( (4/3) * PI * r^3):

(4/3) * Math.PI * Math.pow(r, 3).
```

## Cast

In programming there are situations where we need to change the data type of our variables, this is known as Cast.
### Estimate:
```bash
double monthlyDogs = dogsQuantity / 12.0;
// monthlyDogs: 2.5 (but it's not possible, we didn't rescue half a dog!)

int estimatedMonthlyDogs = (int) monthlyDogs;
// estimatedMonthlyDogs: 2

// Remember that rounding does not round, it just removes the decimals:
Math.sqrt(3) // 1.73205050807575688772
(int) Math.sqrt(3) // 1
```
### Accuracy:
```bash
int a = 30;
int b = 12;

a / b // 2
(double) a / b // 2.5
```


## .JAR files
The JAR files (Java Archive) are Java files with the code compiled from the .class files and compressed with the ZIP format so that later they can be interpreted and executed by the Java Virtual Machine (JVM).

To generate these files we can go to File > Project Structure > Artifacts and select the JAR > From modules with dependencies option. After this we can compile our project from Build > Build Artifacts > Build and we can place our executable files in the out/artifacts/ folder.

### Logical Operators and Boolean Expressions
**Equity operators:**
- Equality: **==**
- Inequality: **!=**


**Relational Operators:**
- Less than: **<**
- Greater than: **>**
- Less than or equal to: **<=**
- Greater than or equal to: **>=**


**Logical operators:**
- **&&** : AND (evaluate whether two or more conditions are true).
- **||** : OR (evaluate if at least one of the conditions is true).
- **!** : NOT (evaluate if the condition is NOT true).

## Conditionals
### If statement
Conditionals are the way computers make decisions, they will evaluate whether the condition for executing a piece of code is met. 
```bash
if (condition) {
  // instructions
}
```
The ELSE statement is the opposite of the IF statement: instead of executing a part of the code if the condition is true, it will only do so if the condition is NOT met:
```bash
if (condition) {
 // instructions
} else {
 // instructions
}
```
### ELSE IF
Remember that in addition to IF and ELSE statements, we can also use ELSE IF. We use this one when we want to evaluate some condition different from the IF.
```bash
if (condition) {
 // instructions
} else if (condition) {
}
```
### Ternary operators 
```bash
Ternary operators are another way to evaluate conditions, as well as IF and ELSE conditionals:
// Operador Ternario:
isTurnOnLight = (isTurnOnLight) ? false : true;
```


## Switch
**Switch to Java 11:**
```bash
switch (teacher) {
  case "Anahi":
    System.out.println("Java teacher!");
    break;
  case "Oscar":
    System.out.println("React.js teacher!");
    break;
  case "JuanDC":
    System.out.println("Hey kid, what are you doing here?");
    break;
  default:
    System.out.println("A new teacher!");
    break;
}
```
In a Switch: in this situation break makes the switch flow not continue executing to the next comparison, so that only a single condition is fulfilled.

**Switch from Java 12:**
```bash
switch (age) {
  case 1 -> System.out.println("You are 1 year old!");
  case 20 -> System.out.println("You are 20 years old!");
  default -> System.out.println("Your age is neither 1 nor 20");
}
```

##  What are the functions for?
Functions help us to execute code that, depending on the options we send it, will transform and return a certain result. Thanks to functions we can organize, modularize, reuse and avoid repetitions in our code.

All our functions must have a name. Optionally, they can take arguments and return a result. We must also specify the data type of our arguments and the final result of our function.
For example:
```bash
public int sum(int a, int b) {
  return a + b;
}
```
If our function does NOT return any data type we can use the reserved word void.

To use our functions we only need to assign the result of the function and its parameters to a variable with the same data type as the function:
```bash
int c = sum(5, 7);
```
### Scope
- The global variables: They are defined before entering a function or process and that as its name indicates can be called to processes in any place since they were previously declared.

- The local variables: They are those that are defined for a specific process in a specific function and only they are going to be recognized for that function or process, that is to say that if we try to make the call to a local variable in another function that is not the one of origin it will not recognize it as declared.
## Java Docs 
Java Docs is a tool used by many other tools and applications because it helps us to document all our code using comments. In addition, it allows us to visualize the documentation in HTML format.
```bash
// Single line comments 
 
/* Comment 
* on multiple 
* lines */ 
 
/** 
* Comment for Java Docs 
* */ ;
```
Let's document the convertToDolar function. Remember that this function returns a double number and receives two arguments: quantity (of type double) and currency (of type String):
```bash
/**
 * General description of our function.
 * 
 * @param quantity Description of the quanity parameter.
 * @param currency Description of the currency parameter (MXN or COP).
 * Description of the value we return in this function.
 * */
```
For the IDE to show the description and documentation of the functions we must enter IntelliJ IDEA > Preferences > Editor > General > Code Completion and enable the Show the documentarion popup option.

## Loops
### Do while loop
Loops  help us to execute a part of our code a number of times until some condition is met and we can continue with the execution of our code.
There are different loops. For example, the do while loop:
```bash
do {
  // instructions
} while (condition);
```

### While loop
The While Loop helps us to execute a part of the code as long as a condition is met. Remember to be very careful and make sure that the while loop condition changes at some point, otherwise, the loop will never stop and you will overload your program:

```bash
while (isTurnOnLight) {
  printSOS();
}
```

### For loop
The For Loop also helps us to execute a part of our code as many times as necessary for a condition to be met. In fact, the FOR loop gives us many aids to achieve this result in the easiest possible way:
```bash
// Structure:
for (initialization; condition; increment or decrement;) {
  // Instructions
}
```
## Arrays
Arrays are objects in which we can store more than one variable, a list of elements. Arrays are one-dimensional, but if we store arrays inside other arrays we can obtain multidimensional arrays.
Arrays are defined in code in the following ways:
```bash
// 1. Define the variable name and data type.
// that it will contain, either of the following two
// options is valid:
DataType[] variableName;
DataType variableName[];
```

```bash
// 2. Define the size of the array, the amount of elements
// we can store in the array:
Datatype[] variableName = new Datatype[capacity];
```

```bash
// Two-dimensional array:
Datatype[][] cities = new String[numberRows][numberColumns];
Since arrays can store multiple elements, the convention is to write variable names in plural.
```
Indexes are simple variables that help us identify positions in an array. These variables always store numbers, they start at 0 and increment from bottom to top and from left to right as we store more elements in our arrays.

To store a value in some position of our array we only have to use the index in the following way:

```bashvariableName[index] = value;```
