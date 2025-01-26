# ActionScript 3 Null Object Reference Bug

This repository demonstrates a common ActionScript 3 error: the `Null Object Reference` error.  This occurs when code attempts to access a property or method of an object that is currently `null`.  This often happens in asynchronous operations or when object initialization is not properly handled.

The `bug.as` file contains code that reproduces the error. The `bugSolution.as` file provides a solution.

## How to Reproduce

1.  Compile and run `bug.as`. Observe the error message.
2. Review the corrected code in `bugSolution.as` to understand the fix.

## Solution

The solution involves checking for `null` before accessing object properties.  This can be done using an `if` statement or conditional operator, ensuring that the object is initialized before any property access. For asynchronous operations, ensure the operation is complete (e.g., using events) before processing the data.