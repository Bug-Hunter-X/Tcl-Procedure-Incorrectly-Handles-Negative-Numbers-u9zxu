# Tcl Procedure Bug: Incorrect Negative Number Handling

This repository demonstrates a bug in a simple Tcl procedure that incorrectly handles negative numbers. The procedure is intended to return different strings depending on whether the input number is greater than 10 or not. However, it fails to handle negative numbers correctly, resulting in unexpected output.

## Bug Description

The `buggyProc` procedure uses an `if` statement to check if the input `x` is greater than 10.  It correctly handles numbers greater than 10, but incorrectly classifies negative numbers as "Less than or equal to 10".

## Bug Solution

The solution involves modifying the `if` statement to explicitly check for negative numbers before comparing to 10. This ensures correct classification for all input numbers. 

## How to reproduce

1.  Clone this repository.
2.  Run the `bug.tcl` script using a Tcl interpreter. 
3. Note the unexpected result for the negative input.
4. Run the `bugSolution.tcl` script for corrected behaviour. 