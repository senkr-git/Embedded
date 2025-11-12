# Embedded Software Interview Preparation

A curated list of commonly asked questions and topics for Embedded Software Engineering interviews, structured for effective study. This guide covers computer science fundamentals, C/C++ language specifics, and core embedded systems concepts.

*(Based on topics from Grind75, marked as G75)*

---

## 🖥️ 1. Data Structures & Algorithms (CS Fundamentals)

### Arrays
* Find pivot index (sum of left == sum of right)
* Diagonal traverse and print
* Spiral matrix
* Implement `strstr()`
* **Two Pointer Technique:**
    * Reverse string
    * Array partition
    * Remove element (fast/slow runner)
    * Max consecutive 1's
    * Minimum size subarray sum
    * Rotate array
* Reverse words in a string (word by word, and reverse within words)
* Remove duplicates from a sorted array
* Move all zeroes to the end
* Max sub-array sum (Dynamic Programming)
* Find K closest elements to a given value

### Linked Lists
* Determine if there is a cycle
* Return the node where a cycle begins
* Find the intersection node of two linked lists
* Remove Nth node from the end of the list
* Reverse a linked list
* Remove all elements of a given value
* Group all odd-indexed and even-indexed nodes together
* Palindrome linked list
* Merge two sorted linked lists
* Insert into a cyclic sorted linked list
* Rotate linked list by K places
* Reverse linked list in blocks of K
* (Advanced) XOR linked list

### Hashmaps (Hash Tables)
* Two Sum (G75)
* Four Sum
* Find all duplicates
* Intersection of two arrays
* Isomorphic strings
* First unique character in a string (one-pass vs. two-pass)
* Group anagrams
* Valid Sudoku
* Longest substring without repeating characters
* Ransom Note (G75)
* Insert Delete GetRandom O(1) (G75)
* Design Hashmap
* Design LRU Cache (G75)

### Stacks
* Implement Stack using an Array
* Implement Stack using a Linked List
* Implement Queue using Stacks (G75)
* Valid (Balanced) Parentheses (G75)
* Backspace String Compare (G75)
* Evaluate Reverse Polish Notation (G75)
* Min Stack (G75)
* Daily Temperatures (G75)
* Decode String (G75)
* Asteroid Collision (G75)
* Basic Calculator II (G75)
* Trapping Rain Water (G75)

### Queues
* Implement Queue using an Array
* Implement Queue using a Linked List
* Implement Stack using Queues
* Circular (Ring) Buffer implementation
* Design Hit Counter (G75)

### Sorting & Searching
* **Sorting Algorithms:**
    * Selection Sort
    * Bubble Sort
    * Insertion Sort
    * Merge Sort
    * Quick Sort
* **Searching Algorithms:**
    * Linear Search
    * Binary Search

---

## ⌨️ 2. C / C++ Programming Language

### Bit Manipulation
* Swap bits in odd and even positions
* Check for Power of 2
* Set, clear, and toggle the i'th bit
* Find the position of the only set bit
* Count number of set bits (logN time)
* Add two numbers without arithmetic operators (G75)
* Find the only number that appears once (G75)
* Set all bits in a given range
* Compute 2's complement
* Find the position of the right-most set bit
* Isolate the right-most set bit
* Toggle the right-most set bit
* Find the position of the left-most set bit
* Swap two numbers without a temporary variable
* Reverse the order of bits in a number
* Modify a bit at a given position (set to 0 or 1)
* Missing Number (G75)
* Number of 1 Bits (Hamming Weight) (G75)
* Counting Bits (G75)
* Find the Duplicate Number (G75)

### C Language & Standard Library
* **Keywords:** `volatile`, `const`, `static`
* **Build Process:** Pre-processor, Pragmas
* **Standard Library Implementation:**
    * `memcpy` vs. `memmove`
    * `strstr`
    * `strcpy`
    * `atoi`
    * `malloc` / `free`
* **Memory:**
    * Aligned `malloc`
    * Struct padding and alignment

### C++ Concepts
* **OOP Theory:** Abstraction, Inheritance, Polymorphism, Encapsulation
* **Core C++:**
    * `new` vs. `delete`
    * Pointers vs. References
    * `lvalue` and `rvalue`
    * `inline` functions
    * `static` keyword, `static` functions
* **Object Lifecycle:**
    * Constructors vs. Destructors
    * Copy Constructors
    * Deep vs. Shallow Copy
* **Polymorphism & Advanced Features:**
    * Virtual functions, `vptr`, and `vtable`
    * Function Overloading vs. Overriding
    * Friend class and function
    * Virtual base class, Abstract class
    * Templates and Template Specialization
    * Object slicing
* **Modern C++:**
    * Smart Pointers (Unique, Shared, Weak)
    * Different types of `cast` (static, dynamic, reinterpret, const)

---

## ⚡ 3. Core Embedded Systems Concepts

### Hardware & Architecture
* **Endianness:**
    * Big Endian vs. Little Endian
    * Write a program to detect system endianness
    * Convert between endian types
* **Communication Protocols:**
    * SPI (Serial Peripheral Interface)
    * I2C (Inter-Integrated Circuit)
    * UART (Universal Asynchronous Receiver-Transmitter)
    * Differences and trade-offs
* **Timers:**
    * Hardware Timers
    * Build an API for a Software Timer using a given Hardware Timer
* **Debugging:**
    * Hardware breakpoint vs. Software breakpoint

### System Boot & Build
* **Build Toolchain:** Compiler, Assembler, Linker, Loader (steps and outputs)
* **Boot Sequence:** From power-on to `main()`
* **Firmware Updates:**
    * Process for a secure firmware update (OTA)
* **Security:**
    * Digital Signing
    * Hashing
    * Encryption

### Low-Level Programming
* **Interrupts:**
    * Interrupts vs. Exceptions
    * Differences between Fault, Abort, and Trap
* **RTOS vs. Bare Metal:**
    * Pros and Cons
    * When to use each
* **C Programming:**
    * Function pointers and their use for callbacks
* **Testing:**
    * Unit Testing vs. Integration Testing

---

## 🔄 4. Operating Systems & Concurrency

### Core OS Concepts
* **Processes & Threads:**
    * Process vs. Thread
    * Fine-grained vs. Coarse-grained multithreading
* **Memory Management:**
    * Virtual Memory, Paging, Page Faults
    * TLBs (Translation Lookaside Buffers)
    * VIPT (Virtually Indexed, Physically Tagged) caches
    * Inverted Paging
    * Buddy System memory allocation
    * Banker's Algorithm
* **Scheduling:**
    * Task scheduling algorithms
    * Thrashing
    * Belady's Anomaly
    * Cycle Stealing
* **Faults:**
    * Causes of a Segmentation Fault and how to debug it

### Concurrency & Synchronization
* **Core Primitives:**
    * Mutex vs. Semaphore
    * Spinlocks
    * Conditional Variables
    * Reader-Writer Mutex
* **Implementation:**
    * Implement a Mutex using Test-and-Set
    * Implement a Mutex using Load-Linked / Store-Conditional
* **Common Problems:**
    * Race Conditions
    * Deadlocks
    * Priority Inversion and Priority Inheritance
    * Producer-Consumer Problem
    * Dining Philosophers Problem
* **IPC Mechanisms:**
    * Queues
    * FIFO (Named Pipes)
    * Mailboxes

### System Performance
* **Cache-Aware Programming:**
    * Matrix multiplication
    * Cache blocking / Tiling
    * GEMM (General Matrix Multiply)
    * Rotation of matrices
