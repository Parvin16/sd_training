# This is my repo

## Table of content

*  [Day 0](https://github.com/Parvin16/sd_training#day-0)


## Day 0
### Theory Basic

**IC Package** - is a container that holds die and was connected to outside (external device) by using wire bonding.
Example of package - Quadruple in-line package (QIP) and Dual in-line package (DIP).


* **Pad** - used to connect inside (core) to outside (I/O), good at ESD protection to prevent charge coming from outside damage the core inside.
* **Core** - consists of all the main logic gate (NMOS/PMOS) and cell block such as macro cell and foundry IP's.
* **I/O** - help in communication between die with external and will be connected to die by using wire bonding.

+ **Differences of macro vs foundry IP's**:

![note1day0](https://user-images.githubusercontent.com/118954022/203972752-ff83fa9e-0606-4701-8380-ad3f4b81ec4c.jpg)

  * **Macro** - a simple core/cell with simple functionality and can be easily found online.
  * **Foundry IP's** - cell with more specific functionality and the design was patent/owned by a company. Has higher value compared to macro.
  
==========================================================================================

How does a **software communicate with hardware**:

**Synthesis process** will help to convert software's instructions which is written in high level language to gate level language/machine language which is normally in binary format.


**Synthesis process flow**:
1. **Specification/instructions** written in RTL (**high-level language** such as C, C++ or Java) as inputs.
1. **Compiler** will compile the instruction into **assembly language** (.exe).
1. **Assembler** will then convert **assembly language** into **gate level language** (low-level language.machine language) which is in binary format (operands), and it is the language understood by a computer.


### Lab Result
Starting a Lab

![day0 lab vsd tarainig ](https://user-images.githubusercontent.com/118954022/203966813-d18863aa-a04d-4f57-953e-b846ccb79b94.jpg)


## Day 1
