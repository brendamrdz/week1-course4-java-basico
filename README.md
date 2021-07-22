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

## Declaring variables
## Working with functions
## Loops
## Conditionals
## Programming logic
## Algorithms
