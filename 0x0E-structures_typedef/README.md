Structures, typedef
Learning Objectives
What are structures, when, why and how to use them
How to use typedef
Tasks
Django
Define a new type struct dog with the following elements:

name, type = char *
age, type = float
owner, type = char *
Solution: dog.h

$ amonkeyprogrammer@ubuntu:~/0x0d. structures, typedef$ cat 0-main.c
#include <stdio.h>
#include "dog.h"

/**
 * main - check the code for Holberton School students.
 *
 * Return: Always 0.
 */
int main(void)
{
    struct dog my_dog;

    my_dog.name = "Django";
    my_dog.age = 3.5;
    my_dog.owner = "Jay";
    printf("My name is %s, and I am %.1f :) - Woof!\n", my_dog.name, my_dog.age);
    return (0);
}
$ amonkeyprogrammer@ubuntu:~/0x0d. structures, typedef$ make
gcc -Wall -pedantic -Werror -Wextra 0-main.c -o a
$ amonkeyprogrammer@ubuntu:~/0x0d. structures, typedef$ ./a 
My name is Django, and I am 3.5 :) - Woof!
$ amonkeyprogrammer@ubuntu:~/0x0d. structures, typedef$
