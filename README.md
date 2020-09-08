# Software level attacks on \(micro\) Architecture

This is a document of everything that I have learnt from the two videos from **HiPEAC** at **\#ACACES20**. They cover both a beginning to low-level, and go into heap exploitation. \(Times are in brackets for the videos\)

* Session 1

  * \(00:00\) [Virtual Address Space](session-1/virtual-address-space.md)
  * \(11:15\) [System V Calling Conventions](session-1/system-v-calling-conventions.md)
  * \(23:07\) [Buffer Overflows \(BOFs\)](session-1/buffer-overflows-bofs.md)
  * \(30:50\) [Shellcode](session-1/shellcode.md)
  * \(35:02\) [Defence: NX + page tables](session-1/nx.md)
  * \(44:30\) [Ret2libc](session-1/ret2libc.md)
  * \(56:17\) [Defence: Stack Canaries](session-1/stack-canaries.md)
  * \(1:06:27\) [Defence: Shadow stacks \(Intel CET\)](session-1/defence-shadow-stacks-intel-cet.md)
  * \(1:21:46\) [Defence: ASLR](session-1/aslr.md)
  * \(1:30:37\) [Defence: Randomising struct layout](session-1/defence-randomising-struct-layout.md)
  * \(1:33:22\) [Control Flow Graphs](session-1/control-flow-graphs.md)
  * \(1:39:50\) [Challenges of Precise CFG](session-1/challenges-of-precise-cfg.md)

* Session 2
  * Memory vulnerabilities via type confusion
  * ROP
  * JOP
  * Compiler-enforced CFI
  * Intel indirect branch tracing
  * kBouncer
  * SGX: design and vulns

## Links to the YouTube videos

{% embed url="https://www.youtube.com/watch?v=z8Wu8dpDLnI&list=PLUU79oBORyMhfViAsbK5yGZS9K5HQu4M2&index=12" caption="\#ACACES20 / Software-level Attacks on Architectural and Microarchitectural State \(session \#1\)" %}

{% embed url="https://www.youtube.com/watch?v=59HuF1hni8I&list=PLUU79oBORyMhfViAsbK5yGZS9K5HQu4M2&index=13" caption="\#ACACES20 / Software-level Attacks on Architectural and Microarchitectural State \(session \#2\)" %}

## Links to the pdf's of the slides given

{% file src=".gitbook/assets/acaces-2020-part-i.pdf" %}

{% file src=".gitbook/assets/acaces-2020-part-ii.pdf" %}



