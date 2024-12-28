# MongoDB $inc Operator with String Value

This repository demonstrates an uncommon bug related to the usage of the `$inc` operator in MongoDB update queries.  The bug arises from providing a string value instead of a numeric value to the `$inc` operator.

## Bug Description
The `$inc` operator in MongoDB is designed to increment a numeric field by a specified value. If a string value is provided instead of a number, the update operation might not work as expected, or it may even cause errors.  This subtle mistake can be difficult to track down.

## Solution
The solution is to ensure that the value you pass to `$inc` is a number, not a string. 
