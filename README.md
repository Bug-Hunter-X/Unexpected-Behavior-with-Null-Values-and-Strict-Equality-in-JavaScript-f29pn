# Unexpected Behavior with Null Values and Strict Equality in JavaScript

This repository demonstrates a common error in JavaScript related to handling null values when using the strict equality operator (===).  The `bug.js` file contains code that produces unexpected results due to this error.  The `bugSolution.js` file provides a corrected version.

## Problem

The initial code uses strict equality (===) to check for null values before performing addition. While this appears correct at first glance, strict equality does not convert types, leading to incorrect results when null is treated as a number. 

## Solution

The corrected code uses a more robust null check, ensuring that null values are handled appropriately.  Alternatively, loose equality (==) could be used, but it is generally recommended to avoid it for clarity and to prevent unexpected type coercion.

## How to run

1. Clone this repository.
2. Open `bug.js` and `bugSolution.js` in a text editor.
3. Run the JavaScript files using your preferred method (e.g., Node.js).
4. Compare the output of both files to see how the corrected code addresses the unexpected behavior.