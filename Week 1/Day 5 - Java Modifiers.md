# **`Java Modifiers`**

## **`Java Identifiers`**

In Java, identifiers are names given to various program elements such as classes, variables, methods, and labels. Identifiers play a crucial role in Java programming as they help in uniquely identifying and referencing these elements.

## **`Rules for Naming Identifiers:`**

1. **`Must Begin with a Letter, Currency Character (`$`), or Underscore (`_`):`**
   - Valid: `variableName`, `_count`, `$total`
   - Invalid: `123value`, `@rate`

2. **`Can Be Followed by Letters, Digits, Currency Characters, or Underscores:`**
   - Valid: `count1`, `totalAmount`, `avg_score`
   - Invalid: `user@name`, `discount%`

3. **`Java Keywords Cannot Be Used:`**
   - Keywords are reserved words in Java and cannot be used as identifiers.
   - Examples: `class`, `int`, `if`, etc.

4. **`Case-Sensitive:`**
   - Java is case-sensitive, meaning `myVariable` and `myvariable` are different identifiers.

5. **`No Spaces or Special Characters (Except Currency Characters and Underscore):`**
   - Spaces, symbols, and special characters (except `$` and `_`) are not allowed in identifiers.
   - Invalid: `user name`, `total#amount`

6. **`Cannot Begin with a Digit:`**
   - Identifiers cannot start with a digit.
   - Invalid: `123total`, `8score`

7. **`Avoid Using Underscore Alone:`**
   - While it's allowed, using a single underscore as an identifier is discouraged.

8. **`Meaningful and Descriptive:`**
   - Choose identifiers that are meaningful and describe the purpose of the element they represent.
   - Good: `totalAmount`, `calculateAverage`
   - Avoid: `x`, `temp`

## Conventions for Naming Identifiers:

1. **Camel Case:**
   - For variables and methods, use camel case (e.g., `myVariable`, `calculateAverage`).

2. **Pascal Case:**
   - For class names, use pascal case (e.g., `MyClass`, `PersonDetails`).

3. **All Uppercase with Underscores (Screaming Snake Case):**
   - For constants, use all uppercase with underscores (e.g., `MAX_VALUE`, `PI`).

Choosing appropriate and consistent identifiers contributes to code readability and maintainability in Java.


Modifiers in Java are keywords that define the scope, visibility, and behavior of classes, methods, and variables. There are two main categories of modifiers: access modifiers and non-access modifiers.

## **`Access Modifiers:`**

### 1. **`Public:`**

- The `public` modifier makes a class, method, or variable accessible to any other class.

```java
   public class MyClass {
       public int myVariable;
       public void myMethod() {
           // Code here
       }
   }
```

### 2. **`Private:`**

- The `private` modifier restricts access to the class, method, or variable to within its own class.

```java
public class MyClass {
    private int myVariable;
    private void myMethod() {
        // Code here
    }
}
```

### 3. **`Protected:`**

- The protected modifier allows access to the class, method, or variable within its own package and by subclasses.

```java
public class MyClass {
    protected int myVariable;
    protected void myMethod() {
        // Code here
    }
}
```

### 4. **`Default (Package-Private):`**

- If no access modifier is specified, it is considered as package-private, allowing access within the same package.

```java
class MyClass {
    int myVariable;
    void myMethod() {
        // Code here
    }
}
```

## **`Non-Access Modifiers:`**

1. **`Static:`**

- The static modifier is used to create class methods and variables that can be accessed without creating an instance of the class.

```java
public class MyClass {
    static int staticVariable;
    static void staticMethod() {
        // Code here
    }
}
```

2. **`Final:`**

- The final modifier is used to make a class, method, or variable unchangeable or non-extendable.

```java
public final class MyClass {
    final int myVariable;
    final void myMethod() {
        // Code here
    }
}
```

3. **`Abstract:`**

- The abstract modifier is used to declare abstract classes and methods.

```java
public abstract class MyAbstractClass {
    abstract void myAbstractMethod();
}
```

4. **`Synchronized:`**

- The synchronized modifier is used to control access to a method or block of code by multiple threads.

```java
public synchronized void myMethod() {
    // Code here
}

```