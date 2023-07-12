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
