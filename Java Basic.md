# Java Basics


## 0. Getting Started 🚀

### Pre-request

- Install JDK
Run bellow command in terminal window to verify you installed jdk correctly.
```shell
java --version
```
- Install IDE
  - [IntelliJ IDEA](https://www.jetbrains.com/idea/download/#section=mac)
  - [Eclipse](https://www.eclipse.org/downloads/)


### Create the source file
- Open a text editor, type in code which defines a class HelloWorld and then save it int a file HelloWorld.java
- file and class name are case sensitive and must be matched exactly(except .java part)

**Example Code: HelloWorld.java**
```java
// The HelloWorld class implements an application
// that displays "Hello World!" to the standard output
public class HelloWorld {
	public static void main(String[] args) {
		//Display "Hello World!"
		System.out.println("Hello World!");
	}
}
```
### Compile the program
- compile HelloWrold.java by using the following command:
```shell
javac HelloWorld.java

# It generates a file named HelloWrold.class
```

### Run the program
- run the code through:
```shell
java HelloWorld

#It will return Hello World!
```
- Note that the command is java, not javac, and you refer to HelloWorld, not HelloWorld.java or HelloWorld.class

😢 Exception in thread "main" java.lang.NoClassDefFoundError: HelloWorld

If you see this error, you may need to set the environment variable CLASSPATH








## 1. Data Types

### Primitive Types
- byte : 8bits (1byte)
- char : 16bits (2byte)
- short : 16bits (2byte)
- int : 32bits
- float : 32bits
- long : 64bits
- double : 62bits
- boolean : 1bit


 📚[Primitive Data Types](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/datatypes.html)\
 📚[Package java.lang](https://docs.oracle.com/javase/9/docs/api/java/lang/package-use.html)\
 ❓ [Why single character file saved as 8bits(1byte) not 16bits? - Answers about UTF-16 UTF-8](https://stackoverflow.com/questions/24095187/char-size-8-bit-or-16-bit)
 

### Wrapper Class

📚[Autoboxing and Unboxing](https://docs.oracle.com/javase/tutorial/java/data/autoboxing.html)\
📚[The Numbers Classes](https://docs.oracle.com/javase/tutorial/java/data/numberclasses.html)

### Buffer Pool


## 2. Object-Oriented programming

### Procedural vs. Object-Oriented Programming 

- The unit in procedural programming is funciton, and unit in OOP is class.
- Procedural programming concentrates on creating function, while OOP starts from isloating the classes, and then look for the methods inside them.
- Procedural programming sperates the data of the program from the operations that manipulate the data, while OOP focus on both of them.

<img width="777" alt="Procedural vs OOP" src="https://user-images.githubusercontent.com/78633515/154190442-5634e1ab-a8a3-4716-8af8-c051faee8078.png">

### Concepts of Class and Object

- "Class" refers to a blueprint. It defines the variables and methods the object support.
- "Object" is an instance of a class. each object has a class which defines its data and behavior.

### Class Members

- A class can have three kinds of members:
  - **fields**: data variables which determine the status of the class or an object (e.g. )
  - **methos**: executable code of the class built from statemets. It allows us to manipulate/change the status of an object or access the value of the data member
  - **nested classes and nested interfaces** 

**Sample class**
```java
class Pencil {
  public String color = "red";
  public int length;
  public float diameter;
  
  pulbic static long nextID = 0;
  
  public void setColor (String newColor) {
  	color = newColor;  
  }
  
  public void getColor() {
  	return color;
  }

```
