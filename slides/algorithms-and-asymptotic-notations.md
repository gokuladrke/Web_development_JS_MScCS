# What is an Algorithm? Asymptotic Notations and its Types

**Algorithms:**

- An algorithm is a well-defined computational procedure that takes some value, or set of values, as input and produces some value, or set of values, as output.
- The goal of an algorithm is to solve a specific problem, and it can be implemented in any programming language.
- It's very much necessary to balance the time complexity and space complexity when implementing algorithms as it directly impacts the performance of the code.

**Analysis of Algorithms:**

- The analysis of algorithms involves determining the amount of resources (time and space) needed to solve a problem using a specific algorithm.
- By evaluating and comparing the performance of different algorithms, we can choose the most efficient one for our needs.
- The process of analyzing an algorithm involves counting the number of basic operations performed, measuring the time taken to execute, and calculating the space (memory) used.
- The aim is to balance the space and time complexity of the algorithm. Time-complexity is evaluated by counting the number of basic operations and this is dependent on the size of the input, space complexity is the amount of memory needed to execute the program, this also depends on the size of the input.
- A common way to measure the performance of an algorithm is by using Big O notation, which describes the upper bound on the growth rate of the algorithm's time or space complexity.
- O(n) is linear time, meaning the time it takes to solve the problem increases linearly with the size of the input. O(log n) is logarithmic time, meaning it takes longer to solve larger inputs, but it grows more slowly than linear time.

In conclusion, the analysis of algorithms is important to ensuring that our programs run as efficiently as possible. It's a way to evaluate and compare the performance of algorithms in terms of time and space, so we can choose the best one for our needs. The Big O notation is a widely used notation used to calculate the upper bound of execution time and memory consumed.

**Asymptotic Notations**

The asymptotic notation is used to describe the performance or complexity of an algorithm. It describes the behavior of the function for large input sizes. The Three types of Asymptotic Notations are as follows.

Theta notation (θ): which gives asymptotically tight bounds of an algorithm's growth rate.

Big O notation (O): describes the upper bound of an algorithm's growth rate, used to describe the worst case scenario of an algorithm.

Omega notation (Ω): describes the lower bound of an algorithm's growth rate, used to describe the best case scenario of an algorithm.

It is important to find ways to measure the efficiency of an algorithm because faster algorithms make it possible to process larger amounts of data in less time.

**Java Examples**

1. Theta notation (θ):

The theta notation gives the asymptotic tight bound i.e it gives both the upper and lower bound of a function.

```java
// The time complexity of the following function is Theta(n)
public static void print(int n) {
    for (int i = 0; i < n; i++) {
        System.out.println(i);
        }
    for(int j = n; j>=0; j--){
         System.out.println(j);
    }
}
```

In the example, our function is doing two loops with n iterations each. Therefore, the total function has a running time of 2\*n which goes to Theta(n).

Another Example:

```java
// Time complexity is Theta(n^2)
public static void printPairs(int[] arr) {
    for (int i = 0; i < arr.length; i++) {
        for (int j = 0; j < arr.length; j++) {
            System.out.println(arr[i] + ", " + arr[j]);
        }
    }
}
```

In this example, we have a nested loop that runs n^2 times. Hence the time complexity of the function would be Theta(n^2).

2.Big O notation (O):

The time complexity of the following function is O(n).

```java
// The time complexity of the following function is O(n)
 public static int sum(int[] arr) {
    int sum = 0;
    for (int i = 0; i < arr.length; i++) {
        sum += arr[i];
    }
    return sum;
}
```

The O(n) represents the upper bound limit of the function. That means the function will take at most O(n) time for best or worst case for large inputs. In the example to get the sum of n elements of the array we have to traverse the whole array atleast once. Thats why it is O(n).

Another Example:

```java
// Time complexity is O(n^2)
public static void printSubset(int[] arr) {
    for (int i = 0; i < arr.length; i++) {
        for (int j = i; j < arr.length; j++) {
            for (int k = i; k <= j; k++) {
                System.out.print(arr[k]+", ");
            }
            System.out.println();
        }
    }
}
```

In this example, depending on the different sizes of the inputs, the running time of the algorithm will vary but for worst-case and sufficient inputs, the running time will be around n^2. Hence, the upper bound limit of the function is O(n^2).

3.Omega notation (Ω):

The Omega notation represents the lower bound of the function.

```java
// Find if the element is present in an array.
public static boolean isPresent(int[] arr, int x) {
    for (int i = 0; i < arr.length; i++) {
        if (arr[i] == x) {
            return true;
        }
    }
    return false;
}
```

The time complexity for the algorithm is Omega(1). Because the best case is when we have the element we are searching for is at the beginning of the array. So it requires only one step to search. The worst-case scenario would be O(n) when the element we are searching for is not in the array or it is present at the last.

Another Example:

```java

public static void foo(int n)
{
   int i = 0;
   while(i<n){
        i++;
   }
   if (n > 0)
   {
        for (i= 1; i<=n; i++)
             System.out.println("some text");
   }

}
```

Here, the for loop inside the if condition runs for n times. However, the while loop has a termination condition that depends on the input, however for n>0, the for loop runs for n times itself. So the output is always larger than or equal to n. Hence the time complexity can be denoted as Omega(n).

**Asymptotic Notations Explained in a single Code Example**

A single code snippet can have all three asymptotic notations depending on the situation you're looking at.

Here's an example:

```java
public static int findElement(int[] arr, int x) {
    for (int i = 0; i < arr.length; i++) {
        if (arr[i] == x)
            return i;
    }
    return -1;
}
```

The function finds an element in an array and returns its index. If the element is not found it returns -1.

We can represent this function in terms of all three asymptotic notations:

- The best-case scenario is when the element is found at the first index in the array, in which case the function would only run for 1 iteration, so the lower bound of the function would be Ω(1).
- The average case scenario is when the element is found somewhere in the middle of the array, it would take around n/2 iteration so we can represent as θ(n).
- The worst-case scenario is when the element is either not in the array or it is the last element of the array. Then it would take n iterations so the upper bound of the function would be O(n).

So the same function can be represented using three different notations based on best case, average case, and worst case scenarios. But it is not always the case, sometimes we can't get the tight bound, so at that point we won't have theta notation.
