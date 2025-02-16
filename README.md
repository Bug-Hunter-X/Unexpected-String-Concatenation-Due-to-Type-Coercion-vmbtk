# Unexpected String Concatenation in JavaScript

This repository demonstrates a common, yet subtle, JavaScript bug related to type coercion.  The `foo` function intends to add two numbers, but due to the implicit type conversion of JavaScript, it instead concatenates the number and string.

## Bug
The bug lies in the `foo` function's lack of explicit type checking.  It assumes both inputs are numbers, leading to unexpected behavior when a string is passed as an argument.

## Solution
The solution involves explicitly checking the types of the inputs or using a method that handles different data types gracefully (e.g., `parseInt` to convert strings to numbers).