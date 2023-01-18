## Problem Statement

Write a Java program to find the factorial of a given number using Recursion

## Algorithm

1. Start by validating the input, if a no is less than '0', return an error message "Invalid Number".

2. Declare a function 'factorial' that takes an integer 'n' as input. Inside the function check for the base case
   a. If the value of 'n' is '0' , return 1.
   b. If value of 'n' is 1, then the factorial should be 1 so return 'n'

3. If it is not the base case, make a recursive call to the function 'factorial' which evaluates as follows: multiply the number n to the factorial value of 'n-1'. The factorial value of 'n-1' is determined by calling the function factorial recursively , passing 'n-1' as argument.

4. Repeat step 3 by decrementing value of passed variable with each resursive call until it reaches 0 or 1 where base case returns and recursive calls are over.
5. Before calling this `factorial` function do make sure to check if data input is valid, if it's not throw an exception if possible.

6. Once you have returned from the final recursion, the return result should have evaluated the factorial. Return that value

7. .At the end print result by calling factorial function with the value for which factorial is to be calculated.
