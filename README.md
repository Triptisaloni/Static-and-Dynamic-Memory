# Static-and-Dynamic-Memory
8.Static & Dynamic Memory

In a C++ program, memory is divided into two parts:
The stack: All of your local variables take up memory from the stack.
The heap: Unused program memory that can be used when the program runs to dynamically allocate the memory.

new keyword allocates a new memory location in heap

int *p = new int;
*p = 5;

The pointer p is stored in the stack as a local variable, and holds the heap's allocated address as its value.

delete 

For local variables on the stack, managing memory is carried out automatically.
On the heap, it's necessary to manually handle the dynamically allocated memory, and use the delete operator to free up the memory when it's no longer needed 

int *p = new int; // request memory
*p = 5; // store value

cout << *p << endl; // use value

delete p; // free up the memory
// now p is a dangling pointer

p = new int; // reuse for a new address

dangling pointer
Pointers that are left pointing to non-existent memory locations are called dangling pointers.

9.Sizeof( )



The sizeof operator can be used to get a variable or data type's size, in bytes.
Syntax: - sizeof ( datatype);
