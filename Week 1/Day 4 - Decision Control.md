# **`Introduction to Decision Control in Programming`**

Decision control, often referred to as conditional statements or branching, is a fundamental concept in programming that allows a program to make decisions based on certain conditions. These conditions determine the flow of the program, enabling it to execute specific blocks of code based on whether a condition is true or false. Decision control structures help in creating dynamic and responsive programs.

## **`Types of Decision Control Statements:`**

## **`If Statement, If-Else Statement, Nested If Statement`**

## 1. **`If Statement:`**

- The `if` statement is a fundamental decision-making statement that executes a block of code only if a specified condition is true.

```java
   if (condition) {
       // Code to be executed if the condition is true
   }

```

Example:

```java

int x = 10;
if (x > 5) {
    System.out.println("x is greater than 5");
}

```

## 2.  **`If-Else Statement:`**

- The `if-else` statement provides an alternative block of code to execute if the condition in the `if` statement is false.

```java

if (condition) {
    // Code to be executed if the condition is true
} else {
    // Code to be executed if the condition is false
}

```

Example:

```java

int y = 3;
if (y % 2 == 0) {
    System.out.println("y is even");
} else {
    System.out.println("y is odd");
}

```

## 3. **`Nested If Statement:`**

Nested `if` statements occur when an `if` or `if-else` statement is placed inside another `if` or `else` block.

```java

if (condition1) {
    // Outer if block
    if (condition2) {
        // Nested if block
        // Code to be executed if both condition1 and condition2 are true
    }
}

```

Example:

```java
int a = 5;
if (a > 0) {
    // Outer if block
    if (a % 2 == 0) {
        // Nested if block
        System.out.println("a is a positive even number");
    } else {
        System.out.println("a is a positive odd number");
    }
}


```

These decision control structures provide the foundation for creating logic that responds to different conditions, allowing for dynamic and flexible program execution.

## **`Switch Statement and Ternary Operator in Java`**

## **`Switch Statement:`**

```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter the mark: ");
        int mark = scanner.nextInt();

        // Using Switch Statement
        System.out.print("Grade (Switch): ");
        switch (mark / 10) {
            case 10:
            case 9:
                System.out.println("A");
                break;
            case 8:
                System.out.println("B");
                break;
            case 7:
                System.out.println("C");
                break;
            case 6:
                System.out.println("D");
                break;
            default:
                System.out.println("F");
        }

        // Close the scanner
        scanner.close();
    }
}

```

## **`Ternary Operator:`**


```java

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter the mark: ");
        int mark = scanner.nextInt();

        // Using Ternary Operator
        System.out.print("Grade (Ternary): ");
        char grade = (mark >= 90) ? 'A' :
                     (mark >= 80) ? 'B' :
                     (mark >= 70) ? 'C' :
                     (mark >= 60) ? 'D' : 'F';
        System.out.println(grade);

        // Close the scanner
        scanner.close();
    }
}

```

In these examples:

- The **`Switch Statement`** is used to evaluate the grade based on the value of mark divided by 10.
- **`The Ternary Operator`** is used to achieve the same result, providing a concise way to express conditional operations.

