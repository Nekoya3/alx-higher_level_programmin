# 0x00-python-hello_world

This is the first task on ALX high level programming, this tasks emphasizes Python programming language, use of python strings and python scripting.

## Learning Objectives

At the end of this task, I was able to learn :

- What is the Zen of Python
- python and shell scripting
- How to use the Python interpreter
- How to print text and variables using print
- How to use strings
- What are indexing and slicing in Python
- What is the official Python coding style and how to check your code with pycodestyle

## Tasks

### 0. [Run Python file](https://github.com/Sanctus-Peter/alx-higher_level_programming/blob/main/0x00-python-hello_world/0-run)

Write a Shell script that runs a Python script.
The Python file name will be saved in the environment variable $PYFILE
```
$ cat main.py
#!/usr/bin/python3
print("Best School")

$ export PYFILE=main.py
$ ./0-run
Best School
$
```

### 1. [Run inline](https://github.com/Sanctus-Peter/alx-higher_level_programming/blob/main/0x00-python-hello_world/1-run_inline)

Write a Shell script that runs Python code.
The Python code will be saved in the environment variable $PYCODE
```
$ export PYCODE='print(f"Best School: {88+10}")'
$ ./1-run_inline
Best School: 98
$
```

### 2. [Hello, print](https://github.com/Sanctus-Peter/alx-higher_level_programming/blob/main/0x00-python-hello_world/2-print.py)

Write a Python script that prints exactly "Programming is like building a multilingual puzzle, followed by a new line.
- Use the function __print__

### 3. [Print integer](https://github.com/Sanctus-Peter/alx-higher_level_programming/blob/main/0x00-python-hello_world/3-print_number.py)

