---
description: Revision of the VAS
---

# Virtual Address Space

## Virtual Address Space

```java
64-bit                                                          32-bit

0xFFFFFFFFFFFFFFFF ---->  +-------------------------+  <---- 0xFFFFFFFF
       ^                  |   Kernel static data    |         ^
       |                  +-------------------------+         |
       |                  |                         |         |
       |                  +-------------------------+         |
       |                  |       Kernel code       |         |
  High Canonical          +-------------------------+    Kernel only
  (Kernel only)           |                         |      access
       |                  +-------------------------+         |
       |                  |   Kernel heap + stack   |         |
       |                  +-------------------------+         |
       |                  |                         |         |
       v                  +-------------------------+         v
0xFFFF800000000000 ---->  | Physical memory mapping |  <---- 0xC0000000
Not valid space range ->  ---------------------------  <---- 0xBFFFFFFF 
0x00007FFFFFFFFFFF ---->  |         Stack           |         ^
       ^                  +-------------------------+         |
       |                  |                         |         |
       |                  |                         |         |
 Low canonical            +-------------------------+    Kernel + user
 (Kernel + user)          |          Heap           |       access
       |                  ---------------------------     (user land)
       |                  |       Static data       |         |
       |                  ---------------------------         |
       V                  |          Code           |         v
0x0000000000000000        +-------------------------+  <---- 0x00000000
```

### High canonical + Kernel only access

* CPU has to be running in privileged mode
* There's possibly more than 1 kernel stack
  * Kernel establishes kernel-level stack for when processes call **`syscall`**

### Low canonical + user land

* Stack: stores local variables and return addresses
  * LIFO structure so grows downwards
  * Grows and shrinks when values are pushed / popped from it
  * Space managed by the OS
* Heap: Where malloc'd data lives
  * Is dynamic
  * Identity of variables put on heap not known statically
  * `free()` to deallocate memory on the heap \(if fail, then memory leak\)
  * Slightly slower to r/w from because of pointers
  * Global variable access
*  Code: Currently executable process

## When to use the heap vs stack

> From [https://gribblelab.org/CBootCamp/7\_Memory\_Stack\_vs\_Heap.html](https://gribblelab.org/CBootCamp/7_Memory_Stack_vs_Heap.html)

If you need to allocate a large block of memory \(e.g. a large array, or a big struct\), and you need to keep that variable around a long time \(like a global\), then you should allocate it on the heap. If you are dealing with relatively small variables that only need to persist as long as the function using them is alive, then you should use the stack, it's easier and faster. If you need variables like arrays and structs that can change size dynamically \(e.g. arrays that can grow or shrink as needed\) then you will likely need to allocate them on the heap, and use dynamic memory allocation functions like `malloc()`, `calloc()`, `realloc()` and `free()` to manage that memory "by hand".

