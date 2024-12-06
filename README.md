# Incorrect use of $inc operator in MongoDB update query
This example demonstrates an uncommon error in MongoDB queries related to the `$inc` operator. The `$inc` operator is used to increment a numeric field. However, if a string value is provided instead of a number, the operation might fail or produce unexpected results.

## Bug
The bug involves providing a string value ('1' instead of 1) to the `$inc` operator. This leads to an error or incorrect result because `$inc` expects a numeric value.

## Solution
The solution involves ensuring that a numeric value is provided to the `$inc` operator. Correcting the code to use the numeric value `1` instead of the string '1' resolves the issue.