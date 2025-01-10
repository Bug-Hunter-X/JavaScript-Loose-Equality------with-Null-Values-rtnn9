# JavaScript Loose Equality with Null Values

This repository demonstrates a common error in JavaScript related to loose equality (==) when checking for null values.

## The Problem
The provided `bug.js` file contains a function that uses loose equality (`==`) to check for null values before performing an addition. This approach can lead to unexpected results because loose equality performs type coercion, which might lead to unexpected true results when compared to null.

## The Solution
The `bugSolution.js` file corrects the issue by using strict equality (`===`). Strict equality checks for both value and type equality, preventing this type of unexpected behavior.

## How to reproduce
1. Clone the repository.
2. Run `bug.js` and note the output.
3. Run `bugSolution.js` and compare the output. 

## Learning Points
- Always use strict equality (`===`) when comparing values to `null` in JavaScript to avoid unexpected behavior due to type coercion. 
- Understanding the difference between loose and strict equality is crucial for writing reliable and bug-free JavaScript code.