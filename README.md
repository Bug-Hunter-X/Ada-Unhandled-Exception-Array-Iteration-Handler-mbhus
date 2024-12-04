# Uncommon Ada Error: Unhandled Exceptions and Array Iteration

This repository demonstrates an example of a potential issue in Ada programming related to exception handling and array processing.  The `bug.ada` file shows an Ada program that doubles the values in an array. While functional, its exception handling is too broad, potentially masking specific errors. The improved solution is provided in `bugSolution.ada`.

## Bug Description

The original Ada code iterates through an array, doubling each element.  The exception handler (`when others`) is too general. This could mask more specific exceptions, making debugging more difficult.  More precise exception handling improves the robustness of the code.

## Solution

The solution refactors the exception handling to be more specific.  This enables more targeted error handling and more informative diagnostics.