# MongoDB $inc operator error with non-numeric value
This repository demonstrates an error that occurs when using the `$inc` operator in MongoDB with a non-numeric value.  The `$inc` operator is designed to increment a numeric field, attempting to use it with a string or other non-numeric value will result in an error.  The solution provided shows how to correctly use the `$inc` operator.

## Bug Description
The provided code snippet shows an incorrect usage of the `$inc` operator, leading to an error when the update operation is executed.  The error message will indicate a type mismatch or an invalid operation.

## Solution
The solution involves ensuring that the value passed to `$inc` is a valid number.  Avoid using strings or other non-numeric values. If the field needs to be initialized or updated with non-numeric values before incrementing, a separate update should be performed first.