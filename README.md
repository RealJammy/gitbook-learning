# EuanB Resources

I will be going into a lot of detail about computer science concepts, as well as cyber security related content. With the nature of this, we're going to need to learn some programming, so there shall also be a section on programming.

Anything marked with `***` needs to be done 

## Cyber Security

* [List](cybersec/list.md)
* [Binary exploitation](cybersec/binary-exploitation/)
  * [Theory](cybersec/binary-exploitation/theory/)
    * [Virtual Address Space](cybersec/binary-exploitation/theory/virtual-address-space.md)
    * [System V Calling Conventions](cybersec/binary-exploitation/theory/system-v-calling-conventions.md)
    * [Why doesn't the OS detect BOF?](cybersec/binary-exploitation/theory/side-note-os-doesnt-detect-bof.md)
    * [Control Flow Graphs](cybersec/binary-exploitation/theory/control-flow-graphs.md)
    * [Challenges of Precise CFG](cybersec/binary-exploitation/theory/challenges-of-precise-cfg.md)
    * [GOT and PLT](cybersec/binary-exploitation/theory/got-and-plt.md)
    * [Endianness](cybersec/binary-exploitation/theory/endianness.md)
    * [Pwntools](cybersec/binary-exploitation/theory/pwntools/)
      * [Setting Up pwntools](cybersec/binary-exploitation/theory/pwntools/setting-up-pwntools.md)
      * [Importing the Binary](cybersec/binary-exploitation/theory/pwntools/importing-the-binary.md)
      * [Communication](cybersec/binary-exploitation/theory/pwntools/communication.md)
      * [Packing and Context](cybersec/binary-exploitation/theory/pwntools/packing.md)
      * [Logging](cybersec/binary-exploitation/theory/pwntools/logging.md)
  * [Attacks](cybersec/binary-exploitation/attacks/)
    * [Buffer Overflows \(BOFs\)](cybersec/binary-exploitation/attacks/buffer-overflows-bofs.md)
    * [Shellcode](cybersec/binary-exploitation/attacks/shellcode.md)
    * [Ret2libc](cybersec/binary-exploitation/attacks/ret2libc.md)
    * [Format strings](cybersec/binary-exploitation/attacks/format-strings/)
      * [Fuzzer](cybersec/binary-exploitation/attacks/format-strings/fuzzer.md)
    * \*\*\* [Partial Overwrite](cybersec/binary-exploitation/attacks/partial-overwrite.md)
    * \*\*\* [Stack Pivotting](cybersec/binary-exploitation/attacks/stack-pivotting.md)
    * \*\*\* [SIGROP](cybersec/binary-exploitation/attacks/sigrop.md)
    * \*\*\* [Ret2csu](cybersec/binary-exploitation/attacks/ret2csu.md) 
  * [Defences](cybersec/binary-exploitation/untitled/)
    * [NX + page tables](cybersec/binary-exploitation/untitled/nx.md)
    * [Stack Canaries](cybersec/binary-exploitation/untitled/stack-canaries.md)
    * [Shadow stacks \(Intel CET\)](cybersec/binary-exploitation/untitled/defence-shadow-stacks-intel-cet.md)
    * [ASLR](cybersec/binary-exploitation/untitled/aslr.md)
    * [Randomising struct layout](cybersec/binary-exploitation/untitled/defence-randomising-struct-layout.md)
    * [RELRO](cybersec/binary-exploitation/untitled/relro.md)
  * \*\*\* [Defeating Defences](cybersec/binary-exploitation/defeating-defences/)
    * \*\*\* [Defeating Stack Canaries](cybersec/binary-exploitation/defeating-defences/defeating-stack-canaries.md)
    * \*\*\* [Defeating ASLR and PIE](cybersec/binary-exploitation/defeating-defences/defeating-aslr-and-pie.md)
    * \*\*\* [Defeating NX](cybersec/binary-exploitation/defeating-defences/defeating-nx.md)
    * \*\*\*[ Defeating RELRO](cybersec/binary-exploitation/defeating-defences/defeating-relro.md)

## Computer Science

[https://www.ocr.org.uk/Images/170844-specification-accredited-a-level-gce-computer-science-h446.pdf](https://www.ocr.org.uk/Images/170844-specification-accredited-a-level-gce-computer-science-h446.pdf)

* [List-cs](computer-science/untitled.md)
* [Processors](computer-science/processors/)
  * \*\*\* [Structure of processors](computer-science/processors/structure-of-processors.md)
  * \*\*\* [Fetch Decode Execute](computer-science/processors/fetch-decode-execute.md)
  * \*\*\* [Factors Affecting Performance](computer-science/processors/factors-affecting-performance.md)
  * \*\*\* [Pipelining](computer-science/processors/pipelining.md)
  * \*\*\* [Von Neumann, Harvard Architecture and Contemporary Processors](computer-science/processors/von-neumann-harvard-architecture-adn-contemporary-processors.md)
  * \*\*\* [CISC vs RISC](computer-science/processors/cisc-vs-risc.md)
  * \*\*\* [GPUs](computer-science/processors/gpus.md)
  * \*\*\* [Multi core and parallel processing](computer-science/processors/multi-core-and-parallel-processing.md)
* [Inputs and Outputs](computer-science/inputs-and-outputs/)
  * \*\*\* [Magnetic, Flash, Optical Storage](computer-science/inputs-and-outputs/magnetic-flash-optical-storage.md)
  * \*\*\* [RAM and ROM](computer-science/inputs-and-outputs/ram-and-rom.md)
  * \*\*\* [Virtual Storage](computer-science/inputs-and-outputs/virtual-storage.md)

## Programming Languages

* [List-program](programming/untitled.md)
* \*\*\* [Python](programming/python.md)
* \*\*\* [C](programming/c.md)
* \*\*\* [C++](programming/c++.md)
* \*\*\* [Rust](programming/rust.md)
* \*\*\* [Assembly \(asm\)](programming/assembly-asm/)
  * \*\*\* [Registers](programming/assembly-asm/registers.md)
  * \*\*\* [Intel Syntax](programming/assembly-asm/intel-syntax.md)
  * \*\*\* [AT&T syntax](programming/assembly-asm/at-and-t-syntax.md)
* \*\*\* [Java](programming/java.md)
* \*\*\* [Powershell](programming/powershell.md)
* \*\*\* [Bash](programming/bash.md)
* \*\*\* [SQL](programming/sql.md)
* \*\*\* [Verilog](programming/verilog.md)
* \*\*\* [Markdown](programming/markdown.md)



