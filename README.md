# Use of Bitwise Operators in C++

## Program Overview

This C++ program demonstrates **bit-level operations** on an integer using **bitwise operators**. It allows the user to:

1. Set a bit at a given position (i.e., change it to 1)
2. Reset a bit at a given position (i.e., change it to 0)

The operations are performed on the number `a = 57`, and the results are displayed after each operation.

---

## Theory

### Bitwise Operators Used:

1. `|` (OR): Used to set a specific bit to 1.  
2. `&` (AND): Used to reset a specific bit to 0 (combined with bitwise NOT).  
3. `<<` (Left Shift): Used to shift bits to the left — creates a bitmask for the specific bit position.  
4. `~` (Bitwise NOT): Inverts all bits — used to create a reset mask.

### How it Works:

#### 1. Set Bit
```cpp
set = a | (1 << bit_to_be_set);
 ```
This sets the bit at the specified position to 1 without altering other bits.

#### 2. Reset Bit
```cpp
reset = a & ~(1 << bit_to_be_reset);
```

This resets the bit at the specified position to 0, again preserving other bits.
## Working

**Initial integer:**  
`a = 57` (binary: `00111001`)

**User inputs:**

- A bit position to **set**
- A bit position to **reset**

**Output:**

- New integer value after **setting** the bit
- New integer value after **resetting** the bit

---

## Sample Output

Input the Bit position u want to set: 2

The set bit= 61

Input the Bit position u want to reset: 5

The reset bit= 25


**Explanation:**

- `57` in binary = `00111001`
- Setting bit at position `2` results in `00111101` → **61**
- Resetting bit at position `5` results in `00011001` → **25**

---

## Key Concepts Demonstrated

- **Bitwise OR (`|`)**: Turns a bit ON at a given position.
- **Bitwise AND (`&`) + NOT (`~`)**: Turns a bit OFF at a given position.
- **Left Shift (`<<`)**: Creates a bitmask by shifting a `1` to the desired position.
- **Binary Masks**: Used to isolate or manipulate specific bits in a number.
- **Memory Efficiency**: All operations are performed directly on the binary representation without using extra memory or arrays.

---

## Learning Outcomes

This program helps reinforce:

- Bitwise manipulation techniques
- Understanding of binary representations of integers
- Efficient data manipulation without using arrays or extra memory
- Practical use of logical operations on binary data
- Importance of operator precedence and correct use of parentheses in bitwise expressions


