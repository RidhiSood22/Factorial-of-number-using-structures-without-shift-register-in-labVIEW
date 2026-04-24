# Factorial-of-number-using-structures-without-shift-register-in-labVIEW
Factorial of a Number Using Structure (Without Shift Register) in LabVIEW
# Overview

This project demonstrates how to calculate the factorial of a number in LabVIEW using control structures (such as a For Loop) without using shift registers. It is designed as a simple educational experiment to understand iterative logic and data flow in LabVIEW.

# Objective

To compute the factorial of a given integer using LabVIEW structures without implementing shift registers.

# Theory

The factorial of a non-negative integer n is defined as:

n!=n×(n−1)×(n−2)×⋯×1

Special case:

0!=1

In LabVIEW, factorial can be implemented using:

For Loop for iteration
Multiplication logic inside the loop
Feedback node or tunnel-based accumulation instead of shift registers
 #  Implementation Details
 # Components Used
Numeric Control (Input: number n)
Numeric Indicator (Output: factorial result)
For Loop
Multiplication function
Loop tunnel / feedback node (instead of shift register)
#  Working Principle
The user inputs a number n.
A For Loop runs n times.
Each iteration multiplies the current value with the iteration index.
The result is accumulated using a tunnel or feedback node.
Final output gives the factorial of the input number.
#  Procedure
Open LabVIEW.
Create a new VI (Virtual Instrument).
Add:
Numeric control for input
Numeric indicator for output
Place a For Loop on the block diagram.
Wire the input n to the loop count.
Inside the loop:
Use multiplication to compute factorial step-by-step
Use a tunnel or feedback node to store intermediate values
Connect the final result to the output indicator.
Run the VI and test with different values.
#  Precautions
Ensure the input number is non-negative.
Large inputs may cause overflow due to factorial growth.
Avoid using shift registers as per project constraints.
Verify loop iteration count is correctly wired.
# Output
The VI correctly computes factorial values.
Example:
Input: 5 → Output: 120
Input: 0 → Output: 1
