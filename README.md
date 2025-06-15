# MiniProject-3 Subset Selection
This program finds all possible subsets of a given size from a set of integers that sum to zero, using a randomized approach.

## Description

The program randomly samples subsets of a specified size from a given set of integers and checks if their sum equals zero. Valid subsets are collected and displayed.

## Features

- Finds all unique subsets of a specified size that sum to zero
- Uses random sampling for efficient searching
- Handles both positive and negative integers
- Configurable parameters for set size and iterations
- Outputs all valid subsets and a total count

## Usage

1. **Configure the parameters** at the top of the script:
   ```python
   Set = set([-12, -3, -6, 7, 2, -2, 6, 3, 9, -7, -5, -8, 1, 11, -9, -4])  # Input set
   SetSize = 5  # Size of subsets to find
   Iterations = 1000  # Number of random samples to try
   ## Customization

Modify these parameters to customize the program's behavior:

- **`Set` variable**: Replace with your own set of integers  
  Example: `set([1, -2, 3, -4, 5])`

- **`SetSize`**: Adjust to find subsets of different sizes  
  Example: `SetSize = 3` for triplets that sum to zero

- **`Iterations`**: Control the number of random samples  
  Increase for more exhaustive search (e.g., `10000`)  
  Decrease for faster execution (e.g., `500`)

- **Duplicate handling**: Add duplicate removal logic if your input set contains duplicates

## Algorithm Overview

1. **Random Sampling**:
   - Selects a random subset of size `SetSize` from the input set

2. **Zero-Sum Check**:
   - Calculates the sum of the selected subset
   - Verifies if the sum equals zero

3. **Storage**:
   - Valid subsets are stored in a set (automatically handles duplicates)

4. **Iteration**:
   - Repeats the process for the specified number of iterations

5. **Output**:
   - Prints all unique valid subsets
   - Displays the total count of solutions found
