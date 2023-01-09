---
marp: true
---

# Variables and Data Types

## Variables

---

- In Java, a variable is a named location in memory that can store a value.
- Variables are declared with a specific data type which determines what type of values it can hold.
- Java has two types of data types:
  - Primitive data types
  - User-Defined or Reference data types.

## Primitive and User-Defined

---

## Primitive Data Types

Examples of the primitive data types in Java:

- char : To represent a single character 'a'
- byte : For storing 8-bit integers
- short : For storing 16-bit integers
- int : For storing 32-bit integers
- float : For storing 32-bit floating-point numbers
- double : For storing 64-bit floating-point numbers
- long : For storing 64-bit integers
- boolean : To represent a logical value (true/false)

### Example:

```java
//Declaring a variable
int a;

//Assigning a value to a variable
a = 10;

//Declaring and assigning a value to a variable
double b = 0.5;
```

---

## User-Defined Data Types

Common user-defined data types in Java are:

- Strings : a sequence of characters "hello world",
- Arrays : a contiguous chunk of memory that stores a set of values, [1, 2, 3, 4, 5]
- Enumerations : a set of named constants, also known as enum
- Class : user defined blueprint or prototype from which objects are created.
- Interface : an abstract type that contains a collection of abstract methods and constants.

```java
// Creating an instance of the String

String str = new String("Hello World");
```
