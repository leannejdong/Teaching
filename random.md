## Random useful facts

1. What is the difference between C, embedded C and Linux kernel C?

The embedded C uses the same syntax and semantics of the C such as the `main`, declaration of datatypes, defining variables, loops, functions, statements etc.

**The extension in Embedded C from normal C** include I/O hardware addressing, fixed point arithmetic operations, accessing address spaces etc.

**The difference between embedded C and Linux kernel C** 

- Direct hardware interaction with microcontrollers or microprocessors, whereas 
linux kernel C interacts with hardware through abstraction layers provided by the linux kernel.

- Resource Constraints: Embedded C often deals with limited resources, requiring careful management of memory, power consumption,
  and processing capabilities. Linux kernel C programming benefits from resources and abstractions provided by the Linux kernel
- System complexity: Linux Kernel C focus more on complex systems, providing services to user-space applications, and dealing with interprocess communication.
- Embedded C  programming is often centred around specific tasks and hardware control.

The main distinction between embedded C and Linux Kernel C lies in the context and level of abstraction they operate at. 
Embedded C concerns with developing software for resource-constrained embedded systems, while kernel C focus on implementation of kernel-level 
functionality within the linux operating system.

2. Can you set pointer to null? Reference to null?

In C++, references cannot be set to null. Once a reference is declared and initialized, it must always refer to an object. Attempting to set a reference to null or reassign it to another object is not allowed and will result in a compilation error.

On the other hand, pointers can be reassigned. After declaring a pointer, you can change its value to point to a different memory location by assigning it a new address or the value nullptr.

```cpp
 // ptr can be set null
    int *a = new int(5);
    a = nullptr;

    int value = 3;
    // ref cannot be set null
    int &ref = value;
    ref = nullptr;

    // Can you re-assign pointer? Yes
    int value1 = 5;
    int value2 = 10;

    int* ptr = &value1;   // Pointer 'ptr' is initially assigned the address of 'value1'
    ptr = &value2;        // Pointer 'ptr' is reassigned to the address of 'value2'
    // Can you re-assign ref? No
    int& ref = value1;    // Reference 'ref' is bound to 'value1'
    // ref = value2;      // Error: References cannot be reassigned to refer to a different object
}
```
