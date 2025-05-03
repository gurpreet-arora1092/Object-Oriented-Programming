
## Pass By Value & Pass By Reference
In computer programming, "pass-by-value" and "pass-by-reference"  refer to how arguments are passed to functions. Pass-by-value creates a copy of the argument, so changes inside the function don't affect the original. Pass-by-reference passes the argument's memory address, allowing changes inside the function to affect the original.

**Pass-by-Value:**

-   A copy of the argument's value is created and passed to the function.
-   The function works with this copy, and any modifications made to the argument within the function do not affect the original value outside the function.
-   This ensures the original variable remains unchanged and provides predictability.
-   Example: In Java, if you pass a primitive data type like an integer to a function, the function receives a copy, and any changes made within the function will not alter the original integer

**Pass-by-Reference:**
-   The function receives a reference (or pointer) to the original argument's memory location.
-   Changes made to the argument within the function are reflected in the original variable.
-   This allows functions to modify the original variable's value directly.

When to Use:
-   **Pass-by-Value:**
    Use when you want to prevent changes to the original variable and maintain its original value within the calling code.
-   **Pass-by-Reference:**
    Use when you want to allow the function to modify the original variable, such as for swapping values or updating data structures




**
