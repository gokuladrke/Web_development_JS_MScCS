## Problem Statement

Write a Java program to reverse a string using Recursion

## Algorithm

1. Create a function 'reverseString' which takes following arguments:

- `str` , a string - The input string.
- an empty string
- `startIndex`, an integer - The starting index of `str`.
- `endIndex`, an integer - The ending index of `str`.

2. Check Base Case : If the `startIndex` is greater than or equal to `endIndex`, terminates and returns the empty string as output.

3. Recursively invoke the function `reverseString` passing following parameters :

- received string as `str`
- the empty string appended with the value in the received string at the index endindex from previous recursive call
- `startIndex`
- `endIndex - 1`, for moving to next character to reverse in each recursive call.

4. After the termination of recursion, return the resulting string .
