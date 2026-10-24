# Project Reflection

## Work distribution (Who did what?)
- TOURE MAMADOU: Implementation of Task 1  (`collatz_sequence`) Writing the README.
- NUHU WASINDA BASSI: Implementation of Task 2 (`steps` and `highest`).
- OMAR MBAYE: Implementation of Task 3 (`longest_start`).
- SAMBIANI SOUGLEMAN ESTHER: Completion of the optional challenge and testing.
- MARIAMA BA:  The reflection explanations.

## Bugs encountered and how we fixed them

**Bug 1: The division issue**
At first, we used `/` instead of `//` to divide even numbers. In Python 3, `6 / 2` gives `3.0` (a decimal number), which broke the logic for the next steps. We fixed this by using `n = n // 2` (integer division).

**Bug 2: "NameError" issue**
We tried to test the `highest()` function before running the cell that contained `collatz_sequence()`. Python did not recognize the function. We learned that we must always execute the function definitions before using them.

