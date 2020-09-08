---
description: A look at 32 bit vs 64 bit calling conventions
---

# System V Calling Conventions

## What is a calling convention?

It is a contract between the caller and the callee that function parameters and return addresses get returned to

## x86-64 

Simplest case: callee arguments + return value are integer or pointers

* Caller stores the first six arguments in the following registers in this order:
  * **`rdi`**
  * **`rsi`**
  * **`rdx`**
  * **`rcx`**
  * **`r8`**
  * **`r9`**
* Remaining arguments are passed via the `stack`
* Callee places the return value in the `rax`

## x86-32

Register pressure is so high \(Not as many registers as 64 bit\), so parameters are mostly passed via the `stack`

* Parameters are pushed in reverse order of parameter list \(LIFO structure\)
* Callee places return value in eax

## Calling functions

### Preamble

This is how a _stack frame_ would be set up

#### Stack frame

* Acts like a partition on the stack
* Created when a subroutine is defined 
* Now able to define its own local variables, as it is independent of other functions
* Created at the current rsp location

{% tabs %}
{% tab title="Intel syntax" %}
```text
push rbp         ; Save the value of the base pointer onto the stack
mov rbp, rsp     ; rbp now points to the top of the stack frame
sub rsp, 0x10    ; Space allocated for local variables
```
{% endtab %}

{% tab title="AT&T syntax" %}
```text
push %rbp         ; Save the value of the base pointer onto the stack
mov %rsp, %rbp    ; rbp now points to the top of the stack frame
sub 0x10, %rbp    ; Space allocated for local variables
```
{% endtab %}
{% endtabs %}

### Epilogue

How a stack frame would be closed

{% tabs %}
{% tab title="Intel syntax" %}
```text
leave
    -> mov rsp, rbp   ; set rsp to rbp 
    -> pop rbp        ; pop rbp
ret
    -> pop rip        ; pop the saved value into the instruction pointer
    -> jmp rip        ; jmp to that location
```
{% endtab %}

{% tab title="AT&T syntax" %}
```text
pop %rbp         ; pop the last value on the stack into rbp
ret
    -> pop %rip  ; same as intel 
    -> jmp %rip
```
{% endtab %}
{% endtabs %}

