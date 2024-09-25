# Computer Architecture Assignment – 2

## Overview
This project implements three essential algorithms in MIPS assembly language: calculating the factorial of a number, sorting an array using the selection sort algorithm, and searching for a number in an array using the binary search algorithm. These implementations demonstrate fundamental programming concepts and how algorithms operate at a low level in a non-pipelined MIPS processor.

## Implemented Programs
1. **Factorial of a Number**
   - **Description**: Computes the factorial of a non-negative integer.
   - **Algorithm**: The program uses a loop to multiply the current product by each integer from 1 to the given number.
   - **Instructions Used**: 
     - Load Word (lw)
     - Store Word (sw)
     - Add Immediate (addi)
     - Multiply (mul)
     - Branch on Not Equal (bne)
     - Jump (j)

2. **Selection Sort**
   - **Description**: Sorts an array of integers in ascending order using the selection sort algorithm.
   - **Algorithm**: The program iterates through the array, repeatedly finding the minimum element from the unsorted portion and swapping it with the first unsorted element.
   - **Instructions Used**:
     - Load Word (lw)
     - Store Word (sw)
     - Add Immediate (addi)
     - Add (add)
     - Branch on Greater Than or Equal (bge)
     - Jump (j)

3. **Binary Search**
   - **Description**: Searches for a specific integer in a sorted array using the binary search algorithm.
   - **Algorithm**: The program defines lower and upper bounds for the search interval, calculates the midpoint, and adjusts bounds based on comparisons to the target value.
   - **Instructions Used**:
     - Load Word (lw)
     - Store Word (sw)
     - Load Address (la)
     - Add Immediate (addi)
     - Shift Right Logical (srl)
     - Shift Left Logical (sll)
     - Branch on Equal (beq)
     - Branch on Less Than (blt)
     - Branch on Greater Than (bgt)
     - Jump (j)

## Assumptions in Processor Design
- ALUOp for the `bne` instruction is defined as 11.
- ALU control input codes for `srl` and `sll` are defined as ‘101’ and ‘110’ respectively.

## Results
The project demonstrates the functionality of each algorithm with the following expected outputs:
- **Factorial**: Displays the computed factorial value.
- **Selection Sort**: Shows the sorted array after execution.
- **Binary Search**: Returns the index of the searched number or -1 if not found.

## Instructions for Running the Programs
1. Open the MARS MIPS Assembler.
2. Load the corresponding assembly code file for each algorithm.
3. Assemble the code.
4. Run the program and observe the results in the data memory.
