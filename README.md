This project implements a binary adder and display system written entirely in ARM assembly for a Cortex-M4 microcontroller. Two decimal values are read from hardware switches, validated 
in software, added together, and displayed on a seven-segment LED interface. The program handles both valid and invalid inputs, displaying results normally for sums between 0–9 and 
switching to a decimal-point mode for sums between 10–18, with additional error handling for invalid switch configurations.

The program directly configures GPIO ports and peripheral registers, demonstrating low-level control of hardware without the use of high-level libraries. Switch inputs are read from 
PORTC, decoded bit-by-bit, and converted into two numeric operands. The sum is computed in assembly and mapped to the appropriate seven-segment display pattern using lookup tables stored
in ROM. The project emphasizes careful bit manipulation, register-level programming, validation logic, and structured control flow in assembly, highlighting an understanding
of embedded systems fundamentals and hardware-software interaction.
