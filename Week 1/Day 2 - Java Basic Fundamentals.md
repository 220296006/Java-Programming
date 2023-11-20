# Java Basic Fundamentals: Variables

## Variable Definition

In Java, a variable is a named storage location that holds data, and its value can be changed during the execution of a program. Variables are fundamental to programming and are used to store and manipulate data in memory.

## Key Characteristics of Variables in Java

### 1. **Declaration:**

- Variables must be declared before they can be used.
- The declaration specifies the data type and the name of the variable.

```java

   int myVariable; // Declaration of an integer variable named myVariable

```

### 2. **Initialization:**

- Initialization is the process of giving a variable an initial value.
- It is typically done at the time of declaration or later in the program.

```java

int myVariable = 10; // Declaration and initialization in one line

```

### 3. **Data Types:**

- Java is a statically-typed language, meaning that the data type of a - variable must be explicitly specified during declaration.
- Common data types include int, double, char, boolean, and more.

```java

double pi = 3.14; // Declaration and initialization of a double variable

```

### 4. **Naming Conventions:**

- Variables must follow naming conventions.
- Names should be meaningful, start with a letter, and can include letters, digits, and underscores.

```java

String myName = "John"; // Declaration and initialization of a String variable

```

### 5. **Scope:**

- The scope of a variable defines where in the program it can be accessed.
- Variables can have local scope (limited to a block of code) or class scope (accessible throughout the class).

```java

public class Example {
    int classVariable; // Class-scoped variable

    public void myMethod() {
        int localVariable; // Local variable within a method
    }
}

```

### 6. **Final Keyword:**

The final keyword can be used to make a variable constant (its value cannot be changed once initialized).

```java

final int constantValue = 100; // Declaration and initialization of a final variable

```

# **Example Usage:**

```java

public class VariableExample {
    public static void main(String[] args) {
        // Declaration and initialization of variables
        int age = 25;
        double salary = 50000.50;
        char grade = 'A';
        boolean isStudent = true;

        // Printing variable values
        System.out.println("Age: " + age);
        System.out.println("Salary: " + salary);
        System.out.println("Grade: " + grade);
        System.out.println("Is Student: " + isStudent);
    }
}

```

In this example, various variables are declared, initialized, and their values are printed to the console.

# Data Types in Java

In Java, data types are used to define the type of data that a variable can hold. Java has two categories of data types: primitive data types and reference data types.

## 1. Primitive Data Types

### a. **Numeric Types:**

- **`byte`**: 8-bit signed integer.
- **`short`**: 16-bit signed integer.
- **`int`**: 32-bit signed integer.
- **`long`**: 64-bit signed integer.
- **`float`**: 32-bit floating-point number.
- **`double`**: 64-bit floating-point number.

```java
   int age = 25;
   double salary = 50000.50;

```

### b. **Character Type:**

- **`char`**: 16-bit Unicode character.

```java

char grade = 'A';

```

### c. **Boolean Type:**

- **`boolean`**: Represents true or false.

```java

boolean isStudent = true;

```

# 2. Reference Data Types

### a. **`Object Types`:**

- **`Classes and Interfaces`**: Objects of user-defined classes and interfaces.
- `**String**`: Represents a sequence of characters.

```java

String message = "Hello, Java!";

```

### b. **`Array Types:**

- Arrays can hold elements of the same data type.

```java

int[] numbers = {1, 2, 3, 4, 5};

```

## Default Values

- Primitive data types have default values:

- `0` for numeric types.
- `\u0000` (null character) for `char`.
- `false` for `boolean`.
Reference data types have a default value of `null`.

```java

public class DataTypesExample {
    public static void main(String[] args) {
        // Numeric Types
        byte myByte = 127;
        short myShort = 32767;
        int myInt = 2147483647;
        long myLong = 9223372036854775807L;
        float myFloat = 3.14f;
        double myDouble = 3.141592653589793;

        // Character Type
        char myChar = 'A';

        // Boolean Type
        boolean myBoolean = true;

        // Object Type (String)
        String myString = "Java Programming";

        // Array Type
        int[] myArray = {1, 2, 3, 4, 5};
    }
}

```

## Casting in Java Data Types

Casting in Java refers to the process of converting a value from one data type to another. This is necessary when you want to assign a value of one type to a variable of another type. In Java, casting can be broadly categorized into two types: Widening (Implicit) Casting and Narrowing (Explicit) Casting.

1. **`Widening (Implicit) Casting`**:

- Definition: It occurs automatically when a smaller data type is converted into a larger data type.

- No Data Loss: Widening casting is safe and does not result in data loss.

Example:

```java

int intValue = 10;
long longValue = intValue; // Widening casting (int to long)

```

2. **`Narrowing (Explicit) Casting`**:
Definition: It must be explicitly performed when a larger data type is converted into a smaller data type.

Data Loss Possible: Narrowing casting may result in data loss, as the larger data type may have a range of values that the smaller data type cannot accommodate.

```java

public class CastingExample {
    public static void main(String[] args) {
        // Widening Casting (Implicit)
        int intValue = 100;
        long longValue = intValue; // Widening casting (int to long)
        System.out.println("Widening Casting: " + longValue);

        // Narrowing Casting (Explicit)
        double doubleValue = 15.75;
        int truncatedValue = (int) doubleValue; // Narrowing casting (double to int)
        System.out.println("Narrowing Casting: " + truncatedValue);
    }
}

```

