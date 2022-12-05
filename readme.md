# This is my repo

## Table of content

*  [Day 0](https://github.com/Parvin16/sd_training#day-0)
*  [Day 1](https://github.com/Parvin16/sd_training/blob/main/readme.md#day-1)


## Day 0
### Theory Basic

![ic package](https://user-images.githubusercontent.com/118954022/205561763-5f0e8dbd-a4d5-4834-b794-a5267fdecd2f.jpg)

* **IC Package** - the material that contains a semiconductor device. The package is a case that surrounds the circuit material to protect it from corrosion or physical damage and allow mounting of the electrical contacts connecting it to the printed circuit board (PCB).

![chip parts](https://user-images.githubusercontent.com/118954022/205562390-02869142-9fd8-461e-99e4-732a76a7dcd0.jpg)

* **Pad** - a square of top-level metal of approximately 100µm on a side that is either soldered to bond wire connecting to a package or coated with lead solder ball. Pad refers to metal square only or to the complete I/O cell containing the metal.
* **Core** - a core comprises a logical execution unit and functional units. It able to independently execute programs or threads. Consists of main logics.
* **Die** - is the formal term for the square of silicon containing an integrated circuit that has been cut out of the wafer.

**Macro and Foundry IP's**

![note1day0](https://user-images.githubusercontent.com/118954022/203972752-ff83fa9e-0606-4701-8380-ad3f4b81ec4c.jpg)

* **Macro** - Hard macro, firm macro and soft macro are all known as IP (Intellectual property). They are optimized for power, area and performance. They can be purchased and used in your ASIC or FPGA design implementation flow. Soft macro is flexible for all type of ASIC implementation. Soft macros are synthesizable register transfer level (RTL) design forms, have more flexibility, and can be configured compared to hard complex macros. Using Soft macros in the design is a risk factor because of its being unpredictable behavior in timing, performance and power
* **Foundry IP's** - all Intellectual Property, regardless of when or for what purpose it is developed, pertaining to genetic components, pathways, and strains; and methods and tools for design, genetic engineering, testing and/or small-scale fermentation of microbial strains.Has higher value compared to macro.
  
--------------------------------------------------------------------------------------------------

**Software communication with Hardware**

<img width="547" alt="process flow" src="https://user-images.githubusercontent.com/118954022/205565519-1869689f-7d35-4ccf-bdd7-a38275e7a8f7.png">

**Synthesis process** - a process of converting RTL (synthesizable Verilog code) into a technology specific Gate level netlist which includes nets, sequential cells, combinational cells and their connectivity. It is a process of combining pre-existing elements to form something new. It is the conversion of an idea into an implementation.

**Process flow**:

**Application Software** -> **System Software** -> **Hardware**

**Specification/instructions** - written in RTL (high-level language) such as C, C++ or Java as inputs.
**Compiler** - compile of the instruction into assembly language (.exe).
**Assembler** - convert of the assembly language into gate level language (low-level language or machine language) which is in binary format, and it is the language understood by a computer.

--------------------------------------------------------------------------------------------------

### Lab Result
Starting a Lab (Intel Unix) 

![day0 lab vsd tarainig ](https://user-images.githubusercontent.com/118954022/203966813-d18863aa-a04d-4f57-953e-b846ccb79b94.jpg)


## Day 1

