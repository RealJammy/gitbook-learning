# EuanB26 Resources

I will be going into a lot of detail about computer science concepts, as well as cyber security related content. With the nature of this, we're going to need to learn some programming, so there shall also be a section on programming.

Anything marked with `***` needs to be done 

## Contact

[Contact](contact.md)

## Cyber Security

* [List cybersec](cybersec/list-cybersec.md)

### Binary Exploitation

* [Binary exploitation](cybersec/binary-exploitation/)
  * [Theory](cybersec/binary-exploitation/theory/)
    * [Virtual Address Space](cybersec/binary-exploitation/theory/virtual-address-space.md)
    * \*\*\* [Deep Diving ELFs](cybersec/binary-exploitation/theory/deep-diving-elfs.md)
    * [System V Calling Conventions](cybersec/binary-exploitation/theory/system-v-calling-conventions.md)
    * [Why doesn't the OS detect BOF?](cybersec/binary-exploitation/theory/side-note-os-doesnt-detect-bof.md)
    * [Control Flow Graphs](cybersec/binary-exploitation/theory/control-flow-graphs.md)
    * [Challenges of Precise CFG](cybersec/binary-exploitation/theory/challenges-of-precise-cfg.md)
    * [GOT and PLT](cybersec/binary-exploitation/theory/got-and-plt.md)
    * [Static vs Dynamic Linking](cybersec/binary-exploitation/theory/static-vs-dynamic-linking.md)
    * [Endianness](cybersec/binary-exploitation/theory/endianness.md)
    * [Pwntools](cybersec/binary-exploitation/theory/pwntools/)
      * [Setting Up pwntools](cybersec/binary-exploitation/theory/pwntools/setting-up-pwntools.md)
      * [Importing the Binary](cybersec/binary-exploitation/theory/pwntools/importing-the-binary.md)
      * [Communication](cybersec/binary-exploitation/theory/pwntools/communication.md)
      * [Packing and Context](cybersec/binary-exploitation/theory/pwntools/packing.md)
      * [Logging](cybersec/binary-exploitation/theory/pwntools/logging.md)
  * [Defences](cybersec/binary-exploitation/untitled/)
    * [NX + page tables](cybersec/binary-exploitation/untitled/nx.md)
    * [Stack Canaries](cybersec/binary-exploitation/untitled/stack-canaries.md)
    * [Shadow stacks \(Intel CET\)](cybersec/binary-exploitation/untitled/defence-shadow-stacks-intel-cet.md)
    * [ASLR](cybersec/binary-exploitation/untitled/aslr.md)
    * [Why move from 32 to 64 bit?](cybersec/binary-exploitation/untitled/why-move-from-32-to-64-bit.md)
    * [Randomising struct layout](cybersec/binary-exploitation/untitled/defence-randomising-struct-layout.md)
    * [RELRO](cybersec/binary-exploitation/untitled/relro.md)
  * [Attacks](cybersec/binary-exploitation/attacks/)
    * [Stack](cybersec/binary-exploitation/attacks/stack/)
      * [Buffer Overflows \(BOFs\)](cybersec/binary-exploitation/attacks/stack/buffer-overflows-bofs.md)
      * [Shellcode](cybersec/binary-exploitation/attacks/stack/shellcode.md)
      * [Ret2libc](cybersec/binary-exploitation/attacks/stack/ret2libc.md)
      * [Format strings](cybersec/binary-exploitation/attacks/stack/format-strings/)
        * [Fuzzer](cybersec/binary-exploitation/attacks/stack/format-strings/fuzzer.md)
      * [Stack Pivoting](cybersec/binary-exploitation/attacks/stack/stack-pivotting.md)
      * [\(SIG\)ROP](cybersec/binary-exploitation/attacks/stack/sigrop.md)
      * \*\*\* [Ret2dlresolve](cybersec/binary-exploitation/attacks/stack/ret2csu.md)
    * [Heap](cybersec/binary-exploitation/attacks/heap.md)
  * \*\*\* [Defeating Defences](cybersec/binary-exploitation/defeating-defences/)
    * \*\*\* [Defeating Stack Canaries](cybersec/binary-exploitation/defeating-defences/defeating-stack-canaries.md)
    * \*\*\* [Defeating ASLR and PIE](cybersec/binary-exploitation/defeating-defences/defeating-aslr-and-pie.md)
    * \*\*\* [Defeating NX](cybersec/binary-exploitation/defeating-defences/defeating-nx.md)
    * \*\*\*[ Defeating RELRO](cybersec/binary-exploitation/defeating-defences/defeating-relro.md)

## Computer Science

[https://www.ocr.org.uk/Images/170844-specification-accredited-a-level-gce-computer-science-h446.pdf](https://www.ocr.org.uk/Images/170844-specification-accredited-a-level-gce-computer-science-h446.pdf)

* [List-cs](computer-science/list-cs.md)
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

* [List-program](programming/list-program.md)
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



