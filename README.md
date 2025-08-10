# Pointers-in-C-Plus-Plus

//NAME:MAHI THAKRAR

//PRN:24070123056

//ENTC A3

## Overview
Pointers in C++ are variables that store the **memory address** of another variable.  
They provide a powerful way to directly access and manipulate memory, making them essential for:
- **Dynamic memory allocation**
- **Efficient data handling**
- **Low-level programming**

Pointers are widely used in:
- Dynamic memory management (`new` and `delete`)
- Passing large data structures to functions without copying
- Working with arrays and strings
- Implementing data structures like linked lists, trees, and graphs

---

## Theory

### What is a Pointer?
A pointer is a special variable that stores the memory address of another variable.  
If `x` is a variable, then a pointer to `x` stores the address where `x` is located in memory.

### Syntax for Declaration
```cpp
data_type* pointer_name;
```
## Accessing and Dereferencing

- **Address-of operator (`&`)**: Retrieves the memory address of a variable.  
- **Dereference operator (`*`)**: Accesses the value at the address stored in the pointer.

## Pointer Arithmetic

Pointers can be incremented or decremented to move between memory locations, based on the size of the data type they point to.

## Null Pointers

A null pointer points to nothing and is often used for safety.

---

# Program Summaries and Algorithms

## 1. Reverse Array in C++

### Theory

Arrays in C++ store elements in contiguous memory locations with zero-based indexing.  
Reversing an array means printing or arranging its elements in the opposite order, from last to first.  
This program prints a predefined array of 5 integers in reverse order without modifying the actual array.

### Algorithm

1. Start  
2. Declare and initialize an array of size 5 with values.  
3. Set loop counter `i` to last index (`4`).  
4. While `i >= 0`:  
   - Print `arr[i]`.  
   - Decrement `i`.  
5. End.

---

## 2. Printing a String using Pointers in C++

### Theory

A string in C++ can be stored in a character array (`char[]`).  
A pointer can traverse the string character-by-character until the null terminator (`'\0'`) is reached.  
This program prints a string using pointer traversal rather than array indexing.

### Algorithm

1. Start  
2. Declare a character array `str[100]`.  
3. Declare a pointer `sptr` and assign it to point to `str`.  
4. Take user input for the string.  
5. While `*sptr` is not `'\0'`:  
   - Print the character pointed by `sptr`.  
   - Increment `sptr`.  
6. End.

---

## 3. Pointer Arithmetic in C++ for Different Data Types

### Theory

Pointer arithmetic moves the pointer based on the size of the data type it points to.  
For example, incrementing an `int*` pointer moves it by `sizeof(int)` bytes, while incrementing a `double*` moves it by `sizeof(double)` bytes.

| Data Type | Typical Size (bytes) |
| --------- | -------------------- |
| int       | 4                    |
| float     | 4                    |
| double    | 8                    |
| string    | Varies (usually pointer size, e.g., 8 bytes on 64-bit systems) |

### Algorithm

1. Start  
2. Declare variables of types `int`, `float`, `double`, and `string`.  
3. Declare pointers for each and assign the addresses of the variables.  
4. Print original values and their addresses.  
5. Increment each pointer (`ptr++`).  
6. Print the new addresses showing pointer arithmetic effect.  
7. End.

---

## 4. Pointer Value Addition and Subtraction in C++

### Theory

This program performs arithmetic operations on the **values** pointed to by pointers rather than on the pointer addresses themselves.  
It uses two pointers to elements of an integer array and computes the difference and sum of the values at those pointers.

### Algorithm

1. Start  
2. Declare and initialize an integer array.  
3. Assign two pointers to different array elements.  
4. Dereference pointers to access values.  
5. Calculate difference: `diff = (*p2) - (*p1)`.  
6. Calculate sum: `add = (*p2) + (*p1)`.  
7. Print results.  
8. End.

---

## 5. Pointer Basics in C++

### Overview

Demonstrates how to declare a pointer, store a variable’s address, and access the value via the pointer.

### Algorithm

1. Start  
2. Declare integer variable `a` and assign a value (e.g., 20).  
3. Declare pointer `aptr` of type `int*`.  
4. Store address of `a` in `aptr` using `&a`.  
5. Print:  
   - Value of `a`  
   - Value stored in `aptr` (address of `a`)  
   - Value pointed to by `aptr` (dereferenced)  
   - Address of `a` using `&a` directly  
6. End.

---

## Conclusion
Pointers in C++ are fundamental for low-level memory access, efficient data handling, and dynamic memory management.  
While powerful, pointers require careful handling to avoid errors such as dangling pointers and memory leaks.  
A solid grasp of pointers is crucial for advanced programming areas like data structures, system programming, and performance optimization.
