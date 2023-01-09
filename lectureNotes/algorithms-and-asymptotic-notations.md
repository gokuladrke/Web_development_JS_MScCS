# Algorithms and Asymptotic Notations

**What is an Algorithm?**
An algorithm is a sequence of well-defined steps or instructions that solve a specific problem.

**Asymptotic Notations**
The efficiency of an algorithm is measured by the Asymptotic notation which is nothing but a symbolic representation of the complexity of a certain algorithm for largeinput. It describes the behavior of the function for large input sizes. It is important to understand the asymptotic notation to measure the efficiency of an algorithm because faster algorithms make it possible to process larger amounts of data in a given time.

**Types of Asymptotic Notations**

There are three types of asymptotic notation:

1. `Theta notation (θ)`: which gives the average case scenanrio of an algorithm's growth rate. Both the best case and worst case.

2. `Big O notation (O)`: describes the upper bound of an algorithm's growth rate, used to describe the worst case scenario of an algorithm.

3. `Omega notation (Ω)`: describes the lower bound of an algorithm's growth rate, used to describe the best case scenario of an algorithm.

> For example, if the number of steps required by an algorithm is n, then its time complexity is represented by the big O notation as O(n), which means the algorithm's performance is directly proportional to the input size n. (Its a linear function)

**Summary**

In the Asymptotic Notations where you have a function g(n) which is representing the number of steps in a problem of size n. So the Asymptotic notations can be expressed as.

Theta notation:

Here, the function g(n) is bound from above and below by constant multiples of n. It means the value of g(n) lies between c1*n and c2*n for large n, where c1 and c2 are any arbitrary positive constant.

Big O notation:

Here, the function g(n) is bound from above by constant multiple of n. It means value of g(n) lies below c\*n for large n, where c is any arbitrary positive constant.

Omega notation:

It's the other way around of big O. Here the function g(n) is bound from below by the constant multiple of n. It means the value of g(n) always lies above c\*n.
Therefore, Asymptotic Notation is the way of analysing the behavior of a function for asymptotically large input i.e. as n increases, how the function behaves.

**Asymptotic notations in detail, with examples.**

Theta notation (θ):

- The theta notation gives us a tight bound on the function. This means that the function is upper-bounded and lower-bounded by constants.

- The theta notation is used to denote the average case performance of an algorithm.

- We can use the theta notation when the algorithm is sure to take time between two constants multiplied with same order of growth in relation for different size of inputs.

```java
// Time complexity of the following function is Theta(n)
public static void function(int n) {
    for (int i = 0; i < n; i++) {
        System.out.println(i);
    }
    for(int i = 0; i < n; i++) {
        System.out.println(i);
    }
}
```

In the example, our function is doing two loops with n iterations each. Therefore, the total function has a running time of 2\*n which is not dependent on the value of n. Hence, it comes under theta(n).

Big O notation (O):

- The big O notation gives us the upper bound limit of the function.
- It is the most commonly used notation because we are more interested in the worst-case run time of an algorithm. This helps us to optimize the performance of the algorithm.

```java
// Time complexity is O(n^3)
    public static void function(int n) {
        for(int i=0;i<n;i++){
            for(int j=0;j<n;j++){
                for(int k=0;k<n;k++){
                    System.out.println(i);
                }
            }
        }
    }
```

The above code will give us the time complexity of O(n^3). This is derived from the three nested loops, which each run n times. Thus, the worst-case time complexity is O(n^3). Even if we add one more loop outside these loops that run for n iterations then also the time complexity will be O(n^3) because O(n\*n^3) equals O(n^4) and the highest order term n^4 is considered as the worst-case.

Omega notation (Ω):

- Representing with the help of Omega notation comes in handy when best case and worst case times differ significantly.
- As discussed, it represents the lower bound of the running time.
- Not commonly used, except in the analysis of sorting algorithms.

```java
public static int getMax(int[] arr)
{
    if(arr.length == 0) return -1;
    int max = Integer.MIN_VALUE;
    for(int i=0;i<arr.length;i++){
        if(arr[i]>max){
            max = arr[i];
        }
    }
    return max;
}
```

The function above finds the max element in an array. The function is looping through the entire array once and checking each element. Here the best case doesn't vary because for an array with n elements it will run n times no matter what the value of n is. So we can say that the best case is Ω(n).

We can also represent the minimal running time of the function by using Omega(n) i.e let's say we have a function that takes n^3 time. We can represent it as Omega(logn) because the time will always be greater than or equal to logn no matter how small or large the input n is.

In general, Theta notation depicts both upper and lower bounds of the time taken by the algorithm, Big O notation depicts the upper bound or worst case time taken by the algorithm and Omega notation depicts the lower bound or best case time taken by the algorithm.

**Additional Examples**

Theta Notation(Θ):

```java
// Time complexity of the following function is Theta(n)
public static void function(int n) {
    int k=0; //Constant time operation
    for (int i = 0; i < n; i++) {
        System.out.println(i);
         k++; //constant time operation
    }
}
```

In this example, the function is doing the loop with n iterations. Therefore, we can consider the total function has a running time of theta(n).

```java
// Time complexity of the following function is Theta(n^2)
public static void function(int n) {
    for(int i=0;i<n;i++){
        for(int j=0;j<n;j++){
            System.out.println(i);
        }
    }
}
```

Here, we have two nested for loops running with n and n iterations respectively. Therefore the total running time would be n\*n = n^2. So, the time complexity will be Theta(n^2)

Big O notation (O):

```java
// Time complexity of the following function is O(1)
public static void function(int n) {
    System.out.println(n);
}
```

In this example, there is only one operation performed inside the function, which is independent of the input n. So the time complexity is O(1).

```java
// Time complexity of the following function is O(log(n))
public static void function(int n) {
    for (int i = 1; i < n; i = i*2)
        System.out.println("Hello World");
}
```

Here, we have a single loop but, in each iteration, i is multiplying by 2. So, the number of times it will run is equal to log(n). So the time complexity is O(log(n)).

Omega notation (Ω):

```java
// Time complexity of the following function is Omega(1)
public static void function(int n) {
    System.out.println(n);
}
```

The function has only one operation that is independent of the input n. So the best case will be omega(1).

```java
// Time complexity of the following function is Omega(log(n))
public static void function(int n) {
    for (int i = n; i > 0; i /= 2)
        System.out.println("Hello World");
}
```

In the last example of Omega notation, we have a single loop in which each time i is dividing by 2. So, the number of times it will run would be log(n). So the best case will be Ω(log(n)).
