# Project 1: The Collatz Sequence

## How the program works
The program contains the following functions:
- `collatz_sequence(n)`: Generates the complete list of numbers from `n` down to 1.
- `steps(n)`: Calculates the number of steps required to reach 1.
- `highest(n)`: Finds the highest number reached in the sequence.
- `longest_start(limit)`: Finds the starting number below `limit` that takes the most time to reach 1.

## Examples of results
- `collatz_sequence(6)` returns `[6, 3, 10, 5, 16, 8, 4, 2, 1]`
- `steps(6)` returns `8` and `highest(6)` returns `16`
- `longest_start(10)` returns `(9, 19)`
- `longest_start(1000)` returns `(871, 178)`

## Answers to the think questions

**1. Why does `steps(1)` return 0?**

If we start at 1, we are already at 1. No transformation is needed. In our code, the sequence list is `[1]`, its length is 1, so `1 - 1 = 0`.

**2. What happens if `n = 0`? Explain why the loop never stops.**
If `n = 0`, the number is even. The rule states that if it is even, we divide it by 2. However, `0 / 2 = 0`. The number remains stuck at 0. The loop's stopping condition `while n != 1:` will always be true (`0 != 1`), which creates an infinite loop. (Note: Our code includes an `if n <= 0: return []` to prevent this crash).