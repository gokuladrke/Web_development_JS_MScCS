### Arrays

An **array** is a fundamental data structure in many programming languages, including Java. It is a collection of variables of the same type, called elements, that are stored in a contiguous block of memory. Arrays have a fixed size and cannot be resized once created.

Array elements are accessed using an integer index, which starts at 0 and goes up to one less than the number of elements in the array.

Here is an example of declaring and initializing an array with 5 elements :

```java
int[] myArray = new int[5];
```

You can also initialize and declare the array with the elements like this;

```java
int[] myArray = {1,2,3,4,5};
```

You can modify and access the elements of an array using their index like this;

```java
myArray[0] = 20;
int x = myArray[1];
```

Java also provides a useful property `length` that can be used to find the length of the array like this;

```java
int length = myArray.length;
```
