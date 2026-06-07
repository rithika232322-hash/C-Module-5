# 🔁 Recursion: (Factorial) Calculator in C

## 🎯 Aim

To write a C program to calculate the product (factorial) of a given natural number using recursion.

## 🧠 Algorithm

1. **Define** a function `find_factorial(int n)` that recursively calculates the factorial.
2. **Check** if `n == 0`, return `1` (base case, since 0! = 1).
3. **Otherwise**, return `n * find_factorial(n - 1)`.
4. In `main()`:
   - **Read** an integer `num` from the user.
   - **Call** `find_factorial(num)` and store the result in `fact`.
   - **Print** the result.

## Program
#include <stdio.h>

// Function to calculate factorial recursively
int find_factorial(int n) {
    // Base case: 0! = 1
    if (n == 0) {
        return 1;
    }
    // Recursive case: n * (n - 1)!
    else {
        return n * find_factorial(n - 1);
    }
}

int main() {
    int num, fact;

    printf("Enter a natural number: ");
    scanf("%d", &num);

    // Check for negative input handles edge cases outside natural numbers
    if (num < 0) {
        printf("Factorial is not defined for negative numbers.\n");
    } else {
        // Call the recursive function
        fact = find_factorial(num);
        printf("The factorial of %d is: %d\n", num, fact);
    }

    return 0;
}

## Output
Enter a natural number: 5
The factorial of 5 is: 120

## Result
The C program to calculate the factorial of a given natural number using recursion was successfully implemented, compiled, and verified with the expected output.
