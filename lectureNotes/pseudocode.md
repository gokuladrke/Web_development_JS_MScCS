# Problem Solving

## Problem Statement

Given a number 'n', print the first 'n' fibonacci numbers.

For example:

if the input is n = 5

the output has to be:

0 1 1 2 3

## Written Algorithm (Steps)

```python
1. get the number from the user -> n

2. set the first variable to a value 0

3. set the second variable to a value 1

4. iteratively repeat for 'n' times the following steps:

    - find the third number -> set it to third

    - print the third number

    - change the values of first and second
```

## Pseudocode:

```python
Program:

Input: N

0. Initialize first and second numbers for Fibonacci sequence, FirstNumber=0, SecondNumber=1
1. Read N from user
2. if N == 1, Print FirstNumber
3. if N == 2 Print FirstNumber  " " SecondNumber
4. if N >= 3
         Print FirstNumber   " " SecondNumber
         i = 0
         Repeat
	     ThirdNumber <- FirstNumber + SecondNumber
	     Print  ThirdNumber
	     FirstNumber <- SecondNumber
	     SecondNumber <- ThirdNumber
	     i<-i+1
         Until i >= N-2

5.End Program
```

## Java Implementation

```java
import java.util.*;

class Fibonacci {
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);

        // your logic goes here

        // 1. get the number from the user -> n
        int n = in.nextInt();

        // 2. set the first variable to a value 0
        int firstNumber = 0;

        // 3. set the second variable to a value 1
        int secondNumber = 1;

        if (n == 1) {
            System.out.print(firstNumber + " ");
        } else if (n == 2) {
            System.out.print(firstNumber + " " + secondNumber + " ");
        } else if (n >= 3) {
            System.out.print(firstNumber + " " + secondNumber + " ");
            // 4. iteratively repeat for 'n' times
            for (int i = 0; i < n - 2; i++) {
                // 5. find the third number -> set it to third
                int thirdNumber = firstNumber + secondNumber;

                // 6. print the third number
                System.out.print(thirdNumber + " ");

                // 7. change the values of first and second
                firstNumber = secondNumber;
                secondNumber = thirdNumber;
            }
        }
        in.close();
    }
}
```
