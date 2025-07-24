Use of Bitwise Operators

This C++ program demonstrates bit-level operations on an integer using bitwise operators. It allows the user to:
1. Set a bit at a given position (i.e., change it to 1)
2. Reset a bit at a given position (i.e., change it to 0)
3. The operations are performed on the number a = 57.

Theory:
Bitwise Operators Used:
1. | (OR): Used to set a specific bit to 1.
2. & (AND): Used to reset a specific bit to 0 (combined with bitwise NOT).
3. << (Left Shift): Used to shift bits to the left — creates a mask for the specific bit position.
4. ~ (Bitwise NOT): Inverts all bits — used to create a mask for resetting.

How it Works:
1. Set Bit:
   set = a | (1 << bit_to_be_set);
   This sets the bit at the specified position to 1 without altering other bits.

3. Reset Bit:
reset = a & ~(1 << bit_to_be_reset);
This resets the bit at the specified position to 0, again preserving other bits.

This program is a basic demonstration of low-level binary manipulation.It reinforces understanding of:
1. Bitwise masks
2. Logical operations on binary data
3. Efficient data manipulation without using arrays or extra memory
