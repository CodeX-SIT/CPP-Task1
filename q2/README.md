# Question 2 — Write the program (data types, scope, input/output)

Objective

Write a complete C++ program in `q2/q2.cpp` that reads user input, uses variables with appropriate types and scope, performs a small computation, and prints the result in the exact format shown in the examples.

What this tests

- Using `std::cin` and `std::cout` for input/output
- Choosing correct data types for inputs and calculations
- Understanding variable scope (local variables inside blocks)

Problem statement

Create a program that:

1. Prompts the user to enter their first name (single word), age (integer), and height in meters (a floating-point number). Prompt texts must match the sample run exactly.
2. Calculates the approximate height in centimeters (height_m \* 100) and stores it in an integer variable `height_cm` (rounded down).
3. Prints a summary exactly in the format shown below.

Input / Output format (sample runs)

Sample run 1 (user input shown after prompts):

```
Enter your first name: Alice
Enter your age: 20
Enter your height in meters: 1.68

Summary:
Name: Alice
Age: 20
Height (m): 1.68
Height (cm): 168
```

Sample run 2:

```
Enter your first name: Bob
Enter your age: 17
Enter your height in meters: 1.55

Summary:
Name: Bob
Age: 17
Height (m): 1.55
Height (cm): 155
```

Requirements and hints

- Use `std::string` for the name, `int` for age, and `double` or `float` for the height in meters.
- After reading the height as a floating-point number (e.g., `double height_m`), compute `int height_cm = static_cast<int>(height_m * 100);` to convert meters to centimeters and drop the fractional part.
- Keep prompts and output formatting identical to the samples (including blank line before "Summary:").

When you finish, compile and run your program and verify it matches the sample runs.
