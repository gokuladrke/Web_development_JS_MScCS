### Recursion

A recursive function is a function that calls itself based on a base case and or condition. There are two important concepts in the recursive function:

- The **base case**, which is the condition that causes the function to stop calling itself.
- The **recursive call**, which is the function calling itself with new arguments until the base case is met.

Here's an example of a recursive function that computes the factorial of a number:

```java
public static int factorial(int n) {
    if (n == 0) {
        return 1; // base case
    } else {
        return n * factorial(n-1); // recursive call
    }
}
```

Notice that the base case acts as a "guard" against infinite recursion.

A few points to remember in recursion are :

- Every recursive function must have a valid base case otherwise the function will lead to infinite calling and as a result, the system will run out of stack memory.
- In addition to checking the validity of the base case, always check the arguments passed because it might cause infinite recursion.
- Recursive functions can utilize a lot of stack memory and as a result, the system might run out of stack space for large inputs.
