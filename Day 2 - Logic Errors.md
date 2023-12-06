# **`Logic Errors in Java`**

Logic errors, also known as semantic errors, occur when there is a flaw in the algorithm or logic of a Java program. Unlike syntax errors (compile-time errors) and runtime errors, logic errors do not cause the program to terminate or display error messages. Instead, they lead to incorrect or unexpected results due to a mistake in the program's design or flow.

## **`Examples of Logic Errors:`**

## 1. **`Incorrect Algorithm:`**

```java
   public class Example {
       public static void main(String[] args) {
           int result = addNumbers(5, 7);
           System.out.println("The sum is: " + result);
       }
       
       static int addNumbers(int a, int b) {
           // Incorrect addition algorithm
           return a - b;
       }
   }
```

- **`Error:`** The addNumbers method has an incorrect algorithm, resulting in the wrong sum.
