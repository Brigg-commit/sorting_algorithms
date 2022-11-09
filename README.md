# 0x1B. C - Sorting algorithms & Big O

# Resources

<ul>
<li> https://alx-intranet.hbtn.io/rltoken/Ea93HeEYuNkOL7sGb6zzGg</li>
http://www.youtube.com/watch?v=ewd7Lf2dr5Q
<li> http://justin.abrah.ms/computer-science/big-o-notation-explained.html</li>

<li> https://alx-intranet.hbtn.io/rltoken/-j5MKLBlzZAC2RfJ5DTBIg</li>

# Learning Objectives

<li>
At least four different sorting algorithms</li>

<li>
What is the Big O notation, and how to evaluate the time complexity of an algorithm</li>

<li>
How to select the best sorting algorithm for a given input
</li>

<li>
What is a stable sorting algorithm
</li>

</ul>

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

<ul>
<li>or this project you are given the following print_array, and print_list functions:</li>

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



#include <stdio.h>
#include "sort.h"

/**
 * print_list - Prints a list of integers
 *
 * @list: The list to be printed
 */
void print_list(const listint_t *list)
{
    int i;

    i = 0;
    while (list)
    {
        if (i > 0)
            printf(", ");
        printf("%d", list->n);
        ++i;
        list = list->next;
    }
    printf("\n");
}

Please use the following data structure for doubly linked list:

/**
 * struct listint_s - Doubly linked list node
 *
 * @n: Integer stored in the node
 * @prev: Pointer to the previous element of the list
 * @next: Pointer to the next element of the list
 */
typedef struct listint_s
{
    const int n;
    struct listint_s *prev;
    struct listint_s *next;
} listint_t;

0.<a href =""> Bubble sort</a>

Write a function that sorts an array of integers in ascending order using the <a href =""> Bubble sort algorithm</a>

<ul>
<li> prototype: *void bubble_sort(int array, size_t size);</li>

<li> You’re expected to print the array after each time you swap two elements (See example below)</li>

Write in the file 0-O, the big O notations of the time complexity of the Bubble sort algorithm, with 1 notation per line:

<li> in the best case</li>
<li> in the average case</li>
<li> in the worst case</li>

</ul>
