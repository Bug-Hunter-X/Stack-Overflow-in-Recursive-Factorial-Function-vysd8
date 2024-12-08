# Hack Bug: Stack Overflow in Recursive Factorial Function

This repository demonstrates a common bug in recursive functions written in Hack: a stack overflow error caused by improper handling of base cases. The `foo` function calculates the factorial of a number recursively.  However, it lacks a base case to handle negative input, causing infinite recursion.

The `bug.hack` file contains the buggy code. The `bugSolution.hack` file shows the corrected code, addressing the base case for negative inputs, thus preventing stack overflow.

## Bug Description

The factorial function fails to handle negative input gracefully.  When a negative number is provided, the recursive calls continue indefinitely, eventually exceeding the stack limit and resulting in a stack overflow.

## Solution

The solution introduces a check for negative input at the beginning of the function. If the input is negative, the function returns an appropriate value (like -1 in this case to indicate an error), preventing the infinite recursion and the stack overflow.
