# 0x1B. C - Sorting algorithms & Big O
# Resources

https://alx-intranet.hbtn.io/rltoken/Ea93HeEYuNkOL7sGb6zzGg
http://www.youtube.com/watch?v=ewd7Lf2dr5Q
http://justin.abrah.ms/computer-science/big-o-notation-explained.html
https://alx-intranet.hbtn.io/rltoken/-j5MKLBlzZAC2RfJ5DTBIg

# Learning Objectives
At least four different sorting algorithms
What is the Big O notation, and how to evaluate the time complexity of an algorithm
How to select the best sorting algorithm for a given input
What is a stable sorting algorithm

# Requirements

Allowed editors: vi, vim, emacs
All your files will be compiled on Ubuntu 20.04 LTS using gcc, using the options -Wall -Werror -Wextra -pedantic -std=gnu89
All your files should end with a new line
A README.md file, at the root of the folder of the project, is mandatory
Your code should use the Betty style. It will be checked using betty-style.pl and betty-doc.pl
You are not allowed to use global variables
No more than 5 functions per file
Unless specified otherwise, you are not allowed to use the standard library. Any use of functions like printf, puts, … is totally forbidden.
The prototypes of all your functions should be included in your header file called <a href =""> sort.h </a>
Don’t forget to push your header file
All your header files should be include guarded
A list/array does not need to be sorted if its size is less than 2.

# Data Structure and Functions
For this project you are given the following print_array, and print_list functions:
<hr>
#include <stdlib.h>
#include <stdio.h>

/**
 * print_array - Prints an array of integers
 *
 * @array: The array to be printed
 * @size: Number of elements in @array
 */
void print_array(const int *array, size_t size)
{
    size_t i;

    i = 0;
    while (array && i < size)
    {
        if (i > 0)
            printf(", ");
        printf("%d", array[i]);
        ++i;
    }
    printf("\n");
}
