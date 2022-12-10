# This is my repo

## Table of content

*  [Day 0](https://github.com/Parvin16/sd_training/blob/main/readme.md#day-0) - System/Tool Setup Check. GitHub ID creation
*  [Day 1](https://github.com/Parvin16/sd_training/blob/main/readme.md#day-1) - Introduction to Verilog RTL Design and Synthesis
*  [Day 2](https://github.com/Parvin16/sd_training/blob/main/readme.md#day-2) - Timing libs(QTMs/ETMs), Hierarchical vs Flat Synthesis and Efficient Flop Coding Styles
*  [Day3]( ) - Combinational and Sequential Optimizations
*  [Day4]( ) - GLS, Blocking vs Non-blocking and Synthesis-Simulation mismatch
*  [Day5]( ) - DFT
*  [Day6]( ) - Introduction to Logic Synthesis


## Day 0
### Theory Basic

![chip](https://user-images.githubusercontent.com/118954022/205806514-3bc166e8-7d8f-4fa7-bfb1-9f8445d3a3b6.jpg)

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

--------------------------------------------------------------------------------------------------

## Day 1

### Open-source Simulator Iverilog and Synthesis

![TestBench](https://user-images.githubusercontent.com/118954022/205607323-ed0d9f04-64bf-44ef-815b-015f60d2d878.jpg)

**Simulator** - Tool used to simulating design. RTL design checked for adherence to the spec by simulating the design. eg: iverilog.
**Design** - The actual Verilog code / set of Verilog codes. It has intended functionality to meet the requirements. 
**TestBench** - A setup to check the functionality of the design wether it is obeying or not by applying stimulus(test_vesctors).
 Note: Simualtor is looking for change in the input values. No change in input, no change to the output. 
 
 **Iverilog Simultion Flow**:
 
 ![iverilog flow](https://user-images.githubusercontent.com/118954022/205609796-a0640932-c666-427b-bd1d-580b11ca72be.jpg)

 **VCD file** - Value Change Dump format file, output file of iverilog. 
 **gtkwave** - A tool to view the output in a waveform format.

![yosys 1](https://user-images.githubusercontent.com/118954022/205850578-acdc3325-bfdc-46f4-bb25-2dde63261765.jpg)

**Synthesizer** - tool used to convert RTL to netlist. Eg: Yosys.
**Netlist** - a file of representative of the design in  the form of standard cells in the .lib .

Verify the Synthesis :
![yosys 2](https://user-images.githubusercontent.com/118954022/205851298-873238e5-541f-4ece-b8e8-90e0b46b333b.jpg)

Synthesis 

![synthesis 1](https://user-images.githubusercontent.com/118954022/205862428-d27fdb4b-5a18-425c-9500-c17456091855.jpg)

**RTL Design** - Behavioral representation of the required specification. 
**Synthesis** - The RTL to gate level translation where the design is converted into gates and the connections are made between gates which given out as a file called netlist.
**.lib** - Collection of logical modules includes basic logic gates. Different flavors of same gate. 

Combinational delay in logic path determines the max speed of operation of digital logic circuit. We need cells to work fast enough for required performance.
Faster the charging , lesser the cell delay. Propagation delay is the time for the input to be fill up the output.

![sysnthesis 2](https://user-images.githubusercontent.com/118954022/205865780-da755d6c-7a6b-4fbf-b6c3-6cdc002bbca5.jpg)

We need cells to work fast enough for required performance.Faster the charging/discharging of capacitance, lesser the cell delay. Propagation delay is the time for the input to be fill up the output. Faster cells do not comes free, they comes with area and power consumption. 

Why do we need slow cells? - to meet holds. To ensure that there are no HOLD issues at DFF_B, we need cells that work slowly.
The collection forms the **.lib** .

**Transistors** - charge/discharge the capacitance fast and sourcing more current. **Wider transistors** - low delay (more area and power). **Narrow transistors** - More delay (less area and power). 
**Constarints** - the guidance offered to syntheziser with the correct set of cells. 

------------------------------------------------------------------------------------------------

 ### LABS

**LAB 1 - iverilog and gtkwave**

* Create VLSI directory, git clone the path and done setup labs with files. 

![lab1](https://user-images.githubusercontent.com/118954022/205810801-6083626c-1b34-405f-afd3-14b729c85e6e.jpg)

* Check git cloning and ts files. Verilog_files contains all the details and it comes along with tb files (testbench).

![lab1 1](https://user-images.githubusercontent.com/118954022/205815692-9ce497f0-b66b-44ee-a23b-1055dff84b72.jpg)

* Load iverilog, command >>  iverilog good_mux.v tb_good_mux.v , (design name = good_mux.v) , then ls , execute a.out file ( >> ./a.out), dumpfile tb_good_mux.vcd opened for output.

![lab1 2](https://user-images.githubusercontent.com/118954022/205838648-a7236d46-52e5-4c08-9808-92278baa8f6e.jpg)

* Load .vcd file in simulator ( >> gtkwave (wave file) ), then observe the waveform pattern. 

![lab1 3](https://user-images.githubusercontent.com/118954022/205840901-707693be-8568-4412-ac3e-196312daa819.jpg)

* Look into file >> gvim tb_good_mux.v -o good-mux.v , Unit Under Test (UUT), //Initialize Inputs - this showing the stimulus generators , #300 - refers to running time 300ns and we can change run time here. Below that is the toggle settings, where always #75 sel = -sel; it means that every 75ns it changes its value.  

![lab 1 4](https://user-images.githubusercontent.com/118954022/205848755-c72633d7-88fa-445c-9930-fa40a40ef965.jpg)

**LAB 2 - Yosys and Sky130 PDKs**

* Invoke Yosys ( >> yosys). 

![lab2 0](https://user-images.githubusercontent.com/118954022/205979710-cdaa0cf5-8ce7-4890-aaf4-cca1711d0ce7.jpg)

* Read the library file from my_lib ( >> read_liberty)

![lab2 1](https://user-images.githubusercontent.com/118954022/206081939-25e08d4c-6d5e-4599-8449-4d83b874fc00.jpg)

* Read design (>> read_verilog)

![lab2 2](https://user-images.githubusercontent.com/118954022/205999677-e1492a86-2d9a-4ed7-b1c0-01e05c5c7d8b.jpg)

* To link the module that we are going to do synthesis. (>> synth -top)

![lab2 3](https://user-images.githubusercontent.com/118954022/206001758-68506909-4ba2-4c1b-9f78-0e0c982bf9bb.jpg)

* Command to generate the netlist (converts the rtl file into gate and specify what gate will be link to).(>> abc -liberty). Focus on the last part of internal, input and output signals. 

![lab2 4](https://user-images.githubusercontent.com/118954022/206087861-59fdd3f5-3cd8-4615-b33e-705bac78e4e5.jpg)

* To see the graphical version of the logic it realised ( >> show).

![lab2 5](https://user-images.githubusercontent.com/118954022/206088587-e929ebca-15e8-4a63-917d-acb368b46e14.jpg)

* Write the netlist ( >> write_verilog).

![lab2 6](https://user-images.githubusercontent.com/118954022/206093571-86733aa0-b415-495a-ac11-8dcbd40a01de.jpg)

* Convert to view in simplified netlist version ( >> write_verilog -noattr ).

![lab2 7](https://user-images.githubusercontent.com/118954022/206094427-b76866ad-10c8-424e-9cd4-469b93e5def2.jpg)

--------------------------------------------------------------------------------------------------

## Day 2

### Theory

![note1](https://user-images.githubusercontent.com/118954022/206676452-7fa846b3-ccb6-4a97-81f9-21f07f01fc6e.jpg)

<img width="649" alt="note2" src="https://user-images.githubusercontent.com/118954022/206155681-a270c9f8-9571-4850-a8dd-4338873bde1b.png">

<img width="643" alt="note3" src="https://user-images.githubusercontent.com/118954022/206155789-307dc603-27e2-48bb-8bfd-f39654b9b37c.png">

<img width="707" alt="note4" src="https://user-images.githubusercontent.com/118954022/206155866-5ad2df82-eb79-47c4-8e12-26f588c7e482.png">

<img width="650" alt="note5" src="https://user-images.githubusercontent.com/118954022/206155913-f58eb53a-30c7-4e3d-809b-af49f8309733.png">

(A.B) bar = A bar + B bar ; CMOS NAND got stacked NMOS ; 
NOR + INV = OR , this will stack PMOS and it is bad ; basic CMOS inverter.
Difference between hier and flat design. 
Glitch. More combinational circuit used, more glitches happens. This is why we used **FLOPS** in between combinational circuits. Flops which has clock in it, will make the output more stable and settle down the glitches. 
Flop. ( types, reset, set, synchronous and asynchronous) 

Flop with asy&syn-reset , syn-reset and asyn-reset.

![note6](https://user-images.githubusercontent.com/118954022/206848949-7b799eaa-a4cb-457a-8a37-700df77a3d38.jpg)


------------------------------------------------------------------------------------------------

### Labs

**LAB 1 - Intro to timing.libs**

in gvim ../my../lib/sky/...lib , if saw lot of highlighted in red , just press in tht gvim tab , ':syn off' .

Library name is sky130_fd_sc_hd__tt_025C_1v80.lib .
In library name _tt_ - this mean it is typical process of library. Other two diff process of libraries are slow and fast. _025C_ this refers to temperature and _1v80_ refers to voltage. 

(number of inputs)'square = possible conditions. A = 1 = high ; A! = 0 = low. 

**LAB 2 - Hierarchical vs Flat Synthesis**

Open file >> gvim multiple_modules.v , Multiple modules have some sub modules in it that are connected to inputs and outputs. 

![lab 2 0](https://user-images.githubusercontent.com/118954022/206657428-7249931c-6a0e-40bf-9025-a1b9be7d96e0.jpg)

For sysnthesis part, open yosys ,read_liberty file, read_verilog , synth -top multiple_modules.v , then can see details at point 3.25.

![lab 2 1](https://user-images.githubusercontent.com/118954022/206659004-d573a8eb-5dcc-40a6-aa25-7f7aee747671.jpg)

Then >> abc -liberty ../my_lib/lib/sky130_fd_sc_hd__tt_025C_1v80.lib ;  >> show ; >> show multiple_modules ,it will show the hierarchy model.

![lab 2 3](https://user-images.githubusercontent.com/118954022/206662082-ce4dbd88-dd23-4313-93d3-01aeb5032587.jpg)

Then >> write_verilog -noattr multiple_modules_hier.v ; >> !gvim multiple_modules_hier.v 

![lab 2 4](https://user-images.githubusercontent.com/118954022/206675312-e16b96c6-4906-4fbe-a4c4-3279706eda6b.jpg)

Next, to verify out flat netlist, >> flatten ; >> write_verilog -noattr multiple_modules_flat.v ; >> !gvim multiple_modules_flat.v , it shows as a single netlist where hierarchy all are flatten. To see the flat design module >> show 

![lab 2 5](https://user-images.githubusercontent.com/118954022/206679063-0667de52-98f9-4098-9229-59fc9ab5e97f.jpg)

![lab 2 6](https://user-images.githubusercontent.com/118954022/206680700-52f4a089-e346-4381-8a9b-a5728a495252.jpg)

To do sub module synthesis , just repeat the steps and at this point , do this >> synth -top sub_module1 ; >> abc -liberty ; >> show ; we will see only the gates in sub module 1. Module level synthesis will be doing when we have multiple instances of same module, so just do module and replicate it. Good to do in massive design using design and conquer method. 

**LAB 3 - Flop Synthesis Simulations**

Files used for this lab in verilog_files are  dff_asyncres_syncres.v and counter_opt.v

Open dff_asyncres_syncres.v ; Lets see acychronous-reset. Asynchronous is irespective of clock where it cn happens at anytime, not based on posedge or negedge.  always @ posedge clk - this signifies a flop. q is output. **Posedge** - is the clk change from 0 to 1 , **Negedge** - is the clk change from 1 to 0. 

![lab 3 0](https://user-images.githubusercontent.com/118954022/206844524-4f2023fd-52b7-4ffb-9a0f-d5dcf548c8a2.jpg)

We going to use the dff files that is highlighted in the snapshot below. 

![lab 3 1](https://user-images.githubusercontent.com/118954022/206851064-08e0199c-bce7-44f2-a8f6-31c55698beba.jpg)
