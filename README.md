# JavaScript Null Handling Bug

This repository demonstrates a common, yet subtle, bug in JavaScript related to handling `null` values in arithmetic operations.  The `foo` function intends to safely handle cases where either `a` or `b` might be `null` by returning 0, but the approach has unintended consequences for arithmetic operations.

## Bug Description

The core issue lies in how JavaScript handles `null` in addition. While the null check prevents direct errors, it masks the fact that the addition operation may result in an unexpected value. The solution ensures that null values are correctly handled in addition operations, preventing this type of subtle error from occurring in various code scenarios.

## How to Reproduce

1. Clone this repository.
2. Open `bug.js` and run the code.
3. Observe the output which may be unanticipated. Then open and execute the `bugSolution.js` file and compare the results.