# Java Basic Fundamentals: Operators

Operators in Java are symbols that perform operations on operands. They are fundamental for manipulating variables and values. Here are some common types of operators in Java:

## 1. **`Arithmetic Operators`**

- **`+` (Addition):** Adds two operands.
- **`-` (Subtraction):** Subtracts the right operand from the left operand.
- **`*` (Multiplication):** Multiplies two operands.
- **`/` (Division):** Divides the left operand by the right operand.
- **`%` (Modulus):** Returns the remainder of the division.

```java

int a = 10, b = 3;
int sum = a + b;    // 13
int difference = a - b;  // 7
int product = a * b; // 30
int quotient = a / b;   // 3
int remainder = a % b;  // 1

```

## 2. **`Relational Operators`:**

- **`==` (Equal to):** Checks if two operands are equal.
- **`!=` (Not equal to):** Checks if two operands are not equal.
- **`>` (Greater than):** Checks if the left operand is greater than the right operand.
- **`<` (Less than):** Checks if the left operand is less than the right operand.
- **`>=` (Greater than or equal to):** Checks if the left operand is greater than or equal to the right operand.
- **`<=` (Less than or equal to):** Checks if the left operand is less than or equal to the right operand.

```java

int x = 5, y = 10;
boolean isEqual = (x == y);  // false
boolean isNotEqual = (x != y);  // true
boolean isGreater = (x > y);  // false
boolean isLess = (x < y);  // true
boolean isGreaterOrEqual = (x >= y);  // false
boolean isLessOrEqual = (x <= y);  // true

```

## 4. **`Assignment Operators`:**

- `=` (Assignment): Assigns the value on the right to the variable on the left.
- `+=`, `-=`, `*=`, `/=`, `%=`: Combined assignment and arithmetic operation.

```java

int a = 5;
a += 3;  // Equivalent to: a = a + 3; (a becomes 8)

```

## 5. **`Unary Operators`:**

- `++` (Increment): Increases the value of the operand by 1.
- `--` (Decrement): Decreases the value of the operand by 1.
- `+` (Unary Plus): Represents positive values.
- `-` (Unary Minus): Represents negative values.

```java

int num = 10;
num++;  // Increment by 1 (num becomes 11)
num--;  // Decrement by 1 (num becomes 10)
int positiveNum = +num;  // Positive value
int negativeNum = -num;  // Negative value

```

## 6. **`Conditional (Ternary) Operator`:**

- `? :` `(Conditional)`: A shorthand way to write an `if-else` statement.


```java 

import java.util.Scanner;

public class ArithmeticOperations {
    public static void main(String[] args) {
        // Create a Scanner object to read input from the user
        Scanner scanner = new Scanner(System.in);

        // Prompt the user to enter the first integer
        System.out.print("Enter the first integer: ");
        int num1 = scanner.nextInt();

        // Prompt the user to enter the second integer
        System.out.print("Enter the second integer: ");
        int num2 = scanner.nextInt();

        // Close the Scanner to prevent resource leak
        scanner.close();

        // Perform arithmetic operations
        int sum = num1 + num2;
        int difference = num1 - num2;
        int product = num1 * num2;
        double average = (double) (num1 + num2) / 2; // Convert to double for accurate average
        int maximum = Math.max(num1, num2);
        int minimum = Math.min(num1, num2);

        // Display the results
        System.out.println("Sum: " + sum);
        System.out.println("Difference: " + difference);
        System.out.println("Product: " + product);
        System.out.println("Average: " + average);
        System.out.println("Maximum: " + maximum);
        System.out.println("Minimum: " + minimum);
    }
}

```

# Java Classes and Objects

## Class Definition

```java
// Define a simple class named "Person"
class Person {
    // Instance variables (attributes)
    String name;
    int age;

    // Constructor method
    public Person(String name, int age) {
        this.name = name;
        this.age = age;
    }

    // Method to display information about the person
    public void displayInfo() {
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
    }
}

```

- **`Class: Person`** is a class that encapsulates the concept of a person with attributes (name and age).

- **`Instance Variables:`** `name` and `age` are instance variables, representing the attributes of the person.

- **`Constructor Method`:** The `Person` class has a constructor method used to initialize the instance variables when an object is created.

- **`Method`:** `displayInfo` is a method that prints information about a person.

## **`Object Creation and Usage`**

```java

// Main class to demonstrate the usage of the Person class
public class Main {
    public static void main(String[] args) {
        // Create an instance (object) of the Person class
        Person person1 = new Person("John", 25);

        // Access and modify instance variables
        person1.name = "John Doe";
        person1.age = 26;

        // Call a method on the object
        person1.displayInfo();

        // Create another instance of the Person class
        Person person2 = new Person("Alice", 30);

        // Call a method on the second object
        person2.displayInfo();
    }
}

```

- `Object Creation`: Instances of the `Person` class (`person1` and `person2`) are created using the `new` keyword.

- `Access and Modification`: Instance variables (`name` and `age`) are accessed and modified directly.

- `Method Invocation`: The `displayInfo` method is called on both objects to display information about the persons.

- `Encapsulation`: This example demonstrates the encapsulation of data (attributes) and behavior (methods) within a class.

- `Object-Oriented Programming`: The program follows the principles of object-oriented programming, where objects represent real-world entities.
