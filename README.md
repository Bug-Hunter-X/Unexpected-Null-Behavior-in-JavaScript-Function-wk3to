# Unexpected Null Behavior in JavaScript Function

This repository demonstrates a common but subtle bug in JavaScript related to handling null values in a function. The function `foo` is intended to add two numbers, but its behavior is unexpected when one or both of the input values are null.

## Bug Description

The `foo` function does not handle null values correctly. When either `a` or `b` is null, the function returns 0, even if the other value is not null. This can lead to unexpected results and potential errors in applications that rely on this function.

## Solution

The bug is fixed by checking for null values using the strict equality operator (===) and providing a default value or appropriate handling for null inputs. The corrected function handles null values gracefully and provides meaningful results in all cases. The updated function returns the sum of valid numbers while treating null values as zero.