Complete this [source code](https://github.com/holbertonschool/0x00.py/blob/master/3-print_number.py) in order to print the integer stored in the variable **number**, followed by **Battery street**, followed by a new line.
- You are not allowed to cast the variable number into a string
- Your code must be 3 lines long
- You have to use f-strings

### 4. [Print float](https://github.com/Sanctus-Peter/alx-higher_level_programming/blob/main/0x00-python-hello_world/4-print_float.py)

Complete the [source code](https://github.com/holbertonschool/0x00.py/blob/master/4-print_float.py) in order to print the float stored in the variable **number** with a precision of 2 digits.
- You are not allowed to cast number to string
- You have to use f-strings

### 5. [Print string](https://github.com/Sanctus-Peter/alx-higher_level_programming/blob/main/0x00-python-hello_world/5-print_string.py)

Complete this [source code](https://github.com/holbertonschool/0x00.py/blob/master/5-print_string.py) in order to print 3 times a string stored in the variable **str**, followed by its first 9 characters.
- You are not allowed to use any loops or conditional statement
- Your program should be maximum 5 lines long

### 6. [Play with strings](https://github.com/Sanctus-Peter/alx-higher_level_programming/blob/main/0x00-python-hello_world/6-concat.py)

Complete this [source code](https://github.com/holbertonschool/0x00.py/blob/master/6-concat.py) to print **Welcome to Holberton School!**
- You are not allowed to use any loops or conditional statements.
- You have to use the variables **str1** and **str2** in your new line of code
- Your program should be exactly 5 lines long

### 7. [Copy-Cut-Paste](https://github.com/Sanctus-Peter/alx-higher_level_programming/blob/main/0x00-python-hello_world/7-edges.py)

Complete this [source code](https://github.com/holbertonschool/0x00.py/blob/master/7-edges.py)
- You are not allowed to use any loops or conditional statements
- Your program should be exactly 8 lines long
- **word_first_3** should contain the first 3 letters of the variable **word**
- __word_last_2__ should contain the last 2 letters of the variable **word**
- **middle_word** should contain the value of the variable **word** without the first and last letters

### 8. [Create a new sentence](https://github.com/Sanctus-Peter/alx-higher_level_programming/blob/main/0x00-python-hello_world/8-concat_edges.py)

Complete this [source code](https://github.com/holbertonschool/0x00.py/blob/master/8-concat_edges.py) to print **object-oriented programming with Python**, followed by a new line.
- You are not allowed to use any loops or conditional statements
- Your program should be exactly 5 lines long
- You are not allowed to create new variables
- You are not allowed to use string literals

### 9. [Easter Egg](https://github.com/Sanctus-Peter/alx-higher_level_programming/blob/main/0x00-python-hello_world/9-easter_egg.py)

Write a Python script that prints “The Zen of Python”, by TimPeters, followed by a new line.
- Your script should be maximum 98 characters long (please check with **wc -m 9-easter_egg.py**)
```
$ ./9-easter_egg.py
The Zen of Python, by Tim Peters

Beautiful is better than ugly.
Explicit is better than implicit.
Simple is better than complex.
Complex is better than complicated.
Flat is better than nested.
Sparse is better than dense.
Readability counts.
Special cases aren't special enough to break the rules.
Although practicality beats purity.
Errors should never pass silently.
Unless explicitly silenced.
In the face of ambiguity, refuse the temptation to guess.
There should be one-- and preferably only one --obvious way to do it.
Although that way may not be obvious at first unless you're Dutch.
Now is better than never.
Although never is often better than *right* now.
If the implementation is hard to explain, it's a bad idea.
If the implementation is easy to explain, it may be a good idea.
Namespaces are one honking great idea -- let's do more of those!
$
```

### 10. [Linked list cycle](https://github.com/Sanctus-Peter/alx-higher_level_programming/blob/main/0x00-python-hello_world/10-check_cycle.c)

**Technical interview preparation:**

- You are not allowed to google anything
- Whiteboard first
- This task and all future technical interview prep tasks will include checks for the efficiency of your solution, i.e. is your solution’s runtime fast enough, does your solution require extra memory usage / mallocs, etc.

Write a function in C that checks if a singly linked list has a cycle in it.
- Prototype: **int check_cycle(listint_t *list);**
- Return: 0 if there is no cycle, 1 if there is a cycle

#### Requirements:
Only these functions are allowed: write, printf, putchar, puts, malloc, free

```C
$ cat lists.h
#ifndef LISTS_H
#define LISTS_H

#include <stdlib.h>

/**
 * struct listint_s - singly linked list
 * @n: integer
 * @next: points to the next node
 *
 * Description: singly linked list node structure
 * 
 */
typedef struct listint_s
{
    int n;
    struct listint_s *next;
} listint_t;

size_t print_listint(const listint_t *h);
listint_t *add_nodeint(listint_t **head, const int n);
void free_listint(listint_t *head);
int check_cycle(listint_t *list);

#endif /* LISTS_H */
```

```C
$ cat 10-linked_lists.c
#include <stdio.h>
#include <stdlib.h>
#include "lists.h"

/**
 * print_listint - prints all elements of a listint_t list
 * @h: pointer to head of list
 * Return: number of nodes
 */
size_t print_listint(const listint_t *h)
{
    const listint_t *current;
    unsigned int n; /* number of nodes */

    current = h;
    n = 0;
    while (current != NULL)
    {
        printf("%i\n", current->n);
        current = current->next;
        n++;
    }

    return (n);
}

/**
 * add_nodeint - adds a new node at the beginning of a listint_t list
 * @head: pointer to a pointer of the start of the list
 * @n: integer to be included in node
 * Return: address of the new element or NULL if it fails
 */
listint_t *add_nodeint(listint_t **head, const int n)
{
    listint_t *new;

    new = malloc(sizeof(listint_t));
    if (new == NULL)
        return (NULL);

    new->n = n;
    new->next = *head;
    *head = new;

    return (new);
}

/**
 * free_listint - frees a listint_t list
 * @head: pointer to list to be freed
 * Return: void
 */
void free_listint(listint_t *head)
{
    listint_t *current;

    while (head != NULL)
    {
        current = head;
        head = head->next;
        free(current);
    }
}

```

```C
$ cat 10-main.c
#include <stdlib.h>
#include <string.h>
#include <stdio.h>
#include "lists.h"

/**
 * main - check the code
 *
 * Return: Always 0.
 */
int main(void)
{
    listint_t *head;
    listint_t *current;
    listint_t *temp;
    int i;

    head = NULL;
    add_nodeint(&head, 0);
    add_nodeint(&head, 1);
    add_nodeint(&head, 2);
    add_nodeint(&head, 3);
    add_nodeint(&head, 4);
    add_nodeint(&head, 98);
    add_nodeint(&head, 402);
    add_nodeint(&head, 1024);
    print_listint(head);

    if (check_cycle(head) == 0)
        printf("Linked list has no cycle\n");
    else if (check_cycle(head) == 1)
        printf("Linked list has a cycle\n");

    current = head;
    for (i = 0; i < 4; i++)
        current = current->next;
    temp = current->next;
    current->next = head;

    if (check_cycle(head) == 0)
        printf("Linked list has no cycle\n");
    else if (check_cycle(head) == 1)
        printf("Linked list has a cycle\n");

    current = head;
    for (i = 0; i < 4; i++)
        current = current->next;
    current->next = temp;

    free_listint(head);

    return (0);
}
```
```
$ gcc -Wall -Werror -Wextra -pedantic -std=gnu89 10-main.c 10-check_cycle.c 10-linked_lists.c -o cycle
carrie@ubuntu:~/0x00$$ ./cycle
1024
402
98
4
3
2
1
0
Linked list has no cycle
Linked list has a cycle
```

#### ps:
Solving a problem is already a big win! but finding the best and optimal way to solve it, it’s way better! Think about the most optimal / fastest way to do it.

### 11. [Hello, write](https://github.com/Sanctus-Peter/alx-higher_level_programming/blob/main/0x00-python-hello_world/100-write.py)

Write a Python script that prints exactly **and that piece of art is useful - Dora Korpar, 2015-10-19**, followed by a new line.
- Use the function write from the sys module
- You are not allowed to use print
- Your script should print to stderr
- Your script should exit with the status code 1

### 12. [Compile](https://github.com/Sanctus-Peter/alx-higher_level_programming/blob/main/0x00-python-hello_world/101-compile)

Write a script that compiles a Python script file.
The Python file name will be stored in the environment variable **$PYFILE**
The output filename has to be **$PYFILEc** (ex: **export PYFILE=my_main.py** => output filename: **my_main.pyc**)

```
$ cat main.py
#!/usr/bin/python3
print("Best School")

$ export PYFILE=main.py
$ ./101-compile
Compiling main.py ...
$ ls
101-compile  main.py  main.pyc
$ cat main.pyc | zgrep -c "Best School"
1
$ od -t x1 main.pyc # SYSTEM DEPENDANT => CAN BE DIFFERENT
0000000 ee 0c 0d 0a 91 26 3e 58 31 00 00 00 e3 00 00 00
0000020 00 00 00 00 00 00 00 00 00 02 00 00 00 40 00 00
0000040 00 73 0e 00 00 00 65 00 00 64 00 00 83 01 00 01
0000060 64 01 00 53 29 02 7a 10 48 6f 6c 62 65 72 74 6f
0000100 6e 20 53 63 68 6f 6f 6c 4e 29 01 da 05 70 72 69
0000120 6e 74 a9 00 72 02 00 00 00 72 02 00 00 00 fa 07
0000140 6d 61 69 6e 2e 70 79 da 08 3c 6d 6f 64 75 6c 65
0000160 3e 02 00 00 00 73 00 00 00 00
0000172
```

### 13. [ByteCode->Python #1](https://github.com/Sanctus-Peter/alx-higher_level_programming/blob/main/0x00-python-hello_world/102-magic_calculation.py)
Write the Python function **def magic_calculation(a, b):** that does exactly the same as the following Python bytecode:
```
 3           0 LOAD_CONST               1 (98)
              3 LOAD_FAST                0 (a)
              6 LOAD_FAST                1 (b)
              9 BINARY_POWER
             10 BINARY_ADD
             11 RETURN_VALUE
