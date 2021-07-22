# Java SE
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

## Language syntax
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
### Data types for integers (without decimals):

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
### Data types for floating numbers (with decimals):

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
## Matching between data types

