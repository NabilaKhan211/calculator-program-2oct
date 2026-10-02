# Simple Calculator (Python)

Veda Technology Python Internship — Level 1, Task 2

A simple Python program that takes two numbers and performs addition, subtraction, multiplication, division and modulus operations.

## Objective
Practice arithmetic operators, input handling, and basic program logic.

## Tools
- Python 3 (no external libraries)

## Features
- Takes two numbers as input
- Separate function for each operation
- Handles division by zero (for both `/` and `%`) without crashing
- Shows all results clearly in one run

## How to Run
```bash
python calculator.py
```
Enter two numbers when asked, and the program prints all five results.

## Approach
Each operation has its own function: `add`, `subtract`, `multiply`, `divide` and `modulus`. The `divide` and `modulus` functions check if the second number is `0` before calculating, and return a message instead of raising an error. The inputs are read with `input()` and converted to `float` so both whole numbers and decimals work.

## Sample Output

**Input: 90 and 10**
```
Enter first number: 90
Enter second number: 10
Addition :  100.0
Subtraction :  80.0
Multiplication :  900.0
Division :  9.0
Modulus :  0.0
```

**Input: 10 and 0 (division by zero case)**
```
Enter first number: 10
Enter second number: 0
Addition :  10.0
Subtraction :  10.0
Multiplication :  0.0
Division :  Cannot divide by zero
Modulus :  Cannot find modulus by zero
```

## Interview Questions

**1. What is the difference between `/` and `//` in Python?**
`/` is true division and always returns a float (`7 / 2 = 3.5`). `//` is floor division and rounds down to the nearest whole number (`7 // 2 = 3`).

**2. What does the modulus operator do?**
`%` returns the remainder after division (`10 % 3 = 1`). It is often used to check even/odd numbers (`n % 2`) or divisibility.

**3. How can you prevent division-by-zero errors?**
Check the divisor before dividing (`if b == 0`), or use `try/except ZeroDivisionError`. This project uses the `if` check.

## Outcome
The program performs all five operations correctly and handles division by zero safely.