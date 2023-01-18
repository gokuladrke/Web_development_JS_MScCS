## Problem Statement

Write a Java program to find the second highest number in an array.

## Algorithm

1. Initialize two variables, one for the maximum value and one for the second highest value, with the minimum possible value of the data type used. (example: int max= Integer.MIN_VALUE, secMax = Integer.MIN_VALUE etc)

2. Traverse the array in a loop starting at the beginning.

3. For each element of the array, compare it with the value stored in the maximum value variable.
   a) if the value is greater than maximum variable , then update the sec_max by assigning the current max before update the current Maximum value variable with the current value of the element.
   b) if the value is not greater than max, yet greater than secondMax, then update the secondMax with current value.

4. After the loop finishes, the second highest value variable passed with updated with second highest value

5. check if we know if such secMax exist in the array if yes we print that values otherwise print not found to add one more contion

6. Print the value of the second highest value found in the array.
