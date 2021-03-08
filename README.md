In this tutorial, we will study what are [pointers in c programming](https://usemynotes.com/what-are-pointers-in-c-programming/), the advantage of using a pointer, the disadvantage of using pointers, operators using pointers, and a suitable example of pointers. So let’s go...

## What are Pointers in C Programming

The pointers are variables that store the address of another variable. And every variable has a unique address in memory. These addresses are in hexadecimal form, so we cannot store these addresses in any normal variables, create a pointer variable to store the address of any variable. To declare which variable of pointer type, declare it with an asterisk (*) Symbol. 

**Syntax of its declaration: -**
```
data_type *pointer_name;
```
To access the value of this variable by the address of the storage call of any variable, it is necessary to store the address of the storage call of this variable in another pointer-type variable. Because we cannot access any memory storage call without storing it in any variable.

## Advantages of Using Pointers
- Less time in program execution
- Working on the original variable
- With the help of pointers, we can create data structures (linked-list, stack, queue).
- Returning more than one values from functions
- Searching and sorting large data very easily
- Dynamically memory allocation

## Disadvantages of Using Pointers
- Sometimes by creating pointers, such errors come in the program, which is very difficult to diagnose.
- Sometimes pointer leaks in memory are also created.
- If extra memory is not found then a program crash can also occur.

## Operators Used with Pointers
### 1. & (Address-of ) operator:-
The & (Address-of) operator points to the address of the variable. From this, we can get the address of any variable.

### 2. * (Value-at) operator:-
The * (Value-at) operator only works with pointer variables. This operator represents the value stored at a particular address.

**Example:-**
```
#include<stdio.h>
int main()
{
  int rehanAge = 55;
  int *ptr;
  ptr = &rehanAge;
  /* address of rehanAge */
  printf(“Address of rehanAge: %dn”,ptr);
  /* value at rehanAge */
  printf(“Value of rehanAge: %d”,*ptr);
}
```

**Output**
```
Address of rehanAge: -1074204644
Value of rehanAge: 55
```
Originally posted on - [Pointer in C Programming](https://alimammiya.hashnode.dev/pointers-in-c-programming)
