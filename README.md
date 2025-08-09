# Pointers-in-C-Plus-Plus

//NAME:MAHI THAKRAR
//PRN:24070123056
//ENTC A3

## 📝 Overview
Pointers in C++ are variables that store the **memory address** of another variable.  
They provide a powerful way to directly access and manipulate memory, making them essential for **dynamic memory allocation**, **efficient data handling**, and **low-level programming**.
In C++, pointers are widely used in:
- Dynamic memory management (`new` and `delete`)
- Passing large data structures to functions without copying
- Working with arrays and strings
- Implementing data structures (linked lists, trees, graphs)

## Theory

### What is a Pointer?

A pointer is a special variable that stores the memory address of another variable.  
If `x` is a variable, then a pointer to `x` will store the address where `x` is located in memory.

### 🏗️ Syntax for Declaration
```cpp
data_type* pointer_name;

**Accessing and Dereferencing
Address-of operator (&): Retrieves the memory address of a variable.
Dereference operator (*): Accesses the value at the address stored in the pointer.

**Pointer Arithmetic
Pointers can be incremented or decremented to move between memory locations.

**Null Pointers
A null pointer points to nothing and is often used for safety.


**PROGRAM SUMMARY

#1.Reverse Array in C++

## Theory
In C++, arrays store elements in **contiguous memory locations** and are accessed using **zero-based indexing**.  
Reversing an array means printing or arranging its elements in the opposite order, starting from the last element and ending with the first.
In this program:
- We have an integer array with **5 elements**.
- We use a **for loop** to iterate from the **last index (4)** down to the **first index (0)**.
- We print each element in this reverse order.
This method does **not modify** the actual array in memory; it only changes the **display order**.

## Algorithm
**Step 1:** Start  
**Step 2:** Declare and initialize an array of size 5 with given values.  
**Step 3:** Set a loop counter `i` to the last index (`4` for size 5).  
**Step 4:** While `i >= 0`, print `arr[i]` and decrement `i`.  
**Step 5:** End.

#2.Printing a String using Pointers in C++

## Theory
In C++, a **string** can be stored in a character array (`char[]`).  
When working with character arrays, a pointer can be used to traverse and display each character until the **null terminator** (`'\0'`) is reached.
Key concepts in this program:
- **Character Array (`char str[100]`)**: Stores the input string.
- **Pointer to char (`char* sptr`)**: Points to the first character of the array.
- **Null Terminator (`'\0'`)**: Marks the end of a C-style string.
- **Pointer Increment (`sptr++`)**: Moves the pointer to the next character in memory.

The program:
1. Takes a string input from the user.
2. Uses a pointer to traverse the string character-by-character.
3. Prints the string without directly using array indexing.

## Algorithm
**Step 1:** Start.  
**Step 2:** Declare a character array `str[100]` to store the string.  
**Step 3:** Declare a pointer `sptr` and make it point to `str`.  
**Step 4:** Take user input for the string.  
**Step 5:** While the current character (`*sptr`) is not `'\0'`, print the character and increment the pointer.  
**Step 6:** End.

#3.Pointer Arithmetic in C++ for Different Data Types

## Theory

In C++, a **pointer** stores the memory address of a variable.  
When we perform **pointer arithmetic** (e.g., `ptr++`), the pointer moves to the next memory location **based on the size of the data type** it points to.

### Key Concepts:
- **Pointer Declaration:**
  ```cpp
  data_type* ptr;
Address-of Operator (&): Retrieves the memory address of a variable.

Pointer Increment (ptr++): Moves the pointer forward by the size of the data type.

Memory Size Impact:
int → typically 4 bytes
float → typically 4 bytes
double → typically 8 bytes
string → implementation dependent (pointer size, usually 8 bytes on 64-bit systems)

##Algorithm
Step 1: Start.
Step 2: Declare variables of types int, float, double, and string.
Step 3: Declare pointers for each type and assign them the addresses of the variables.
Step 4: Print the original values and their addresses.
Step 5: Increment each pointer (ptr++).
Step 6: Print the new addresses to see the change based on data type size.
Step 7: End.

# 4.Pointer Value Addition and Subtraction in C++

## Theory
In C++, a **pointer** stores the memory address of a variable.  
Using the **dereference operator** (`*`), we can access the value stored at that memory address.
In this program:
- We create an integer array `arr[5]`.
- Two pointers `p1` and `p2` are assigned to point to different elements in the array.
- Instead of calculating the difference in memory addresses, we use `(*p2) - (*p1)` to find the difference between the **values** at those memory locations.
- Similarly, `(*p2) + (*p1)` finds the sum of the values.
> **Note:** This program is not performing *pointer arithmetic* on addresses, but rather arithmetic on the **values** the pointers refer to.

## Algorithm
**Step 1:** Start.  
**Step 2:** Declare and initialize an integer array.  
**Step 3:** Create two integer pointers and assign them the addresses of specific array elements.  
**Step 4:** Dereference the pointers to access the values.  
**Step 5:** Subtract the value pointed to by `p1` from the value pointed to by `p2` and store it in `diff`.  
**Step 6:** Add the two values and store it in `add`.  
**Step 7:** Print the results.  
**Step 8:** End.

#5.Pointer Basics in C++

## Overview
This program demonstrates the basic concept of **pointers** in C++.  
It shows:
- How to declare a pointer
- How to store the address of a variable in a pointer
- How to access the value of a variable using a pointer
- How to print the address of a variable
Pointers are variables that store **memory addresses** instead of actual data. They are a powerful feature in C++ that allow for direct memory access and manipulation.

## Algorithm
1. Start the program.
2. Declare an integer variable `a` and initialize it with value `20`.
3. Declare a pointer `aptr` of type `int*`.
4. Store the address of `a` in `aptr` using the **address-of operator (`&`)**.
5. Print:
   - The value of `a`
   - The value stored in `aptr` (address of `a`)
   - The value pointed to by `aptr` (dereferencing with `*`)
   - The address of `a` directly using `&a`
6. End the program.

✅ Conclusion
Pointers in C++ are a core concept for low-level memory access, efficient data handling, and dynamic memory allocation.
They can make programs faster and more flexible, but also more error-prone if misused.
A strong understanding of pointers is essential for advanced programming topics such as data structures, system programming, and memory optimization.

```cpp
data_type* pointer_name;
