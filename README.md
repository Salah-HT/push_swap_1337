
<img width="923" alt="Screen Shot 2023-07-21 at 1 36 49 AM" src="https://github.com/SalaHmT/push_swap_1337/blob/master/image/255043290-20c2edae-53f7-48b6-b26f-ba31ecd55267.png">

# Push Swap

A 42 School project that implements an efficient sorting algorithm using two stacks and a limited set of operations.

## Overview

Push Swap is a dual-executable system that generates and validates optimal sorting sequences for integer arrays. The project consists of two main programs:

- **push_swap**: Generates the minimum number of operations to sort an array [1](#0-0) 
- **checker**: Validates operation sequences and confirms if they correctly sort the input [2](#0-1) 

## Architecture

The system uses a shared codebase with modular design:

- **Shared dependencies**: libft functions, parsing functions [3](#0-2) 
- **Main program specific**: movement functions, sorting algorithms [4](#0-3) 
- **Bonus program specific**: silent movement functions, get_next_line [5](#0-4) 

## Available Operations

- `sa`, `sb`, `ss`: Swap first two elements
- `pa`, `pb`: Push from one stack to another
- `ra`, `rb`, `rr`: Rotate stack up
- `rra`, `rrb`, `rrr`: Rotate stack down

## Algorithm Strategy

The program uses different sorting strategies based on input size [6](#0-5) :

- **2-3 elements**: Direct sorting with minimal operations
- **4-5 elements**: Optimized small-set algorithms
- **6-200 elements**: Medium-range sorting algorithm
- **200+ elements**: Large-set optimization algorithm

## Build Instructions

```bash
# Build main program
make all

# Build checker (bonus)
make bonus

# Clean object files
make clean

# Full clean
make fclean

# Rebuild
make re
```

## Usage

```bash
# Generate sorting operations
./push_swap 4 67 3 87 23

# Validate with checker
./push_swap 4 67 3 87 23 | ./checker 4 67 3 87 23
```

## Project Structure

```
├── include/
│   └── push_swap.h          # Main header file
├── dependencies/
│   ├── libft_function/      # Custom standard library
│   ├── parsing_function/    # Input validation and parsing
│   ├── movement_function/   # Stack operations (with output)
│   ├── movement_bonus_function/ # Silent stack operations
│   ├── sorting_function/    # Sorting algorithms
│   └── get_next_line/       # Line reading for checker
├── push_swap.c              # Main program entry point
├── push_swap_bonus.c        # Checker program entry point
└── Makefile                 # Build configuration
```

## Memory Management

The system implements comprehensive memory management with dedicated cleanup functions to prevent memory leaks during normal operation and error conditions.

## Author

Created by Salah Hamsate (shamsate) as part of the 42 School curriculum.

**Notes**

This README is generated from the project's Makefile and source code structure. The push_swap project demonstrates advanced algorithm optimization, memory management, and modular C programming practices. The dual-executable architecture allows for both operation generation and validation within a single codebase.


<img width="920" alt="255043175-4c00f263-5652-4e33-ad12-50c1a538a965" src="https://github.com/SalaHmT/push_swap_1337/blob/master/image/255043175-4c00f263-5652-4e33-ad12-50c1a538a965.png">
<img width="905" alt="Screen Shot 2023-07-21 at 1 31 11 AM" src="https://github.com/SalaHmT/push_swap_1337/blob/master/image/255043198-95e5e196-bcee-48bb-b059-3a434ba284c4%20(1).png">
<img width="849" alt="Screen Shot 2023-07-21 at 1 31 31 AM" src="https://github.com/SalaHmT/push_swap_1337/blob/master/image/255043212-94153338-30b3-47f4-8aff-87aeab80bd3b%20(1).png"><br>
count action:
<img width="949" alt="Screen Shot 2023-07-21 at 1 37 34 AM" src="https://github.com/SalaHmT/push_swap_1337/blob/master/image/255043271-9a00bf4a-db07-414e-9cce-463af1836b32.png">
run checker :
<img width="932" alt="Screen Shot 2023-07-21 at 1 36 37 AM" src="https://github.com/SalaHmT/push_swap_1337/blob/master/image/255043282-7957dcbb-1982-43fa-b415-f934ed270e02.png">
checker result : 
<img width="923" alt="Screen Shot 2023-07-21 at 1 36 49 AM" src="https://github.com/SalaHmT/push_swap_1337/blob/master/image/255043290-20c2edae-53f7-48b6-b26f-ba31ecd55267.png">
