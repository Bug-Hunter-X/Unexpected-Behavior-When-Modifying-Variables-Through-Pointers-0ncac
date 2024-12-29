# Unexpected Behavior When Modifying Variables Through Pointers

This repository demonstrates a potential pitfall when working with pointers in C.  The example shows how modifying a variable indirectly through a pointer can lead to unexpected results if not handled carefully.

## The Bug

The `bug.c` file contains a simple C program that initializes an integer variable `x` to 10. A pointer `ptr` is then assigned the address of `x`. The value pointed to by `ptr` is changed to 20. While it seems straightforward, the program's output might not be what is initially expected by someone unfamiliar with pointer behavior in C. 

## The Solution

The `bugSolution.c` provides a more explicit demonstration of the underlying concept and avoids any potential confusion. In this solution, the programmer makes the intent of manipulating the variable through a pointer explicit, enhancing code readability and maintainability.

## Learning Points

This example emphasizes the importance of understanding pointer arithmetic and memory management in C.  Careful consideration of pointer operations is essential to prevent subtle bugs in C programs.