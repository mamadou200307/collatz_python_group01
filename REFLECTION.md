# Project Reflection

## Work distribution (Who did what?)
- **TOURE MAMADOU**: Implementation of Task 1  (`collatz_sequence`) Writing the README.
- **NUHU WASINDA BASSI**: Implementation of Task 2 (`steps` and `highest`).
- **OMAR MBAYE**: Implementation of Task 3 (`longest_start`).
- SAMBIANI SOUGLEMAN ESTHER: Completion of the optional challenge and testing.
- **MARIAMA BA**:  The reflection explanations.

## Bugs encountered and how we fixed them

**Bug 1 ,TOURE MAMADOU: The division issue**
At first, i used `/` instead of `//` to divide even numbers. In Python 3, `6 / 2` gives `3.0` (a decimal number), which broke the logic for the next steps. i fixed this by using `n = n // 2` (integer division).
To link the project and upload it to GitHub, I accessed the terminal on my computer and followed the procedure outlined in the Python course, specifically in the lesson "Lab_linux_Git_GitHub.ipynb."

**Bug 2,NUHU WASINDA BASSI: "NameError" issue**
i tried to test the `highest()` function before running the cell that contained `collatz_sequence()`. Python did not recognize the function. i learned that we must always execute the function definitions before using them.

**Bug 3, MARIAMA BA: Crashing with 0**
When i tested with n = 0, the program ran infinitely. i added an if n <= 0: condition at the beginning of collatz_sequence to prevent this. 

**Bug 4,SAMBIANI SOUGLEMAN ESTHER** (Optional Challenge & Testing): 
  Work: Modified the rule to 5*n + 1 and handled the 100-step limit. Tested the "n=0" case.
  Bug encountered: When testing n = 0, the program caused an infinite loop and froze our Google Colab notebook because 0 / 2 is always 0.

**Beg 5, OMAR MBAYE**   I put return (best_start, max_steps) inside the for loop. The function stopped at the first number (1) and returned (1, 0) immediately.

