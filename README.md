# my-calculator
1. Project Introduction
Project Name: Interactive Calculator
Objective: Build a calculator that evaluates arithmetic expressions with basic operators, handles parentheses, and operator precedence.
2. Tools & Concepts Used
Programming Language: C++
Libraries Used:
<iostream>: For input/output.
<stack>: To handle numbers and operators.
<cmath>: For power (^) function.
<cstdlib>: For handling exit commands.
Key C++ Concepts:
Control Structures: If-else, switch-case (for operator logic).
Functions: Modularity through functions like applyOperator() and evaluate().
Stacks: Used for managing numbers and operators to ensure correct precedence.
Error Handling: Division by zero and other invalid input checks.
3. Step-by-Step Process
a. Understanding Input Methods
You started by accepting expressions as strings, but later improved it by adding interactive input (e.g., 3 + 5 * 2).
Initial Version: Direct input like "10 + (20 * 30)".
Improved Version: Broke down inputs interactively for user clarity.
b. Implementing Operators
Supported Operators: +, -, *, /, ^.
Operator Precedence:
Handled through a function precedence() to rank operators.
Highest precedence: ^ (power), followed by *, /, and lowest are + and -.
Switch-Case Logic: Functions like applyOperator() use switch-case to apply operations on two operands.
c. Using Stacks for Evaluation
Stacks were crucial for:
Storing numbers while parsing the expression.
Storing operators until the right precedence/order is found.
Pop and apply: As operators are found, operands are popped and calculations are applied.
d. Error Handling & Edge Cases
Division by Zero: Handled gracefully with an error message.
Empty Expression Handling: Prevents invalid input from being processed.
e. Adding Parentheses Support
You added logic to handle expressions like (3 + 5) * 2 by evaluating parentheses first.
find_last_of(): Used to find and evaluate the innermost expression.
4. Final Version of the Calculator
Key Improvements:
Modular Design: Functions for operators, precedence, and expression evaluation make the code easier to manage and expand.
Interactive Input: Accepts expression from users and evaluates it on the fly.
Error Handling: Division by zero and invalid expressions are managed properly.
