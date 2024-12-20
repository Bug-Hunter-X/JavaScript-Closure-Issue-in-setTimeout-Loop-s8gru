# JavaScript Closure Issue in setTimeout Loop

This repository demonstrates a common JavaScript closure issue that occurs when using `setTimeout` within a loop.  The problem lies in how the closure captures the variable `i`.  The solution shows how to properly capture the value of `i` at each iteration using an immediately invoked function expression (IIFE). 

## Bug
The `bug.js` file contains a function that uses a loop and `setTimeout` to log numbers from 0 to 9.  Due to the closure issue, it incorrectly logs 10 ten times.

## Solution
The `bugSolution.js` file demonstrates how to resolve the issue using an IIFE to create a new scope for each iteration of the loop, thereby capturing the correct value of `i`.