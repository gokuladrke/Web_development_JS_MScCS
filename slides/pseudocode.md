**Representing an Algorithm as a Pseudocode**

The Fibonacci sequence is a series of numbers where the next number is the sum of the two preceding ones, usually starting with 0 and 1. That is, the sequence starts 0, 1, 1, 2, 3, 5, 8, 13, 21, 34, and so on.

Here's a step-by-step algorithm for generating the Fibonacci sequence:

1. Set up two variables, a and b, to keep track of the current and next numbers in the sequence.
2. Initialize a to 0 and b to 1.
3. Add the two numbers a and b to get the next number in the sequence.
4. Set the new number as b and previous b value as a.
5. Repeat steps 3 and 4, for a pre-determined number of times or until you reach the desired number in the sequence.

If you are to return the nth fibonacci number then in that case you will repeat steps 3 and 4 for n times. Also, the series here starts from 1 but some starts it from 0.

Here's an implementation of the above algorithm for the first `n` numbers in the Fibonacci sequence in Pseudocode:

```python
function fibonacci(n):
    if n <= 1
        return n

    init a to 0
    init b to 1
    init i to 1

    while i < n
        init nextTerm to a + b
        a = b
        b = nextTerm
        increment i

    return nextTerm
```

Step by step algorithm for Fibonacci series using array:

1. Define a function to compute the Fibonacci sequence with an input parameter "n", where "n" is the number of terms of the sequence to be computed.
2. Initialize an array "FibArray" to store the sequence with size n.
3. Set the values of FibArray[0] and FibArray[1] to 0 and 1 respectively, the first two terms of the sequence.
4. For i from 2 to "n" (inclusive):
   i. FibArray[i] = FibArray[i-1] + FibArray[i-2].
5. Return FibArray

Pseudo-code for Fibonacci series using array:

```python
FIBONACCI(n)
    FibArray[0] <- 0
    FibArray[1] <- 1
    for i <- 2 to i <= n
        FibArray[i] <- FibArray[i-1] + FibArray[i-2]
    return FibArray
```

You can return the last element of the array if you just need the nth fibonacci number or return the entire array if you need whole series.
