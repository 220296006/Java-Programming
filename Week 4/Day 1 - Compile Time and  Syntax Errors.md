# **`Errors in Java: Compile Time / Syntax Errors`**

In Java, errors can be categorized into different types, and one common category is **`Compile Time or Syntax Errors`**. These errors occur during the compilation of the Java source code and prevent the program from being successfully compiled into bytecode. Compile time errors are typically associated with incorrect syntax, structure, or language rules.

## **`Examples of Compile Time / Syntax Errors:`**

## 1. **`Missing Semicolon:`**

```java
   public class Example {
       public static void main(String[] args) {
           System.out.println("Hello World")
       }
   }
```

- **`Error:`** Missing semicolon after the System.out.println statement.

## 2. **`Unclosed String Literal:`**

```java
public class Example {
    public static void main(String[] args) {
        System.out.println("Hello World);
    }
}
```

- **`Error:`** Unclosed string literal.

## 3. **`Incorrect Method Declaration:`**

```java
public class Example {
    public static void main(String[] args) {
        void myMethod() {
            System.out.println("This is a method");
        }
    }
}
```

- **`Error:`** Incorrect method declaration inside the main method.

## 4. **`Mismatched Data Types:`**

```java
public class Example {
    public static void main(String[] args) {
        int number = "Hello";
    }
}
```

- **`Error:`**  Mismatched data types (int assigned a string value).

## 5. **`Incorrect Variable Declaration:`**

```java
public class Example {
    public static void main(String[] args) {
        int number = 10;
        String message;
        System.out.println(message);
    }
}

```

- **`Error:`**  Variable message might not have been initialized.

## **`Best Practices for Handling Compile Time Errors:`**

### 1. **`Careful Code Review:`**

- Regularly review and analyze your code for syntax errors before attempting compilation.

### 2. **`Use an Integrated Development Environment (IDE):`**

- IDEs often provide real-time error detection, helping you identify and fix syntax errors as you code.

### 3. **`Understand Java Language Rules:`**

- Familiarize yourself with Java language rules, including proper syntax, variable declarations, and method structures.

### 4. **`Follow Coding Standards:`**

- Adhere to coding standards and guidelines to maintain consistent and error-free code.

### 5. **`Utilize Code Linters:`**

- Consider using code linters or static code analysis tools to automatically identify and highlight syntax errors.

## **`Advantages of Addressing Compile Time Errors:`**

### 1. **`Early Detection:`**

- Compile time errors are detected early in the development process, reducing the likelihood of deploying faulty code.

### 2. **`Code Stability:`**

- Resolving syntax errors contributes to code stability and ensures a smoother development process.

### 2. **`Enhanced Readability:`**

- Well-structured and error-free code enhances code readability and maintainability.

Addressing compile time errors is an essential part of the software development process, and by following best practices, developers can create more robust and error-free Java applications.

## **`Runtime Errors in Java`**

Runtime errors, also known as exceptions, occur during the execution of a Java program. Unlike compile time errors, runtime errors are not detected until the program is running. These errors are often caused by unexpected conditions or situations that arise during the execution of the program.

## **`Examples of Runtime Errors:`**

## 1. **`NullPointerException:`**

```java
   public class Example {
       public static void main(String[] args) {
           String message = null;
           System.out.println(message.length());
       }
   }
```

- **`Error:`** Attempting to access the length property of a null object (NullPointerException).

## 2. **`ArithmeticException:`**

```java
public class Example {
    public static void main(String[] args) {
        int result = 10 / 0;
        System.out.println(result);
    }
}
```

- **`Error:`** Division by zero (ArithmeticException).

## 3. **`ArrayIndexOutOfBoundsException:`**

```java
public class Example {
    public static void main(String[] args) {
        int[] numbers = {1, 2, 3};
        System.out.println(numbers[3]);
    }
}
```

- **`Error:`** Accessing an index beyond the bounds of the array (ArrayIndexOutOfBoundsException).

## 4. **`NumberFormatException:`**

```java
public class Example {
    public static void main(String[] args) {
        String value = "abc";
        int number = Integer.parseInt(value);
        System.out.println(number);
    }
}
```

- **`Error:`** Attempting to convert a non-numeric string to an integer (NumberFormatException).

## 5. **`ClassCastException:`**

```java
public class Example {
    public static void main(String[] args) {
        Object object = "Hello";
        Integer number = (Integer) object;
    }
}
```

- **`Error:`** Attempting to cast an object to an incompatible type (ClassCastException).

## **`Best Practices for Handling Runtime Errors:`**

### 1. **`Use Exception Handling:`**

- Implement try-catch blocks to handle exceptions gracefully and provide appropriate error messages.

### 2. **`Validate Input:`**

- Validate user input and external data to prevent unexpected values or conditions.

### 3. **`Check Array Bounds:`**

- Verify array indices before accessing elements to avoid ArrayIndexOutOfBoundsException.

### 4. **`Avoid Division by Zero:`**

- Ensure that division operations are performed with non-zero denominators.

### 5. **`Use Safe Type Casting:`**

- Utilize proper type casting and instanceof checks to prevent ClassCastException.

## **`Advantages of Addressing Runtime Errors:`**

### 1. **`Program Stability:`**

- Handling runtime errors improves the overall stability of the program, preventing abrupt terminations.

### 2. **`Enhanced User Experience:`**

- Graceful handling of exceptions contributes to a better user experience by providing informative error messages.

### 3. **`Debugging and Logging:`**

- Proper exception handling allows developers to log detailed information about errors, aiding in debugging and issue resolution.

Runtime errors are inevitable in complex programs, but addressing them through effective exception handling practices helps create more robust and reliable Java applications.