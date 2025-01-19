# TypeScript Bug: Passing Array to String Function

This repository demonstrates a common TypeScript error: passing an array to a function that expects a string argument.  The `greeter` function is designed to accept a string and return a greeting.  However, attempting to pass an array to it results in a runtime error, as TypeScript's type checking doesn't prevent this issue in this particular case. 

The `bug.ts` file contains the erroneous code, while `bugSolution.ts` offers a corrected version.

## How to Reproduce

1. Clone this repository.
2. Compile and run `bug.ts` using a TypeScript compiler (tsc).  You'll observe a runtime error.
3. Examine `bugSolution.ts` to see the correct approach to handling string concatenation when dealing with arrays.

## Solutions

The solution involves checking the type of the input before attempting concatenation, or using template literals for type safety when using arrays.