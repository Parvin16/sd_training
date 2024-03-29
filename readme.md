# #MY_VSD_REPO

## Table Of Content

+  [Day_0](https://github.com/Parvin16/sd_training/blob/main/readme.md#Day_0) : **System/Tool Setup Check. GitHub ID creation**
   * [Lab](https://github.com/Parvin16/sd_training#lab-result)
+  [Day_1](https://github.com/Parvin16/sd_training/blob/main/readme.md#Day_1) - **Introduction to Verilog RTL Design and Synthesis**
   * [Lab](https://github.com/Parvin16/sd_training#labs)
+  [Day_2](https://github.com/Parvin16/sd_training/blob/main/readme.md#Day_2) : **Timing libs(QTMs/ETMs), Hierarchical vs Flat Synthesis and Efficient Flop Coding Styles**
   * [Lab](https://github.com/Parvin16/sd_training#labs-1)
+  [Day_3](https://github.com/Parvin16/sd_training/blob/main/readme.md#Day_3) - **Combinational and Sequential Optimizations**
   * [Lab](https://github.com/Parvin16/sd_training#labs-2)
+ [Day_4](https://github.com/Parvin16/sd_training/blob/main/readme.md#Day_4) : **GLS, Blocking vs Non-blocking and Synthesis-Simulation mismatch**
   * [Lab](https://github.com/Parvin16/sd_training#labs-3)
+  [Day_5](https://github.com/Parvin16/sd_training#Day_5) - **DFT**
+  [Day_6](https://github.com/Parvin16/sd_training#Day_6) : **Introduction to Logic Synthesis**
   * [Lab](https://github.com/Parvin16/sd_training#labs-4)
+  [Day_7](https://github.com/Parvin16/sd_training#Day_7) : **Basic SDC Constraints**
   * [Lab](https://github.com/Parvin16/sd_training#labs-5)
+  [Day_8](https://github.com/Parvin16/sd_training#Day_8) : **Advanced SDC Constraints**
   * [Lab](https://github.com/Parvin16/sd_training#labs-6)
+  [Day_9](https://github.com/Parvin16/sd_training#Day_9) : **Optimization in Synthesis**
   * [Lab](https://github.com/Parvin16/sd_training#labs-7)
+  [Day_10](https://github.com/Parvin16/sd_training#Day_10) : **QOR**
   * [Lab](https://github.com/Parvin16/sd_training#labs-8)
+  [Day_11](https://github.com/Parvin16/sd_training#Day_11) : **Introduction to the BabySoC**
+  [Day_12](https://github.com/Parvin16/sd_training#Day_12) : **VSD BabySoC Modelling**
   * [Lab](https://github.com/Parvin16/sd_training#labs-9)
+  [Day_13](https://github.com/Parvin16/sd_training#Day_13) : **Post-synthesis Simulation**
   * [Lab](https://github.com/Parvin16/sd_training#labs-10) 
+  [Day_14](https://github.com/Parvin16/sd_training#Day_14) : **Synopsys DC and Timing Analysis**
   * [Lab](https://github.com/Parvin16/sd_training#labs-11) 
+  [Day_15](https://github.com/Parvin16/sd_training#Day_15) : **Inception of EDA and PDK**
   * [Lab](https://github.com/Parvin16/sd_training#labs-12) 
+  [Day_16](https://github.com/Parvin16/sd_training#Day_16) : **Understand Importance of Good Floorplan vs Bad Floorplan & Intro to Library Cells**
   * [Lab](https://github.com/Parvin16/sd_training#labs-13) 
+  [Day_17](https://github.com/Parvin16/sd_training#Day_17) : **Design and Characterise One Library Cell using Layout Tool and Spice Simulator**
   * [Lab](https://github.com/Parvin16/sd_training#labs-14)
+  [Day_18](https://github.com/Parvin16/sd_training#Day_18) : **Pre-layout Timing Analysis and Importance of Good Clock Tree**
   * [Lab](https://github.com/Parvin16/sd_training#labs-15)
+  [Day_19](https://github.com/Parvin16/sd_training#Day_19) : **Final Steps for RTL2GDS**
   * [Lab](https://github.com/Parvin16/sd_training#labs-16)
+  [Day_20](https://github.com/Parvin16/sd_training#Day_20) : **Floorplanning and Power Planning Labs**
   * [Lab](https://github.com/Parvin16/sd_training#labs-17)
+  [Day_21](https://github.com/Parvin16/sd_training#Day_21) : **Placement and CTS Labs**
   * [Lab](https://github.com/Parvin16/sd_training#labs-18)
+  [Day_22](https://github.com/Parvin16/sd_training#Day_22) : **CTS Analysis Labs**
   * [Lab](https://github.com/Parvin16/sd_training#labs-19)   
+  [Day_23](https://github.com/Parvin16/sd_training#Day_23) : **Clock Gating Technique**
   * [Lab](https://github.com/Parvin16/sd_training#labs-20) 
+  [Day_24](https://github.com/Parvin16/sd_training#Day_24) : **Timing Violations and ECO**
   * [Lab](https://github.com/Parvin16/sd_training#labs-21) 
+  [Day_25](https://github.com/Parvin16/sd_training#Day_25) : **RISC-V Core RTL2GDS Flow**
+  [Day_26](https://github.com/Parvin16/sd_training#Day_26) : **Introduction to Mixed-signal Flow**
+  [Day_27](https://github.com/Parvin16/sd_training#Day_27) : **Introduction to Crosstalk - Glitch and Delta Delay**
   * [Lab](https://github.com/Parvin16/sd_training#labs-22)
+  [Day_28](https://github.com/Parvin16/sd_training#Day_28) : **Introduction to DRC/LVS**
   * [Lab](https://github.com/Parvin16/sd_training#labs-23)
+  [Day_29](https://github.com/Parvin16/sd_training#Day_29) : **DRC/LVS Labs**

# #Day_0
### BASICS

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

### LAB Result
Starting a Lab (Intel Unix) 

![day0 lab vsd tarainig ](https://user-images.githubusercontent.com/118954022/203966813-d18863aa-a04d-4f57-953e-b846ccb79b94.jpg)

--------------------------------------------------------------------------------------------------

# #Day_1

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

# #Day_2

### THEORY

![note1](https://user-images.githubusercontent.com/118954022/206676452-7fa846b3-ccb6-4a97-81f9-21f07f01fc6e.jpg)

<img width="649" alt="note2" src="https://user-images.githubusercontent.com/118954022/206155681-a270c9f8-9571-4850-a8dd-4338873bde1b.png">

<img width="643" alt="note3" src="https://user-images.githubusercontent.com/118954022/206155789-307dc603-27e2-48bb-8bfd-f39654b9b37c.png">

Setup Time is the time the input data signals are stable (either high or low) before the active clock edge occurs. Hold Time is the time the input data signals are stable (either high or low) after the active clock edge occurs.

<img width="707" alt="note4" src="https://user-images.githubusercontent.com/118954022/206155866-5ad2df82-eb79-47c4-8e12-26f588c7e482.png">

<img width="650" alt="note5" src="https://user-images.githubusercontent.com/118954022/206155913-f58eb53a-30c7-4e3d-809b-af49f8309733.png">

**Hierarchical netlist**: Since pins of submodules are accessible, it's easier to track paths for functional debugging and timing analysis. Pins can be forced or probed in post-synthesis simulations. When have more then 1 module for the entire design. **Flattened netlist**: Synthesis tool can optimize the circuit better. That provides better speed, area, and power. Conversely, debugging capabilities are limited. Hierarchical designs can be recursively "flattened" by creating a new copy (with a new name) of each definition each time it is used. If the design is highly folded, expanding it like this will result in a much larger netlist database, but preserves the hierarchy dependencies. 

![cmos1](https://user-images.githubusercontent.com/118954022/206891318-f193bd3b-a22e-4796-8a6e-6c8482b75f5b.png)

**CMOS Inverter**. When the low input voltage is given to the CMOS inverter, then the PMOS transistor is switched ON whereas the NMOS transistor will switch OFF by allowing the flow of electrons throughout the gate terminal & generating high logic output voltage.

(A.B) bar = A bar + B bar ; CMOS NAND got stacked NMOS ; NOR + INV = OR, this will stack PMOS and it is bad.

![glitch note1 (Reserch Gate)](https://user-images.githubusercontent.com/118954022/206891176-992e63fc-ad67-4baa-bb82-3f366e3b7375.jpg)

**Glitch**. 20 cm of wire will also delay a signal by 1 nanosecond. A + = TRUE. However consider what happens when the signal A goes from 1 to 0. This spurious 0 is called a Glitch. More combinational circuit used, more glitches happens. This is why we used flops in between combinational circuits. Flops which has clock in it, will make the output more stable and settle down the glitches. 

![flop1 ](https://user-images.githubusercontent.com/118954022/206891440-a4a9978c-b273-4f10-b4dd-e23f17a0fc13.jpg)

**Flip-flop** - the circuits that maintain a certain state unless and until directed by the input for changing that state. There are 4 types of flops, but we are going to focus on D Flip-flop. The D flip-flop can be used to introduce delay to the data path. The SET input 'S' set the device or produce the output 1, and the RESET input 'R' reset the device or produce the output 0. The SET and RESET inputs are labeled as S and R, respectively. An asynchronous reset activates as soon as the reset signal is asserted. A synchronous reset activates on the active clock edge when the reset signal is asserted. 

Flop with asy&syn-reset , syn-reset and asyn-reset.

![note6](https://user-images.githubusercontent.com/118954022/206848949-7b799eaa-a4cb-457a-8a37-700df77a3d38.jpg)

------------------------------------------------------------------------------------------------

### LABS

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

Then, >> iverilog dff_asyncres.v tb_dff_asyncres.v ; >> ./a.out ; >> gtkwave tb_dff_asyncres.vcd ; then drag signals in and run. Then do same for rest 2 dff files. Observe and refer to the specific file's code to find out the differences between the files. 

![lab 3 2](https://user-images.githubusercontent.com/118954022/206888013-207571c1-30aa-46e2-949a-a0054f5a4f7d.jpg)

Next is synthesis the 3 circuits using yosys. Open yosys, read and sync -top  dff_asyncres.v , then dfflibmap -liberty ../my_lib/lib/sky130_fd_sc_hd__tt_025C_1v80.lib (this to tell the system to only look the dff file). Then, abc -liberty , then show. 

![lab 3 3](https://user-images.githubusercontent.com/118954022/206888956-25c5efca-8373-4f9c-982e-42322f3f77f4.jpg)

Then do same read_verilog for the rest 2 dff files. Observe the set pin, reset pin and the dflop. We got what we wanted based on the code. 

Next is sysnthesis and RTL code optimisation. We going to use 2 files: mult_2.v and mult_8.v . a[2:0] this means it has 3 bit inputs/outputs. 

![lab 3 4](https://user-images.githubusercontent.com/118954022/206890249-4a530268-791f-4d93-ad61-8e334bfe9844.jpg)

mult_2.v explanation in truth table form. Can compare the result by seeing the design module using yosys , read mult file, abc and show. Do same for mult_8.v file. 

![lab 3 5](https://user-images.githubusercontent.com/118954022/206890427-2fb01147-b179-4dc1-8b1f-4245ab5d7388.jpg)

Extra note: bin 101 if it is times with 4, add 2 zeros at behind (10100) ; if times with 8, add 3 zeros at behind (101000). Can make sure by convert into dec. 


--------------------------------------------------------------------------------------------------

# #Day_3

### Intro to Optimizations 

<img width="614" alt="note1" src="https://user-images.githubusercontent.com/118954022/206914099-6c84840f-a466-4236-a6a9-5d03faf627ba.png">

<img width="647" alt="note2" src="https://user-images.githubusercontent.com/118954022/206914122-723eef1f-d29d-47b5-85a4-6e5b7f7ba6c1.png">

![note12](https://user-images.githubusercontent.com/118954022/206921332-a728ee92-c5a7-4370-a161-04b0aab1ea61.jpg)

![note 8](https://user-images.githubusercontent.com/118954022/206916632-1ac45ab5-6ae1-43dc-bba2-0b4750e5e64b.jpg)

<img width="473" alt="note 3" src="https://user-images.githubusercontent.com/118954022/206914159-d5c28f63-4e56-4754-92b9-30d410401661.png">

DeMorgan's and Absorption law are two importants law.

![note10](https://user-images.githubusercontent.com/118954022/206920074-a4204aaa-1895-4ffe-bdab-cebde653dc8d.jpg)

![note11](https://user-images.githubusercontent.com/118954022/206920181-3ee97efc-88c4-4b1f-b441-1de5aeb7bf27.jpg)

**Sequential Logic** - is a type of logic circuit whose output depends on the present value of its input signals and on the sequence of past inputs, the input history. We present a powerful [sequential logic optimization method] that is based on selectively precomputing the output logic values of the circuit one clock cycle before they are required, and using the precomputed values to reduce internal switching activity in the succeeding clock cycle.

<img width="633" alt="note4" src="https://user-images.githubusercontent.com/118954022/206914250-a9a1e6d2-3cb6-4e23-9e1d-c0aff04b5ce0.png">

<img width="614" alt="note5" src="https://user-images.githubusercontent.com/118954022/206914266-ca73cd2b-04d4-4540-84ee-85c589a554d2.png">

<img width="625" alt="note6" src="https://user-images.githubusercontent.com/118954022/206914346-77fc275d-5d00-4b0e-b57a-94ea8719f0f8.png">

![note 9](https://user-images.githubusercontent.com/118954022/206919844-99ac105f-06ad-487c-9a2e-890678512189.jpg)

<img width="606" alt="note7" src="https://user-images.githubusercontent.com/118954022/206914384-5b35c832-cb61-49d0-9554-c419da0fc875.png">

The algorithms use a field of Computational Mathematics called Graph theory. Going through that, it will give you a different perspective on circuits.

**State Optimization** - Optimization of used state (redundant). As the number of states increases, it becomes difficult to distinguish between possible states. The initial design attempt may include more states than are required by a finite-state machine. Some of the states are redundant, which increases the complexity of the finite-state machine unnecessarily. There are many processes such as state minimization, cloning (physical aware) and retiming. 

Retiming :
![note8](https://user-images.githubusercontent.com/118954022/207113880-7c0a7069-11b1-4316-8521-e0b5ca673089.jpg)


------------------------------------------------------------------------------------------------

### Labs

**LAB 1 - Combinational Logic Optimizations**

The files going to use are :
![lab1 0](https://user-images.githubusercontent.com/118954022/206922571-9aa57347-eb7c-4c27-81ce-25332f67350f.jpg)

gvim opt_check.v and opt_check2.v , then compare both
![lab1 1](https://user-images.githubusercontent.com/118954022/206925830-5a63d584-23ca-4b6d-9ba0-f1dddc1a2004.jpg)

![lab1 1 1](https://user-images.githubusercontent.com/118954022/206925846-a5e6e61d-8c03-4942-a143-6e7f7dd26a75.jpg)

then continue with yosys (read_liberty -lib ../my_lib/lib/sky130_fd_sc_hd__tt_025C_1v80.lib ; read_verilog opt_check.v ; synth -top opt_check ; opt_clean -purge ; abc -liberty ../my_lib/lib/sky130_fd_sc_hd__tt_025C_1v80.lib ; show) . Same do for opt_check2.v from read_verilog in yosys and show. 

![lab1 2](https://user-images.githubusercontent.com/118954022/206927189-8b763d3d-c8cb-4eaf-a84b-32c6ef917835.jpg)

Next check for opt_check3.v file.
![lab1 3](https://user-images.githubusercontent.com/118954022/206927739-2cdce767-befd-4956-90aa-9049456e40ca.jpg)

Then tried check for multiple_moduleopt.v file (read_liberty -lib ../my_lib/lib/sky130_fd_sc_hd__tt_025C_1v80.lib ; read_verilog multiple_module_opt.v ; synth -top multiple_module_opt ; flatten ; opt_clean -purge ; abc -liberty ../my_lib/lib/sky130_fd_sc_hd__tt_025C_1v80.lib ; show)

![lab1 4](https://user-images.githubusercontent.com/118954022/206928459-254348c0-e2d9-45ff-9e19-df5a9fc1bddc.jpg)

**LAB 2 - Sequential Logic Optimizations** 

The files going to use are:
![lab2 0](https://user-images.githubusercontent.com/118954022/206928627-0eff01b1-6222-4005-8013-24dbce5899c2.jpg)

gvim  dff_const1.v and  dff_const2.v , then compare both
![lab2 1](https://user-images.githubusercontent.com/118954022/206928934-78dc1615-706c-4526-9d72-f2eda817f164.jpg)

![lab2 2](https://user-images.githubusercontent.com/118954022/206928989-e7a78506-84e8-44c3-96ea-7e90472cf379.jpg)

Simulate tb in verilog_files tab ( >> iverilog dff_const1.v tb_dff_const1.v ; >> ./a.out ). Then, >> gtkwave tb_dff_const1.vcd , we can observe the function of clk here where flop is signified. 
![lab2 3](https://user-images.githubusercontent.com/118954022/206929471-930b6d64-ac49-481f-9550-2018e87f330a.jpg)

Then in yosys ( read_liberty -lib ../my_lib/lib/sky130_fd_sc_hd__tt_025C_1v80.lib ; read_verilog dff_const1.v ; synth -top dff_const1 ; dfflibmap -liberty ../my_lib/lib/sky130_fd_sc_hd__tt_025C_1v80.lib ; abc -liberty ../my_lib/lib/sky130_fd_sc_hd__tt_025C_1v80.lib ; show), do same for dff_const2.v and rest but no need to dfflibmap. 

![lab2 4](https://user-images.githubusercontent.com/118954022/206947780-f773d22e-897f-42ad-a806-24051a3535c9.jpg)

![lab2 5](https://user-images.githubusercontent.com/118954022/206985792-efe4edce-7703-4364-abaa-a2352786dee4.jpg)

Looking on dff_const3.v , there are 2 flops, first flop is reset flop and flop is set flop. Some delay exists at Q1, so the Q will obtain '0' instead of '1'. Having 1 set 1 reset, no optimization (no constant output), so both flops need to be present. 
![lab2 8](https://user-images.githubusercontent.com/118954022/207231744-7622ffa8-b7eb-41b2-aa22-e97bb54ead7b.jpg)

![lab2 6](https://user-images.githubusercontent.com/118954022/207112593-061c67c7-dc26-4b43-8db8-814a58dd2133.jpg)

![lab2 7](https://user-images.githubusercontent.com/118954022/207116046-14673c9b-535e-4c65-a064-b44e1f16e6e2.jpg)

**LAB 3 - Sequential Logic Optimizations for unused outputs** 

File using is counter_opt.v ,it has a clk , reset and output q. There is a signal internal to it which is 3 bit register signal (count). The code is a upcounter, its rolls back 0-7 (upto 7 because 3 bit count) again and again until reset is thr.
![lab3 0](https://user-images.githubusercontent.com/118954022/207232952-6bd5ba9e-35ca-4376-a66b-4e036e414a46.jpg)

The 2 case is just example for more understanding. 
![lab3 1](https://user-images.githubusercontent.com/118954022/207234062-9eeb00c3-1fde-4c49-b855-5c2db799c9ba.jpg)

Then sysnthesis in yosys ( read_liberty -lib ../my_lib/lib/sky130_fd_sc_hd__tt_025C_1v80.lib ; read_verilog counter_opt.v ; synth -top counter_opt ; dfflibmap -liberty ../my_lib/lib/sky130_fd_sc_hd__tt_025C_1v80.lib ; abc -liberty ../my_lib/lib/sky130_fd_sc_hd__tt_025C_1v80.lib ; show)
![lab3 2](https://user-images.githubusercontent.com/118954022/207235155-71caf754-3b00-42d5-b0ff-39522810f28b.jpg)

We are  seeing only one flop. Suppose 3 bit counter should have 3 flops, but it is toggle where it invert the q output for next input, and the rest 2 bits were unused. 

Modify the RTL ( >> cp counter_opt.v counter_opt2.v ; gvim counter_opt2.v ; 

![lab3 3](https://user-images.githubusercontent.com/118954022/207297128-740cfe8e-1df6-49db-87c5-a6f8da35b07d.jpg)

Change the code , at assign q = (count[2:0] == 3'b100) 
![lab3 4](https://user-images.githubusercontent.com/118954022/207300163-faf13bd8-fc94-4994-81f6-72b8b37154b3.jpg)

Then launch yosys and observe. ( synth -top counter_opt - this part not change the file to counter_opt2 since theprocess still in the old file name)
Now we can see the 3 bit flops. We can see the 
![lab3 5](https://user-images.githubusercontent.com/118954022/207305830-5604bb44-d6c8-4242-b338-55c1dcb2c390.jpg)

Interpret the logic , and it make sense now. (use de morgan law). We can see all the three count are in use. 
![lab3 6](https://user-images.githubusercontent.com/118954022/207306659-010dc99d-39af-4cc3-9db0-3a3ce0c9f334.jpg)


--------------------------------------------------------------------------------------------------

# #Day_4

### GLS Concepts and Flow Using Iverilog

**GLS** - Gate-Level Simulation. Running the testbench with netlist as Design Under Test. Netlist is same as the RTL code (same tb will align with the design). 

Why GLS : To verify the logical correctness of design after synthesis. Ensuring the timing of the design is met by run with delay annotation.

GLS using iverilog :
![note1 0](https://user-images.githubusercontent.com/118954022/207538972-448a1b16-d605-4864-9fb1-daa9a6699fff.jpg)

<img width="628" alt="onenote1" src="https://user-images.githubusercontent.com/118954022/207377212-c11b4373-f6b8-432c-91f5-370e04d5b671.png">

### Synthesis-Simulation Mismatch

Synthesis-Simulation Mismatch happens due to missing sensitivity list, blocking vs non-blocking assignments and non standard verilog coding.

Simulator works based on activity ( output change based on inputs). Coding should be correct and accurate. Synthesis usually will create a mux and acts as flop.

![note1 1](https://user-images.githubusercontent.com/118954022/207545430-e93612bc-d9b8-4585-9293-982ac5324f47.jpg)

<img width="548" alt="onenote5" src="https://user-images.githubusercontent.com/118954022/207377691-a31e1c92-bf8b-449e-a67a-d6196f9867fe.png">

<img width="634" alt="onenote6" src="https://user-images.githubusercontent.com/118954022/207377716-115693e4-e406-40a5-904a-8b9af2196cf0.png">

<img width="566" alt="onenote8" src="https://user-images.githubusercontent.com/118954022/207378215-6a33c401-2c0a-4d90-982c-501bb9e7b021.png">

<img width="685" alt="onenote9" src="https://user-images.githubusercontent.com/118954022/207378260-62efc6db-b99e-41d8-ad40-844e0f007922.png">

### Blocking and Non Blocking Statements in Verilog

**Blocking Statement** - inside always block, making assignments using '='. It executes the statement in the order it is written ( first statement evaluvated before second statement, like a C program). 
**Non-Blocking Statement** - is a parallel evaluation (order doesnt matter) using '<='. Executes all the RHS when always block is entered and assigns to LHS. 

<img width="644" alt="onenote2" src="https://user-images.githubusercontent.com/118954022/207377260-87f674eb-eeb7-4281-a9d9-ce0ca2854db9.png">

<img width="646" alt="onenote3" src="https://user-images.githubusercontent.com/118954022/207377289-dc92238c-a61d-4185-b339-35be9f5cceac.png">

<img width="662" alt="onenote4" src="https://user-images.githubusercontent.com/118954022/207377652-b0d72af1-2541-44b2-846e-4894abab6512.png">

<img width="650" alt="onenote7" src="https://user-images.githubusercontent.com/118954022/207378028-313641b3-db79-47ce-87b8-6d804b5d5a55.png">

### Caveats with Blocking Statements

**Caveat** - a warning to consider. 

Whenever want to write sequential circuit, go with non-blocking statement.

The issue:
![note1 2](https://user-images.githubusercontent.com/118954022/207557926-85b5c930-a80c-4b91-a719-222e2ff75f23.jpg)

Another example :
![note1 3](https://user-images.githubusercontent.com/118954022/207560559-4cc4feee-b666-4884-a27a-f7cc08fea8c5.jpg)

It is very important to check the behaviour of the circuit obtained and then match them with the expected outputs (the aim). 


------------------------------------------------------------------------------------------------

### LABS

**LAB 1 - GLS & Synthesis-Simulation Mismatch**

Recap on run GLS : we need netlist, verilog models and testbench. Then submit these all to iverilog and it dumps out the vcd file. Vcd file contains the waveform which we use gtkwave to see it. 

Files we going to use are  ternary_operator_mux , bad_mux.v and good_mux.v . 
![lab1 0](https://user-images.githubusercontent.com/118954022/207318033-10fae90b-3f7f-4fab-afbf-d3e8108cf180.jpg)

Ternary operator (mux). Condition true : y=i1 , condition is false : y=i0 . 
![lab1 1](https://user-images.githubusercontent.com/118954022/207320140-06d59aa5-4433-4542-8382-a7a4d4100084.jpg)

![lab1 4](https://user-images.githubusercontent.com/118954022/207331373-7845ee1b-b59f-4695-b18c-145baee4f50b.jpg)

Basic rtl simulation: ( >> iverilog ternary_operator_mux.v tb_ternary_operator_mux.v ; ./a.out ; gtkwave tb_ternary_operator_mux.vcd )
![lab1 2](https://user-images.githubusercontent.com/118954022/207322850-d1f623c6-26c0-40f4-9948-2e5322be7c8d.jpg)

Then invoke yosys (>> read_liberty -lib ../my_lib/lib/sky130_fd_sc_hd__tt_025C_1v80.lib ; read_verilog ternary_operator_mux.v ; synth -top ternary_operator_mux ;  abc -liberty ../my_lib/lib/sky130_fd_sc_hd__tt_025C_1v80.lib ; write_verilog -noattr ternary_operator_mux_net.v ; show )
![lab1 3](https://user-images.githubusercontent.com/118954022/207330108-0414a68e-c7fd-492d-86d0-2ed7f428145d.jpg)

Next do GLS , invoke iverilog by read 2 standard files and netlist (>> iverilog ../my_lib/verilog_model/primitives.v ../my_lib/verilog_model/sky130_fd_sc_hd.v ternary_operator_mux_net.v tb_ternary_operator_mux.v ; ./a.out ; gtkwave tb_ternary_operator_mux.vcd ). For RTL , we only see UUT ; GLS we will see numbers under the UUT. 
![lab1 5](https://user-images.githubusercontent.com/118954022/207338804-7348f544-d964-4d18-8a7c-d8ad1f85c69b.jpg)

Next gvim bad_mux.v , the problem here is the always block will work upon sel, will work as flop kind behaviour.
![lab1 6](https://user-images.githubusercontent.com/118954022/207357447-a952b000-017f-4255-a07b-8142356baa96.jpg)

RTL simulation on bad_mux (>>  iverilog bad_mux.v tb_bad_mux.v ; ./a.out ; gtkwave tb_bad_mux.vcd ). When select went high, i1 is high. output y depends on posedge of select , not the changes on i1.
![lab1 7](https://user-images.githubusercontent.com/118954022/207358889-8188d967-0986-4ad4-8798-bf2593a1897a.jpg)

Simulate the bad_mux netlist  (>> iverilog ../my_lib/verilog_model/primitives.v ../my_lib/verilog_model/sky130_fd_sc_hd.v bad_mux_net.v tb_bad_mux.v ; ./a.out ; gtkwave tb_bad_mux.vcd ). It is GLS. Sel is low, it following i0 , when high it follows i1. 
![lab1 10](https://user-images.githubusercontent.com/118954022/207366342-62af32f8-b486-4809-9b53-fd4e27bb5de2.jpg)


Open in yosys ( read_liberty -lib ../my_lib/lib/sky130_fd_sc_hd__tt_025C_1v80.lib ; read_verilog bad_mux.v ; synth -top bad_mux ;  abc -liberty ../my_lib/lib/sky130_fd_sc_hd__tt_025C_1v80.lib ; write_verilog -noattr bad_mux_net.v ; show )

There is no flop or latch kind type of bahviour , only mux type.
![lab1 8](https://user-images.githubusercontent.com/118954022/207362651-7cb71be8-07fb-49a9-acde-7306f50a19a8.jpg)

![lab1 9](https://user-images.githubusercontent.com/118954022/207364629-05efc86c-b07e-4401-be53-6e11f3a8b1fb.jpg)


**LAB 2 - Synthesis-Simulation Mismatch for Blocking Statement**

gvim blocking_caveat.v , d executes firts follows by x. x in d equation is a flopped output where it will be replaced by the new x after the x equation is done.
![lab2 0](https://user-images.githubusercontent.com/118954022/207367628-857d2a23-a77e-4868-8c2f-88f619e37d64.jpg)

The logic that need to create ( x is the a or b , and y output is d, based on the code above)
![lab2 1](https://user-images.githubusercontent.com/118954022/207369093-9de2c110-3ef6-42ad-a42a-cf035b2f0016.jpg)

RTL simulation (>> iverilog ../my_lib/verilog_model/primitives.v ../my_lib/verilog_model/sky130_fd_sc_hd.v blocking_caveat_net.v tb_blocking_caveat.v ; ./a.out ; gtkwave tb_blocking_caveat.vcd )
![lab2 2](https://user-images.githubusercontent.com/118954022/207371356-bc245f6d-633c-427d-9eed-0aa8e118a23f.jpg)

Open in yosys ( read_liberty -lib ../my_lib/lib/sky130_fd_sc_hd__tt_025C_1v80.lib ; read_verilog blocking_caveat.v ; synth -top blocking_caveat ;  abc -liberty ../my_lib/lib/sky130_fd_sc_hd__tt_025C_1v80.lib ; write_verilog -noattr blocking_caveat_net.v ; show ). It is or2 and gate. There is no latch so cannot look on past value.
![lab2 3](https://user-images.githubusercontent.com/118954022/207373008-6948e0ff-5c23-46f9-be64-c6e39e23706d.jpg)

GLS simulation : (>> iverilog ../my_lib/verilog_model/primitives.v ../my_lib/verilog_model/sky130_fd_sc_hd.v blocking_caveat_net.v tb_blocking_caveat.v ; ./a.out ; gtkwave tb_blocking_caveat.vcd ) compare with RTL. 

Need to be very carefull when using blocking statement in verilogs. Avoid mistakes in here which might lead to huge turnover in design cycle.


--------------------------------------------------------------------------------------------------

# #Day_5

### DFT ( DESIGN FOR TESTABILITY )

**TESTABILITY** - it means a characteristic of an item's design which allows the status (operable, inoperable or degraded) of that item to be confidently and quickly determined. In VLSI term, it means " if a design is _well-Controllable_ and _well-Observable_ it is said to easily testable ". It is possible when a known input is applied to a unit in a known state, and a known response can be evaluated. Testability analysis involves circuit topological analysis without test vectors and search algorithm, it has linear complexity. Through testability analysis, estimation of fault coverage, number of untestable faults and test vector length is also possible.

![web2](https://user-images.githubusercontent.com/118954022/207802976-b2f2fc23-8e65-4ad3-ae71-50ea207a9be0.jpg)
source: www.electronics-tutorial.net

**DFT** - a technique which facilitates a design to become testable after production. Adding an extra design for an existing design to make sure it can be tested after being fabricated. A few samples of Designs included for making the whole chip testable. 
Intel term - **DFx**. 

Example : 
* Macros, we including **MBist Logic**
* Flops, we will use **Scan Chains**
* Combinational Circuit, we will **Generate Test Patterns**

**Why DFT ??** - it makes the testing easy at the post-production process. It is also done due to economical and market needs. 

We have mainly 3 levels of testing after a chip being fabricated :
* **Chip-level**, when chips are manufactured.
* **Board-level**, when chips are integratedon the boards/package.
* **System-level**, when several boards are assembled together like laptops. 

Pros :
* Reduces tester complexity and tester time.
* Faster development cycle and better quality of results.
* Reduces the chances of going into loss due to faulty devices. 
* Easier diagnostics and improved product quality.
* Realize concurrent engineering and support hierarchical test.
* Improve fault coverage.

Cons :
* DFT adds complication to the design flow.
* DFT increase power, area,timing and package pins.
* Design time increases.

**DFT** lies in the basic ASIC design flow, where it is included at the beginning of design flow during ' Synthesis '. It is a step of the Design Process in which testing features are added to the hardware. An appropriate strategy being factored into early iterations of an ASICs architecture rather than making significant changes later. A DFT engineer might also conduct further analysis during the RTL design phase to help identify elements that might prove particularly helpful or detrimental, though the main bulk of DFT is typically inserted into a design later in the process.

![web1 0](https://user-images.githubusercontent.com/118954022/207801100-11e71234-c820-48ed-844a-3b94778dd42d.jpg)
source: Quora

### BASIC TERMINOLOGIES

**Controllability** - from DFT point of view, we intend if both '0' and '1' are able to _propagate_  to each and every node within the 
patterns. A point is said to be controllable if both '0' and '1' can be propogated through scan patterns. 

**Observability** - the ability to _measure_ the state of a logic signal. When we say that a node is observable, we mean that the value at the node can be shifted out through scan patterns and can be observed through scan out ports. Example like adding a flip flop to a node line between register to other extra circuitry. 

**Defect** - in an electronic system is the unintended difference between the implemented hardware and its intended design. Typical defects in VLSI chips are process defects, material defects, aging defects, and package defects.

**Fault** - is a physical damage or defect compared to the good system, which may not cause system failure /or/ a representation of a “defect” at the abstracted function level is called a fault.

**Error** - it is caused by a fault because of which system went to erroneous state. A wrong output signal produced by a defective system. An error is an effect whose cause is some “defect.”

**Failure** - when the system is not providing the expected service. 

[  A **fault** causes an **error** which leads to the system **failure**.  ]

**Fault Coverage** - % of the total number of logical faults that can be tested using a given test set T.

![web3](https://user-images.githubusercontent.com/118954022/207812851-67a0c362-c507-40d8-b7a2-c3eb9b22c84d.jpg)

**Defect Level** - refers to the fraction of shipped parts that are defective /or/ the proportion of the faulty chip in which fault isn't detected and has been classified as good. There are two methods for the determination of defect level. One is from the field return data. Chips failing in the field are returned to the manufacturer. The number of returned chips normalized to one million chips shipped is the defect level. The other is using test data. Fault coverage of tests and chip fallout rate are analyzed.

### DFT METHODSS

There are mainly 2 methods for digital circuits :

1. **Ad-hoc Methods**

Ad hoc DFT method relies on good design experience and experienced designers to find the problem area, such as low coverage area. Sometimes circuit modification or test-point insertion may be required to improve the testability for these areas. The ad hoc DFT methods are usually too labor-intensive and do not guarantee good results from ATPG. For these reasons, for large circuits it is **discouraged** to use ad hoc DFT.

* Avoid combinational feedback.
* All flip flops must be initializable.
* Partition on a large circuit into small blocks.
* Provide test control for the signals which are not controllable.
* While designing test logic we have to consider the ATE requirements. 

2. **Structured Methods** 

* Scan ( in the design all the flip flops are converted to **scan flip flop** )
* Partial Scan. ( only selects a subset of flip-flops to be scanned )
* Boundary Scan. ( uses a shift-register stage to test factors such as interconnects and clusters of logic and memories ) Below is boundary scan architecture.

![web6](https://user-images.githubusercontent.com/118954022/207942470-dc9b34e0-edbb-4d73-ae86-50ffc07c8ecb.jpg)
source: https://www.slideshare.net/NejehFerjani/dft-10717334

* Built-in self-test (Bist). Involving the insertion of additional hardware and software features into integrated circuits to allow them to perform self-testing Commonly used for memory block testing. 2 most common categories:
  - MBist ( Memory Bist ) - used specifically for testing memories. It typically consists of test circuits that apply a collection of write-read-write sequences for memories.
  - LBist ( Logic Bist ) - is designed for testing random logic.
Below is Bist architecture.

![web7](https://user-images.githubusercontent.com/118954022/207942672-6de9e8c3-a754-4ac1-b42b-354338401663.jpg)


### INTRO TO SCAN-CHAINS

Scan Chain Technique :
* Specifying the Scan constraint 
* Specifying Scan ports and Scan enables
* Compiling the dft
* Identifying the number of Scan chains

**Scan Chains** are the elements in scan-based designs that are used to _shift-in and shift-out test data_. They are used to detect manufacturing defects present in the combinational logic of the design. A scan chain is formed by a number of flops connected back to back in a chain with the output of one flop connected to another. The **input  of first flop** is connected to the **input pin of the chip** ( know as **scan-in** ) from where scan data is fed. The **output of the last flop** is connected to the **output pin of the chip** ( known as **scan-out** ) which is used to take the shifted data out. 

![web9](https://user-images.githubusercontent.com/118954022/207946794-65c52b34-7d28-453f-983e-05ee4b3f3274.jpg)

**Scan Flip Flop** (SFF) - SFF is generally used for clock edge-trigged scan design. Scan design is realized by replacing flip-flops by scan flip-flops (SFFs) and connecting them to form one or more shift registers in the test mode. A multiplexer is added in front of the DFF to construct a scan D-type flip-flop (SDFF). The test enable (TE) signal controls the working mode of the SDFF. When it is high, it selects the test mode and the scan-in (SI) bits are taken as the input of the DFF. When the TE signal is low, the SDFF works as in functional mode. It acts as a normal DFF and takes value D from the combination circuits as the input to the DFF. Figure below shows the SFF based on D type flip flop (DFF).

![web5](https://user-images.githubusercontent.com/118954022/207940339-b403ceb7-22e1-4019-bf08-f1c80381440e.jpg)

There are 3 types of scan flip-flops configurations :
* Multiplexed
* Clocked
* LSSD ( Level-Sensitive Scan Design )

![web10](https://user-images.githubusercontent.com/118954022/207947495-11d4689d-96f1-40f1-8a34-ac67f15a894d.jpg)

Purpose of Scan flops : 
* To test stuck-at faults in manufactured devices.
* To test the paths in the manufactured devices for delay, eg: to test whether each path is working at functional frequency or not. 

**Functionality of Scan Chain**

The goal is to make each node in the circuit controllable and observable. Simple steps to do basic scan-in and scan-out : 

1. **Assert scan_enable** (make it high) so as to enable (SI->Q) path for each flop.
2. Keep shifting in the scan data until the intended values at intended nodes are reached.
3. **De-assert scan_enable** (for one pulse of clock in case of stuck-at testing and two or more cycles in case of transition testing) to enable D->Q path so that the combinational cloud output can be captured at the next clock edge.
4. Again **assert scan_enable** and shift out the data through scan_out.

Figure below shows a scan chain in a sequential circuit design. The SFFs are stitched together to form a scan chain. When test enable signal SE is high, the circuit works in test (shift) mode. The inputs from scan-in (SI) are shifted through the scan chain. The scan chain states can be shifted out through scan chain and observed at the scan-out (SO or Q) pin. The test program compares the SO values with expected values to verify the chips performance. 
Multiple scan chains are often used to reduce the time to load and observe. SFFs can be distributed among any number of scan chains, each having a separate scan-in (SI) and scan-out (SO) pin. The integrity of scan chains must be tested prior to application of scan test sequences.

<img width="701" alt="note1" src="https://user-images.githubusercontent.com/118954022/207884751-e775cf1f-5af7-408c-b28e-a116ec25da4f.png">

How long one single scan-chain can be ??

By chain length, it means number of flip-flops in a single scan chain.Larger the chain length, more the number of cycles required to **shift the data in and out**. However, considering the number of flops remains same, smaller chain length means more number of input/output ports is needed as scan_in and scan_out ports.

**Number of ports required = 2 x Num of scan chain**

**Number of cycles required to run a pattern = Length of largest scan chain in design**

**Num of patters to check = ( 2 ) ^ ( Num of flip-flops )**

**ATE ( Automatic Test Equipment )** - also known as **ATPG**(Automatic Test Pattern Generator). It is used due to we cannot check or test a large number of flip-flops manually. Lets say, there is 100 flip-flops, so 2^100 patterns need to be check, it will take months to complete check all of it. Basically a method used to find an input (or test) sequence that, when applied to a digital circuit, enables testers to distinguish between the correct circuit behavior and the faulty circuit behavior caused by defects. These algorithms usually operate with a fault generator program, which creates the minimal collapsed fault list, so that the designer needs not be concerned with fault generation. 

![web12](https://user-images.githubusercontent.com/118954022/207948908-3577744a-0cc2-44ff-a168-d85c18b0aac4.jpg)

Basic **ATE Functionality** :

![web11](https://user-images.githubusercontent.com/118954022/207948536-13f8c3d9-230c-45a2-8710-18884ab798d0.jpg)

1. Scan-In Phase - In each cycle, the next scan bit is applied serially to SI. On the clock edge, it is shifted in to the scan chain. Meanwhile, parallel outputs are masked.
2. Parallel Measure - PIs are applied early in the cycle. The clock remains inactive. The CUT is now in a known state. POs are measured late in the cycle.
3. Parallel Capture - The clock is pulsed once. This captures virtual PO data in the scan chain. The CUT is left in a dont care state. Captured bits are ready for scan out.
4. First Scan-Out Phase - With no clock, the SO port is strobed, measuring the first scanned-out bit.
5. Scan-Out Phase - In each cycle, the next captured bit is scanned out and measured at SO.

Basic ATPG flow :

![web4](https://user-images.githubusercontent.com/118954022/207937104-aef239a3-1a40-43f0-a0e1-2a69d5ba3e9d.jpg)
source:.sciencedirect.com

Overview of a **DFT Compiler** :

![note2](https://user-images.githubusercontent.com/118954022/207894356-c046d522-0172-49a9-ae33-6315fdb43ea1.jpg)

**Design Rule Checking (DRC)** - Verifies as to whether a specific design meets the constraints imposed by the process technology to be used for its manufacturing

How do we put the details to use or test them ??

That's where the proprietary tool **synopsys-DFT Compiler** comes into play. 

![note3](https://user-images.githubusercontent.com/118954022/207895576-8794e386-7ebc-4651-b19e-ee0347c9d263.jpg)

Some sample commands are (can find at synopsys documentation) :
* set_scan_configuration
* preview_scan
* insert_scan
* set_scan_path
* set_scan_signal .. and more.

Scan time of different scan chain lengths : 

![web8](https://user-images.githubusercontent.com/118954022/207944644-7f839277-3703-4e42-bccc-0523d0281ec5.jpg)

Other configurations of scan chains:
* Test power is a serious problem in the scan-based testing. DFT-based techniques and X-filling are two effective ways to reduce both shift power and capture power.
* In order to reduce test power and keep the defect coverage, Scan chain configuration based X-filling for low power and high quality testing.
* In this paper mentioned that the scan chain configuration tries to cluster the scan flip-flops with common successors into one scan chain, in order to distribute the specified bits per pattern over a minimum number of chains.

Design with faulty:

Metastability is a phenomenon of unstable equilibrium in digital electronics in which the sequential element is not able to resolve the state of the input signal; hence, the output goes into unresolved state for an unbounded interval of time. If the setup check is violated, data will not be captured properly at the next clock edge. Similarly, if hold check is violated, data intended to get captured at the next edge will get captured at the same edge.

My individual view on How DFT can be game changer for VLSI engineers:

In a design that having lot of logic gates, if there is one faulty logic in one of the circuit, it will lead to a big issue especially if the logic have multiple connection on it. The higher the test coverage, the higher the quality of the design. In timing aspect, the ealier the engineer found out where is the issue occur, the earlier the design can be fixed and fasten the launch process to market. If the test coverage is high and engineer can found out the issue before the chip is fabricated, then this can reduce the lost in cost.


--------------------------------------------------------------------------------------------------

# #Day_6

### Logic Synthesis

**Logic Synthesis** - is the process of automatic production of logic components, in particular digital circuits which that takes place in the transition from the register-transfer level (RTL) to the transistor level. It is a subject about how to abstract and represent logic circuits, how to manipulate and transform them, and how to analyze and optimize them. Synthesis is the process of converting a high-level description of design (Verilog/VHDL) into an optimized gate-level representation. Logic synthesis uses a standard cell library which have simple cells, such as basic logic gates like AND, OR, and NOR, or macro cells, such as adder, muxes, memory, and flip-flops.

**Synthesis = Translation + Optimisation + Mapping**

![note1](https://user-images.githubusercontent.com/118954022/208251188-7bb1cafc-89ab-4bef-8dbd-d5a972c2c7d7.jpg)

Logic Synthesis Overview : 

![note2](https://user-images.githubusercontent.com/118954022/208255713-af204133-8e0f-45e2-a847-c3f8b4aa395d.jpg)

**RTL Synthesis** - the simple RTL design undergoes synthesis to become a gate-level netlist with all of the designer-specified limitations. Synthesis, to put it simply, is the process of turning an abstract design into a correctly implemented chip in terms of logic gates. Multiple stages are involved in the synthesis.

**HDL Compiler** - translates Verilog HDL descriptions into Design Compiler witha GTECH library.

What is RTL in HDL ??

**RTL** “Register Transfer Level” code is a smaller subset of the full range of HDL code. RTL describes circuits at a level similar to the design description on a schematic: flip-flops activated by fully-specified clocks, and combinatorial logic (ranging from simple gates to large multipliers) between the flip-flops. Verilog is a "Hardware Description Language" **HDL**. It is a language used for describing a digital system like a network switch or a microprocessor or a memory or a flip−flop. It means, by using a HDL we can describe any digital hardware at any level. Writing in an **RTL coding style** means describing the register architecture, the circuit topology, and the functionality between registers.

Takeaways from RTL course :
* Labs using 'iverilog' and 'gtkwave'. We must ensure that it compiles properly using a verilog simulator and its waveform are as expected using gtkwave before attempting to 'synthesize' the verilog code. Only after the code passes the simulation phase, can move on to the synthesis phase of the ASIC design flow. 
* Good coding style will reduce most hazards while synthesis.
* Ensure synthesizable constructs are used in RTL.

Design Compiler short background :
* Synthesis EDA tool by Synopsys Inc.
* dc_shell for textual interface, and Design Vision for GUI.
* Synopsys understands .db format instead of .lib(human readable) for the standard library files.
* Design information can be stored in .ddc format (proprietary).
* **SDC** : Design intent in terms of power, timing and area constraints.
* SDC based on TCL.
* **Flow** : set and link .db, Read .v, Read sdc, integrate all the design information in terms of standard cell libraries provided, synthesize, report, QOR is as expected, write netlist.

Netlist and Libraries :
* Design written out in terms of standard cells (gates/flops/mux,etc.), as provided in .db.
* Target library: standard cell database (binary).. cell area/pins/timing data for synthesis decisions.
* It is generated for a specific process, temperature and voltage (a PVT corner).
* Various libraries can be appended together using link library. 

Getting start with DC :
* The differences in Yosys compare to previous labs, is that we have specify our target and link library instead of just reading the db file, and also take care of various file formats, while writing the netlist or/and ddc.  
eg: write-format ddc-hierarchy -o file.ddc
* Start-up Commands :
eg: For opening dc in non-GUI: 'dc_shell', for GUI: 'design_vision', after invoking csh, and to open GUI after opening dc_shell: 'gui_start'
* Will be having dummy libraries at begining if not provided.
* Uses GTECH lib to understand the logic when a Verilog file is read into it.
* For a standard design, multiple libraries at various PVT corner, different library for flops and different libraries for combo logic, can be specified. Linking helps in appending the relevant ones.
* **.synopsys_dc.setup** - can provide libraries during startup itself without any additional command specification.
What .synopsys_dc.setup defined :
-> link_library: the library used for interpreting input description.
-> target_library: the ASIC technology that the design is mapped to.
-> symbol_library: used during schematic generation.
-> search_path: the path to search for unsolved reference library or design.
-> synthetic_library: designware library to be used. 
* DC reads .synopsys_dc.setup files in order :
1. Synopsys installation directory (all user projects)
2. User home directory (all projects for this user)
3. Cureent project directory (this project only)

**TCL** Quick Tips :
* Strongly typed language, have to take care of spaces as well.
* Keep track of different bracket types. 
* While assigning no need to provide $, but while referring a variable in an expression use $. 
* Make a note of Synopsys proprietary TCL commands. eg: get_lib_cells and constructs like foreach_in_collection. 
* Collection and lists are different. **Collections** are not a standard part of TCL verbatim. If something is outputted in between '{}' as an output for a Synopsys command, it specifies a collection.
* Use Wildcards for big data-sets. eg: ' * ' matches any string of characters (including the empty string ). ab*cd, matches a string with ab at the start and cd ar the end. 

More info : http://viplab.cs.nctu.edu.tw/course/DCL2019_Fall/DCL_Mat_03.pdf 


--------------------------------------------------------------------------------------------------

### LABS

**LAB 1 - Invoking DC Basic Setup**

We will see how to invoke a DC, read various setup related files and write out a netlist. 

Start with >> cd ( get into home directory) ; mkdir -p training ; git clone https://github.com/kunalg123/sky130RTLDesignAndSynthesisWorkshop.git ; cd sky130RTLDesignAndSynthesisWorkshop ; /p/hdk/pu_tu/prd/sams/mig76_wlw/setup/enter_p31 -cfg ip76p31r08hp7rev03 -ov ./ ; cd DC_WORKSHOP/lib .We can see .lib and .db (which converted from .lib, DC understands .db only) files here.

![lab1 0](https://user-images.githubusercontent.com/118954022/208379552-08c8f8bc-90e9-4dfe-a2e6-7e1e1a26a14e.jpg)

Lets look at the content of .lib file. ( :syn off (to off the red highlighted)). PVT - process,voltage,temperature. Electronic Circuit Operation = f(Temp,VDD,Process) . So, the .lib is written out for a PVT corner and known as library of standard cells.

![lab1 1](https://user-images.githubusercontent.com/118954022/208426452-00976e64-a0eb-4e4f-8d5b-6780e81e4d52.jpg)

Then check the present verilog, >> cd .../DC_WORKSHOP/verilog_files ; ls 

To invoke dc_shell, need to enable cshell first, >> cd .../sky130RTLDesignAndSynthesisWorkshop ; csh ; dc_shell ; echo $target_library (this to read the technology library) ; echo $link_library (this is to pick the cells for the run) .We can see the compilers that is accesible. your_library.db is a imaginary non existent library. 

![lab1 2](https://user-images.githubusercontent.com/118954022/208436132-b649c672-0caf-44ad-b9be-cf77b6f28d56.jpg)

Read the design, >> read_verilog DC_WORKSHOP/verilog_files/lab1_flop_with_en.v .The file that gonna use in DC compiler is, in pg tab ( not in dc_shell tab) >> gvim DC_WORKSHOP/verilog_files/lab1_flop_with_en.v .The circuit drawn is the expected. It is 1 bit flip flop, asychn reset.

![lab1 3](https://user-images.githubusercontent.com/118954022/208441652-8f1d77d7-d9db-4e09-a55e-e74cb02024fd.jpg)

Next is to point a proper tech library, have to write verilog, >> write -f verilog -out lab1_net.v ; sh gvim /nfs/png/home/chiannio/training/sky130RTLDesignAndSynthesisWorkshop/lab1_net.v .As we see, we cant read the verilog link library as it is imaginary. GTECH - virtual library in DC's memory which is to understand the design. Because there was no proper standard cells it has written out the netlist in the form of the GTECH cells. The 'SEQGEN' should be Sky... .

![lab1 4](https://user-images.githubusercontent.com/118954022/208459818-37149aaf-c8b8-45e8-89aa-5c45c04fe5d4.jpg)

So, lets do and read the correct thing, >> read_db DC_WORKSHOP/lib/sky130_fd_sc_hd__tt_025C_1v80.db ; write -f verilog -out lab1_net.v ; sh gvim /nfs/png/home/chiannio/training/sky130RTLDesignAndSynthesisWorkshop/lab1_net.v ; and we will it is still the same in GTECH format. 

So , now we need to set variables , >> echo $target_library ; echo $link_library ; so we need this library from pointing your_library. So, >> set target_library /nfs/png/home/ppuspara/training/sky130RTLDesignAndSynthesisWorkshop/DC_WORKSHOP/lib/sky130_fd_sc_hd__tt_025C_1v80.db ; set link_library {* /nfs/png/home/ppuspara/training/sky130RTLDesignAndSynthesisWorkshop/DC_WORKSHOP/lib/sky130_fd_sc_hd__tt_025C_1v80.db} ; link ;
There may be multiple libraries loaded in DC’s memory. The ' * ' represents the exist library in that path that already loaded in DC's memory, so it wont overwrite it. Now after link , we can see it is linking and loading the design into the library pointed earlier.

![lab1 5](https://user-images.githubusercontent.com/118954022/208464607-1242ba3e-4abd-467a-a38d-197a4fcd727e.jpg)

Then compile the design, >> compile ; write -f verilog -out lab1_net.v ; sh cat lab1_net.v ; now we can see it is corrected already (cause we can sky... file). 

![lab1 6](https://user-images.githubusercontent.com/118954022/208465728-9960456f-3ae6-44ca-b97b-59bd673b49b5.jpg)


**LAB 2 - Intro to ddc gui with design_vision**

Launch design vision (supports gui format of dc) (not in dc_shell) , >> csh ; design_vision ; then write ddc (in dc_shell) for this >> write -f ddc -out lab1.ddc ; then in design_vision gui, >> read_ddc lab1.ddc ;

![lab2 1](https://user-images.githubusercontent.com/118954022/208477158-55cae19f-1100-4f85-b66a-26a52be73e5a.jpg)

Open another tab of design_vision , and read verilog there >> read_verilog DC_WORKSHOP/verilog_files/lab1_flop_with_en.v ; then compare it with ddc. Read verilog, it only reads verilog file. But read ddc , it automatically pick and load the design file. So, ddc saves all information in the tool memory in that particular session (snynopsis proprietary format).

To view the design, right click select schematic view, then double click the design appeared to view full design in detail. There was a inv connects to reset pin , because the flop is active low reset and we need active high reset. Now it is matching with the earlier expected circuit design.

![lab2 2](https://user-images.githubusercontent.com/118954022/208482005-41e41006-9ed2-4349-9994-d95df15786ce.jpg)


**LAB 3 - DC Synopsys DC Setup**  

Lets see on with dc setup options. Invoke dc first >> csh ; dc_shell ; echo $target_library ; echo $link_library ; set target_library /nfs/png/home/ppuspara/training/sky130RTLDesignAndSynthesisWorkshop/DC_WORKSHOP/lib/sky130_fd_sc_hd__tt_025C_1v80.db ; set link_library { * $target_library } ; echo $link_library ; echo $target_library .We can see the library is set.

![lab3 0](https://user-images.githubusercontent.com/118954022/208486541-d5438971-7eee-4e0f-90ff-4496f8e736d0.jpg)

So here we are having only one design, in real working, there are multiple .db files and cannot miss them. Setting lib every time manually is error prone. Solution: .synopsis_dc.setup .There will be 2 version, one in dc setup (default) , another one is at our homeuser directory. DC will pick up the one in our homeuser directory. All repetitive tasks which is needed for tool setup can be pointed in this file: target_library and link_library. 

Pre-configure must in home directory & the file name is .synopsys_dc.setup ,>> gvim .synopsys_dc.setup ; in the gvim file, insert as in below image, save and exit.
![lab3 1](https://user-images.githubusercontent.com/118954022/208489450-e84af38c-c295-4718-a4c7-7877fce44d21.jpg)

Then invoke dc_shell, we can see the target_library and link_library have been set automatically. >> csh ; dc_shell ; echo $target_library

![lab3 2](https://user-images.githubusercontent.com/118954022/208490072-7c841e6f-b398-4eba-a731-df7269ed8a54.jpg)


**LAB 4 - TCL Scripting**

Lest work on TCL. In dc_shell, set variables
![lab4 0](https://user-images.githubusercontent.com/118954022/208491137-de64001f-13d5-44cc-87d0-d381d3f44c72.jpg)

Next, we create a 'for' loop, must have space after each '}'. Carefull with $i .
![lab4 1](https://user-images.githubusercontent.com/118954022/208492332-f218961d-575b-485d-a48b-c4a006b92092.jpg)

Now for 'while' loop , there are 2 type which is shown in the image below. 
![lab4 2](https://user-images.githubusercontent.com/118954022/208494043-17ccb544-77db-4c19-9626-678fa694f6ba.jpg)

Now do 'foreach', lets create mylist, 
![lab4 3](https://user-images.githubusercontent.com/118954022/208494957-4ba4f5af-5949-4d0c-8d97-cdee68d5e06e.jpg)

Next is 'get_lib_cells' , load a file and look for a specific thing , eg: search for different types of 'and' in the loaded file: 
![lab4 4](https://user-images.githubusercontent.com/118954022/208496042-bb242381-f839-4f9f-aa86-985cfd5cc096.jpg)

Note: if the output printed print without {}, it mrefers to list, eg: a b c d . If the output printed with {} , it refers to a collection eg like the in pic above. 

The _sel3 is like a pointer for the above collection.
![lab4 5](https://user-images.githubusercontent.com/118954022/208496997-de4ad365-4b96-4b6a-9aef-58311d5bc115.jpg)

The get_object_name is used to retrieve value of the pointers.
![lab4 6](https://user-images.githubusercontent.com/118954022/208498117-2a2a6df6-8603-4106-b6b3-35bb35c320ae.jpg)

For this multiple commands, we can create a tcl also (save in a file and source it). >> sh gvim myscript.tcl ; source myscript.tcl .Before source, enter the info into the opened gvim file (save and exit).

![lab4 7](https://user-images.githubusercontent.com/118954022/208500393-3848f78a-948b-486f-93f5-de3a4a731432.jpg)

![lab4 8](https://user-images.githubusercontent.com/118954022/208500729-3c0a2ab4-cc39-4a48-96b5-a1817784473e.jpg)

Note: Becarefull with syntax ';' , the brackets and spacing in tcl file scripting. 


--------------------------------------------------------------------------------------------------

# #Day_7

### Intro to STA

Recaps :

**Setup Time**

Ensures that data is setup before the active clock edge occurs. Verifies that the signals don’t arrive too late, and the data is captured reliably. Timing relation between the latest possible data arrival time (longest or max data path) versus the required arrival time (**Slack** = Required arrival time - Actual Arrival time). Positive slack required to avoid violations. Helps identify the maximum frequency at which the design can operate. Often carried out at worst process corner under worst PVT conditions for yield considerations. Setup value of the flop usually specified as ‘library setup time’ in cell library.

**Hold Time**

Ensures that the data is held long enough at the capture flop so that it doesn’t capture the data being launched by the launch flop at the same edge. Short path analysis that ensures data doesn’t arrive too early. Compares the earliest arriving data with required arrival time of data. It is a same-edge test; neg slack preferred (Required arrival time - Actual Arrival time will be negative to avoid violations). Often conducted at the best process corner under best PVT conditions. Changing the cycle time doesn’t give a remedy to these violations. 

<img width="258" alt="note5" src="https://user-images.githubusercontent.com/118954022/208970448-0ab48273-61f2-440d-895d-3eb9b80c9b26.png">

source: Quora

**Basics Of STA** 

* **STA** - Static Timing Analysis. 
* Design functionality and its performance gets limited by noise, crosstalk and other such variations. 
* STA does a complete and exhaustive point to point analysis of the design. 
* To ensure that despite all possible pessimism in a design, the signals arrive neither too early, nor too late and the design maintains its correct operation.
* Static because it is input-vector independent -> STA basically tries to verify timing of a design without the use of input vectors.
* Doesn’t verify the functionality of the design.
* Provides a faster and simpler way of checking and analyzing all the timing paths in a design for any timing violations

![note6](https://user-images.githubusercontent.com/118954022/208972391-b05fd61a-6eb4-4264-9ef3-59168b1457ba.jpg)

* Design environment should be specified accurately to identify the timing issues :
  - Setting up clocks.
  - Setting up IO timing characteristics.
  - Specifying correct constraints. 
  - Specifying the correct exceptions (like false paths and multi-cycle paths).

![Note7](https://user-images.githubusercontent.com/118954022/208972423-082b51f3-5f61-4ba4-9217-14657a01df3c.jpg)

**Delays**

**Path** - multiple path in combinational logic, **Case** - interms of condition or PVT, **Min Delay** - shortest path and best case, **Max Delay** - longest path and worst case.

* **Transition Delay** - transition delay or slew is defined as the time taken by signal to rise from 10% (20%) to the 90%(80%) of its maximum value. This is known as “rise time”. OR “fall time” can be defined as the time taken by a signal to fall from 90%(80%) to the 10%(20%) of its maximum value. Transition is the time it takes for the pin to change state. 

* **Propagation Delay** - is the time required for a signal to propagate through a gate or net. Traditionally any gate propagation delay is measured between 50% of input transition to the corresponding 50% of output transition. Propagation delay depends on the input transition time (slew rate) and the output load. 

* **Cell/Gate Delay** - is the amount of delay from input to output of a logic gate in a path. STA tools calculate the cell delay from lookup tables provided in the technology library(.lib), which is a function of input transition and output load. The Tech libs model this delay values dependent on PVT (Process, Voltage and Temperature). This is needed in order to make the chip work in after fabrication in all possible conditions. 

* **Net Delay** - Net delay is the difference between the time a signal is first applied to the net and the time it reaches other devices connected to that net. It is due to the finite resistance and capacitance of the net. Hence calculated as a function of Resistance and Capacitance. 

*  Depends on Process and Temperature variation. These net delays are computed using WLM or SPEF dumped after routing. 

Input transition and Output Load : **Effect on IO Delays**

* Cell or gate delay is calculated using Non-Linear Delay Models (NLDM). NLDM is highly accurate as it is derived from SPICE characterizations. 
* The delay is a function of the input transition time (I.e. slew) of the cell, the wire capacitance and the pin capacitance of the driven cells. 
* A slow input transition time will slow the rate at which the cell’s transistors can change state logic 1 to logic 0 (or logic 0 to logic 1), as well as a large output load Cload (Cnet + Cpin), thereby increasing the delay of the logic gate.

**Timing Arcs**

* **Cell Arc** is between an input pin and an output pin of a cell I.e. source pin is an input pin of a cell and sink pin is the output pin of the same cell. Cell arcs can be further divided into sequential and combinational arcs.
* **Combinational Arcs** are between an input and output pin of a combinational cell or block. 
* **Sequential Arcs** are between the clock pin and either input or output pin. Setup and hold timing arcs are between the input data pin and clock pin of flip flop and are termed as timing check arcs as they constrain a form of the timing relationship between a set of signals. Sequential delay arc is between clock pin and output Q pin of FF. An example of a sequential delay arc is clk to q is called delay arc and clk to D input is called timing check arcs in sequential circuits. 
* **Net Arcs** - These arcs are between driver (cell) pin of a net and load pin of a net I.e. the source pin is output pin of one cell and the sink pin is input pin of another cell. Net arcs are always a **delay timing arcs**. 
* Each timing arcs has a timing sense that means how the output changes for different types of transitions on input, this is called unateness. **Unateness** is important for timing as it specifies how the output is responding for the particular input and how much time it will take. 
* For all the combinations of input and outputs and rising and falling conditions of inputs are defined in the .lib file. 
* **Timing Arc Unateness** are of three types:
  - Positive unate : AND, OR
  - Negative Unate : NOT, NAND, NOR
  - Non Unate : XOR

### What are constraints ??

**Timing Paths**

* **Timing Paths** are a collection of paths each having a start point and end point. 
* Valid timing paths based on valid start and end point are categorized into four types:
  - Input port to output port (Not recommended)
  - Input port to input of flop (IO Timing Path)
  - Clock pin of a flop to output port (IO Timing Path)
  - Clock pin of launch flop to input pin of capture flop (Reg2Regs)
* Timing paths are sorted into groups based on clocks associated with endpoint of path.

eg: 
![note8](https://user-images.githubusercontent.com/118954022/208975449-06dc1418-a4f1-4f99-b03a-012dea3955dd.jpg)

Timing paths : 
 
- REG 2 REG : Constrained by Clock
- REG 2 OUT : Constrained by Output External Delay, Output Load and Clock Period
-  IN 2 REG : Constrained by Input External Delay, Input Transition and Clock Period
-   Note    : The IO paths needs to be constrained for both Max delay (Setup) and Min Delay (Hold)

**Constraining the Design**

* STA cannot check any timing on a path that is unconstrained.
* So it is mandatory to give the IO port constraints to complete the timing of paths involving IO ports.
* Tclk -> q = 1.4ns, Tmax_path = 7ns, Tmin_path = 3ns
* At what time does the data arrive at input port : Tclk->q + Tprop_delay_ext_comb
  - set_input_delay - clock CLK -max 8.4ns [get_ports IN1]
  - set_input_delay -clock CLK -min 4.4 ns [get_ports IN1]

![note9](https://user-images.githubusercontent.com/118954022/208976233-5409381b-b789-4b9b-bbc2-6e8184467973.jpg)

* **Output Delay** is specified with respect to capture clock. 
* External logic’s setup requirement relative to CLK
  - set_output_delay -clock CLK -max [Max_Path_Time + Tsetup] [get_ports OUT1]
  - set_output_delay -clock CLK -max 14.8 [get_ports OUT1]
* Min external delay can also be specified by using -min option (external hold requirement)
  - set_output_delay -clock CLK -min [Min_path_time - Thold] [get_ports OUT1]
  - set_output_delay -clock CLK -min 3.6 [get_ports OUT1]

### IO Constraints : Inp Trans, Output Load 

We gonna see on **Advanced Synthesis and STA using Design Compiler IO Constraints**. 

Is IO Delay and Input Transition Modelling sufficient for IO Paths ?? 

Clock time - External time = Internal time = Input logic time + Setup time. Ideal signals has zero rise time. 

![note1](https://user-images.githubusercontent.com/118954022/208827565-45ff3217-2d03-49ea-a6d7-324c8638bbe6.jpg)

**Transition** plays a role at External Delay. If the input logic meets a transition, the delay will vary because cell delay is sensitive to the input transitions. 
**Cell delay** is a function of input transition. Non Zero rise time (pratical signal) will cause the input "input logic" delay to increase. So this will cause the input setup (setup time) at reg1 to fail. Setup violation is seen with practical transition (non ideal timing). 

![gogle1](https://user-images.githubusercontent.com/118954022/208842314-51918483-7288-4abc-a2db-17e805af8f21.jpg)

![note2](https://user-images.githubusercontent.com/118954022/208845059-d6a766f6-379a-4b00-92f4-00478ba73505.jpg)

Extra optimization need to be done in the input logic to let the DC module to know the practiccal transition is occuring at the input. This is time budgeting.

Lets see the output y flow now. Reacll, Cell Delay = funct(output load). Load plays a role at te output part, it is not an ideal net at output logic so need load to make the output behave correctly. 

![note3](https://user-images.githubusercontent.com/118954022/208862932-296c8299-a49c-4a72-81ca-ce9e54d33473.jpg)

So the Output Load increased the delay of output logic, thereby potentially causing setup failure at the receiving flop. So we need to inform to tool that there is going to be an output load, and need to squeeze the logic such that the output load is not going to delay the setup time.

![note4](https://user-images.githubusercontent.com/118954022/208864238-e12544ad-947c-4d3d-aea3-bf3898e996f4.jpg)

Next, how much load or transition need to model, it comes from the module. If it follows some regular interface, then it will has some regular specification. From this info we can know the answer. The ussual composition is 70% of external delay and 30% of internal delay. 

------------------------------------------------------------------------------------------------

### LABS

**LAB 1 - Timing dot Libs**

We going to explore the dot Lib and understand the informations. cd ...//DC_WORKSHOP/lib , open gvim the sky....80.lib file. Observe the informatios in the .lib file such as defaults, units, technology, operations, etc. 

![lab1 0](https://user-images.githubusercontent.com/118954022/208886862-fbf396a0-7fe6-434b-8764-78ac3ec6dc45.jpg)

default_max_transition : 1.5000000000. Let's understand this part. 

![lab1 1](https://user-images.githubusercontent.com/118954022/208897934-3cc8391f-f4cf-4ead-b299-3c76964ebbad.jpg)

If the cell loaded beyond the limit, the output may not rise at all (practical transition), so propagation delay would be very large and not acceptable. In nano second is acceptabel , but it goes large up to mili or micro seconds. If the delay is too large, the entire circuit operation will be jeopardized. We want to avoid this to happen. So we can see in .lib , the max capacitance limit = 1.5pf

All the capacitance load will add a kill, so we must Let know the DC to buffer or split the net. AS example like the below image. 

![lab1 2](https://user-images.githubusercontent.com/118954022/208901197-8434c4f0-e1ea-450e-95d8-6e20df29612c.jpg)

DC has to buffer the nets by knowing the max capacitance. If the gate is going to be heavily loaded such that the max capacitance limit is violated, DC will automatically sense and buffer the net. Since in .lib 1.5pf is very large value , hence 1.5pf is the last line of defence. We should never reach the lib limit cause it is very large , we can set it in the DC tools.

Lets understand about delay model : "table_lookup" , known as **Delay Model Lookup Table** or **'lut'**. The table is for every each cell. The delay will be present in the table of input trans (ns) vs output load (pf). The information will be presented in the .lib file. With two exact value of input trans and output load, interpolation done by taking the range from the table. 

![lab1 3](https://user-images.githubusercontent.com/118954022/208957089-6617df6b-38f8-4583-a473-80bcff60e392.jpg)

VNC knowledge: to split the gvim side by side , in gvim file type ' :vsp '

Let's observe two differentfalvours and2 gates. Tool only understand .lib not vlsi.Infos such as power pins, area, connections, leakage power, etc. Comparing the area; the widder the cell, the greater the area, the bigger the leakage area, the lesser the delay and capacitance. The timing window, Index 1 and index 2 is refering to the lookup table collums and rows respectively, and delays are shown there. 

![lab1 4](https://user-images.githubusercontent.com/118954022/208959083-e490359c-080c-4aaf-b11f-c0add7dd1ef4.jpg)

There is this, timing_sense : "positive_unate" and timing_type : "combinational" . It saya it is combinationational timing arc. **Unateness** . A **non-unatess** timing edge is a clock signal that passes through some sort of block that does not maintain the direction of the edge. A **positive unateness** : 'Rising Input' – Rising Output OR No change in Output. If we apply Rising signal to the input of a Timing Arc, corresponding output signal is either Rising or there is "No change".
A **negative unatess** - means cell output logic is inverted version of input logic. eg. In inverter having input A and output Y, Y is negative unate with respect to A.

Possitive unateness are AND and OR gates. NOT , NAND and NOR are negative unateness. XOR are non-unateness. It is possible for both positive and negative unateness to be in a gate (complex pin). Tools will know how to propagate based on this unateness. 

**LAB 2 - Exploring dot Lib Part1**

We going to see on details of the pins. /df - search for flop. We should see the clk2 timing delay which is seq timing arc. pin ("CLK_N") --> active low clk ; attribute clock : "true" --> pin is connected to the clock pin. Attribute driection is input (input pin). If we see pin ("D") , clock is false , means it is not a clock pin. 

![lab2 0](https://user-images.githubusercontent.com/118954022/209068568-7ae42e93-76ce-4bf9-aa23-c66862f19689.jpg)

For clk_N, the timing sense : non unate anf timing type : falling edge. This is because with respect to clock, Q maybe rising or falling depends on the input D pin. Q depends on D pin. We take posedge dff and negedge dff, clock to Q delay measured after the clock edge. Setup time is before the posedge and negedge. This informations is captured in the .lib so the tool knows it. CLK with rising edge is posedge clock and CLK_N with falling edge is negedge clock.   

timing_type : "setup_rising" --> means setup time is measured with respect to the rising edge. This is for the setup check for the specific flop. 

Invoke dc_shell to know the dff and latch names. (>> csh ; dc_shell ; echo $target_library ; get_lib_cells */* -filter "is_sequential==true" ). 'df' is flip flop and 'dlr' is latches. 

![lab2 1](https://user-images.githubusercontent.com/118954022/209090108-254e53e3-90d6-4153-bbe1-f57b9dc916ca.jpg)

Next, we see on latches. _dlrp --> positive latch , _dlrn --> negative latch. Setup is always before the sampling point. So, setup time of pos latch is with respect to negedge (falling). Setup time of neg latch is with respect to the posedge (rissing).

![lab2 2](https://user-images.githubusercontent.com/118954022/209091076-1381664e-5c15-4c12-990c-b7fac6954a92.jpg)

It is important to do setup calculation to with respect of which edge. 

**LAB 3 - Exploring dot Lib Part2**

We will look on how to vary the properties of .lib from the dc shell. List out what library loaded ( dc_shell >> list_lib ). It will show the library, file and path name. To know all the AND gate in the library: in collection form ( >> get_lib_cells */*and* ) ; in list form ( >> foreach_in_collection my_lib_cell [get_lib_cells */*and*] { set my_lib_cell_name [get_object_name $my_lib_cell]; echo $my_lib_cell_name; } ). 

![lab3 0](https://user-images.githubusercontent.com/118954022/209462258-bd734d32-e034-4590-bd04-19a7e3032682.jpg)

Not to do this , >> foreach_in_collection my_lib_cell [get_lib_cells */*and*] {echo $my_lib_cell}; as it will only list out the pointers. 

To know pins that is available for specific gate ( dc_shell >> get_lib_pins sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__and2_0/* ). For functionality of gate ( dc_shell >> foreach_in_collection my_pins [get_lib_pins sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__and2_0/*] {set my_pin_name [get_object_name $my_pins];      set pin_dir [get_lib_attribute $my_pin_name direction]; echo $my_pin_name $pin_dir; } ) or ( >>  get_lib_attribute sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__and2_0/X function )

![lab3 1](https://user-images.githubusercontent.com/118954022/209478275-b385fd6a-8fdb-42ad-9062-8689017f7997.jpg)

Writing script to print out output pin names and its functionality ( dc_shell >> sh gvim my_script.tcl ; source my_script.tcl ). Can also use to get attributes that we want, eg: area, capacitance, clock pin, etc.

To know all the attributes ( dc_shell >> list_attributes -app ; list_attributes -app > a ; sh gvim a & ). 

![lab3 2](https://user-images.githubusercontent.com/118954022/209478407-80aab570-c643-4cf7-aa85-35a2b9680ea0.jpg)


--------------------------------------------------------------------------------------------------

# #Day_8

## Clocks

### Querying Cells 

* The following example queries the cells that begin with o and references an FD2 library cell: (1)
* The following example shows that, given a collection of pins, we can query the cells connected to those pins: (2)
* The following example shows that, given a collection of nets, we can query the cells connected to those nets: (3)

![note1](https://user-images.githubusercontent.com/118954022/209571559-316aabd8-7d5f-4c8c-bc35-7a4449179a28.jpg)

### Clock Terminology 

Clock is built during **CTS** (Clock Tree Synthesis) only, till then the clock is an ideal network. 

![note20](https://user-images.githubusercontent.com/118954022/209626387-193dee25-b1c8-49e5-83bb-5541c61a1a72.jpg)

The difference in the arrival time of a clock signal at two different registers, which can be caused by path length differences between two clock paths, or by using gated or rippled clocks. Clock skew is the most common cause of internal hold violations. 

* **Clock skew** - Clock path delay mismatches which causes difference in the arrival of the clock.
* **Local Skew** - The difference in clock arrival between two consecutive/related pins of flops.
* **Global Skew**- The difference in clock arrival between the longest path and shortest path.
* **Positive Skew** - If the capture clock comes late than the launch clock.
* **Negative Skew** - If the capture clock comes early than the launch clock. 
* **Useful Skew** - If the clock is skewed intentionally to resolve setup violation.

![note2](https://user-images.githubusercontent.com/118954022/209571701-ad3e3023-22b1-412b-a7a2-52b29ce425a1.jpg)

**Clock Latency** - The total time it takes from the clock source to an end point.
* **Source Latency** - Is also called **Insertion Delay**. The delay from the clock source to the clock definition points.
* **Network Latency**-  The delay from the clock definition points (create_clock) to the flip-flop clock pins.

![note3](https://user-images.githubusercontent.com/118954022/209571802-819f7ae9-5f01-4234-b444-35500a9dea72.jpg)

* **Clock Jitter** - The short-term variations of a signal with respect to its ideal position in time. It is the variation of the clock period from edge to edge. It can vary +/- jitter value. Jitter value depends on the type of clock source. Stochastic variations of clock generation. 2 types:
   * Dutty Cycle Jitter varriation at on time, Ton of the clock.
   * Period Jitter - 
* **Clock Uncertainty** - Specifies a window within which a clock edge can occur. The uncertainty in the timing of  the clock edge is to account for several factors such as jitter and additional margins used for timing verification. Collectively clock skew and clock jitter is called clock uncertainty.

![note4](https://user-images.githubusercontent.com/118954022/209571863-dc4b7b5f-9e7f-4916-834c-98e1e85ad5fa.jpg)

### Clock Generation

All our clock sources will also have inherent variations in the clock period due to stochastic effects. There will be non-zero rise time, and the edge will arrive within a window, wherein the location of edge varies from cycle to cycle within window. This is known as jitter, meaning edge will arrive within a margin window and not at the exact time as expected. Because of this jitter, our timing will not be as expected as our margin will not be the same anymore.

Tclk - Tjitter >= Tcq + Tcombi + Tsetup

Clock sources such as Oscillator, Phase-Locked Loop (PLL) and external clock source. All the clock sources have inherent variations in the clock period due to stochastic effects. 

### Clock Skew

Practical Clock Tree - Clock Tree built during CTS. Ideal Clock Tree - Logic optimization happens in synthesis. Timing Clean path in synthesis may fail after STA. During synthesis, our timing will be clean, but once CTS is performed and the delays and clock skews are introduced, our available timing window will be eaten up. Thus we need to perform optimization with consideration to clock skew and jitter. Our timing delay now affected by the clock skew.

(Tclk - Tskew) => Tcq + Tcomb + T su .We can see the availabe timing window shrinks, path is timing clean before CTS, but fails after CTS which is not good.

![note21](https://user-images.githubusercontent.com/118954022/209626845-d6c895e1-1ad0-4bcd-bee0-2ac653963a21.jpg)

### Setting Up Clocks

By defining a clock, all internal timing paths (flop to flop) are constrained to operate in one clock cycle. Is a single cycle timing analysis from flop to flop (unless the constraints are relaxed in some exception cases – false and multicycle paths).

<img width="409" alt="image" src="https://user-images.githubusercontent.com/118954022/209572335-d52786e7-514c-4d95-ad30-37bd54b993e3.png">

Incase multiple clocks are used in the design, specify the timing relationship between the clocks. Specifying the skew/transition at the source of the clock (applies only to ideal clocks and are disregarded once the clock trees are built) : 
* - rise and -fall options to specify slew for rising and falling edges 
* - min and -max options to specify constraints in various operating conditions 

![note5](https://user-images.githubusercontent.com/118954022/209572526-b87472c5-7488-4922-a8a4-45572db42e9a.jpg)

Specify clock uncertainty that may be introduced due to jitter, skew and other pessimism when performing setup and hold checks. It models factors that effectively reduce the clock period: (1) . Inter-clock uncertainties foe clock domain boundaries will also take into account the skew between the clocks for setup and hold checks: (2)

![note6](https://user-images.githubusercontent.com/118954022/209573082-7bf8a476-c29d-45cf-b422-460e232f3888.jpg)

### Clock Latency

* 2 types: 
  * Source Latency (insertion delay) – (front clock source to clock definition pin)(could be on chip or off chip) 
  * Network Latency – (from clock definition point to clock pin of the flop) 
* **Total Latency = Source latency + Network latency**

<img width="401" alt="image" src="https://user-images.githubusercontent.com/118954022/209573311-9eb0bd3b-5fdb-4438-b09a-ee2b51da3eee.png">

* We can represent external delay through the longest (-late) , shortest (-early) paths and also with respect to rising (-rise) and falling (-fall) edges of the clock transition.
* Network latency gets ignored once the clock tree is built as it is the estimate delay of the clock tree prior to synthesis. (if set_propogated_clock command is set true)
* Source latency cannot be ignored.

![note7](https://user-images.githubusercontent.com/118954022/209573574-93c24656-b370-40ab-9fda-323c08eab836.jpg)

### Generated Clocks

* Such clocks are derived from master clock and are in phase with master clock. Eg: at outputs of divide-by-logic, to notify the STA tool regarding updated clock specifications).
* Major advantage – clock origin is still that of master clock  source latency specifications are automatically included.
* Creating a new master clock instead of generated clocks has below disadvantages : 
  * More clock domains to deal with 
  * Requires additional constraints to be specified 
  * Source latency specifications need to be defined all over again for the new master clocks.
  
 ![note8](https://user-images.githubusercontent.com/118954022/209573829-0be596ea-4f6e-486c-b2f0-fd796f821c28.jpg)

* Generated clocks can also be defined using clock -edge specifications and -edge shift specifications.

![note9](https://user-images.githubusercontent.com/118954022/209573950-35b44512-57fc-4cab-9863-57a7fb2077fe.jpg)

Clock Latency : 

* Source latency specified for the generated clock is from the master clock definition point to the generated clock definition point.
* Total latency = Source latency  of (Master clock + Generated clock) + Network latency of generated clock

![note10](https://user-images.githubusercontent.com/118954022/209574360-01f6c333-f4a6-4fbf-b57f-d3cd577e0a8f.jpg)

### Clock Modelling

Things need to model for the clock :

* Period
* **Clock Skew** - Clock path delay mismatches which causes difference in the arrival of the clock.
* **Source Latency** - Time taken by the clock source to generate clock.
* **Clock Network Latency** - Time taken by Clock Distribution network.
* **Jitter** - Random variation in clock source.

Post CTS, the clock network is real, and hence this modelled clock skew and clock network latency MUST BE REMOVED. In post CTS, clock uncertainty must only contains jitter. 

### Virtual Clocks

Is not associated with any pin or port, not a real clock but mimics the functionality of a real clock. It used as a reference to constrain the interface pins by relating the arrivals  at input/output port with respect to it with help of input and output delays. ROW_In is being timed by CLK_SAD. In such cases timing constraint at input port are specified with virtual clocks. Similar issue occurs at STATE_O :

<img width="339" alt="image" src="https://user-images.githubusercontent.com/118954022/209574453-aada48ed-15e1-4859-af64-e6b26155c013.png">

Once the virtual clocks have been defined, specify the IO delay with respect to virtual clock :

![note11](https://user-images.githubusercontent.com/118954022/209574528-68fca519-70b0-40f2-9d4e-b604877e39b7.jpg)

Note: for virtual clock, there is no latency , no clock definition point.

## Paths

### Timing Paths

* Reg-to-reg: constrained by clock -> clock period
* Reg-to-output: constrained by output external delay, output load and clock period
* Input-to-reg: constrained by input external delay, input transition and clock period

### False Paths

Certain timing paths are not real/possible and need to be excluded from STA as they don’t occur during the functional operation of the design. Such paths are turned off in STA as false paths. Advantage : reduces the analysis to focus only on real paths. Eg: a clock pin of a flip flop to the input of another flip flop ; a few paths that are architecturally not possible. 

![note12](https://user-images.githubusercontent.com/118954022/209574835-7131a60b-ab4e-46a7-a58b-ed404953575c.jpg)

###  Half-cycle Paths 

If the design has both positive and negative edge triggered flops, such path might exist. It could be from rising edge of a flop to the falling edge of another flop. Data path gets only half a cycle for setup check (more stringent condition). The hold check gets relaxed by half a cycle  resulting in slack met with a large value.

![note13](https://user-images.githubusercontent.com/118954022/209575001-67290df2-741b-4f9b-bf57-c6c896e43ec5.jpg)

### Multicycle Paths  

In some cases, the combinational path between two flops may take longer than one cycle to propagate through the logic. We direct the STA tool that the relevant capture edge occurs after some specified number of clocks.

![note14](https://user-images.githubusercontent.com/118954022/209575137-18ed36e1-3c0f-4071-92ff-feec9a187060.jpg)

Here considering default checks would lead to a lot of violation  declare the path as a multicycle exception for setup checks and move the setup capture edge to 3rd edge. However, multicycle exception will move both setup (to 3rd edge) and hold edge (to 2nd edge). Eg: to the edge before setup capture edge.

![note15](https://user-images.githubusercontent.com/118954022/209575352-98edae6e-8ee9-443a-93d2-eb287b193f38.jpg)

This is not the correct way as the hold check should remain at the 0th edge, eg: should be same setup launch edge so we need to define MCP again to bring back hold edge to 0th edge. 

![note16](https://user-images.githubusercontent.com/118954022/209575355-95e490cd-36bf-4df9-83ad-a70ec87bbf60.jpg)

## Asynchronous Timing Checks 

### Removal Time 

Related to asynchronous control signals like asynchronous reset. It ensures there is adequate time between an active edge of clock and release of the asynchronous signal. This is done to ensure the clock edge has no effect and does not cause any change in the values. It is a min path check like hold check. Timing checks are based on the removal time specified in the asynchronous pin of the flop in cell library as ‘library removal time’. All asynchronous timing checks are assigned to default path groups and the endpoint shows it is a removal timing check.

![onenote1](https://user-images.githubusercontent.com/118954022/209569245-190cb7a4-cbdd-4cc0-aada-3e031f3b58e3.jpg)

### Recovery Time 

Ensures that there is minimum amount of time between asynchronous signal becoming inactive and arrival of next active edge of clock. It also ensures that once the asynchronous signal inactivates, the design has enough time to recover and respond back to the clocks. Defined in the cell library of the asynchronous pin of the flops as the ‘library recovery time’. Max path check like the setup clock. Endpoint in the report indicates the check is a recovery check against the clock. Here also the timing path group is ‘async_default’ path group. 

![onenote2](https://user-images.githubusercontent.com/118954022/209569305-8119e819-8b2a-4346-9b2f-72113e0bf60f.jpg)

## IO Delays

DC takes constraints in the form of **SDC** (Synopsys Design Constraints). Ports are the primary IOs of the design for the inputs and outputs. Keep in mind that the attributes will be case sensitive. We use the commands set_input_delay and set_input_transition on our input ports to constrain the IO paths. Similarly for output ports, we need to use the command set_output_delay and set_output_load for constraining the IO path. Command of get query ports in DC, 'get_ports' ,while command of getting clocks in DC, 'get_clocks'. 'filter' used to set condition for the outcomes. Clock dont have attributes in or out , it only has 'period'.

![note18](https://user-images.githubusercontent.com/118954022/209624513-b2d7ca57-77fd-4b5c-a104-54f656e3659f.jpg)

Net is connection of 2 or more pins and ports. Pins are the with pointed by letters or numbers. 

![note17](https://user-images.githubusercontent.com/118954022/209622456-2fbfa772-5d3e-465e-bb49-09d830b8a76b.jpg)

( get_cells * -hier) - will list all the cells. 

![note19](https://user-images.githubusercontent.com/118954022/209625131-bb9ef847-100b-4af9-a4d1-05e23295ac56.jpg)

To check wethwer it s hier cell or physical cell. eg: as below in the image. The first will how as true and the second one will show as false due to it is not a hier cell.

<img width="281" alt="image" src="https://user-images.githubusercontent.com/118954022/209625424-e25fc63b-30ac-484e-b27f-220f8c3db6b9.png">

In Clock Distribution , the command to create clock is 'create_clock -name <clock name> -per <period(ns)> [clock definition point]' ,eg: 'create_clock -name MY_CLK -per 5 [get_ports CLK]' .Clock must be created on a valid clock generators (PLL, Oscilator) or Primary IO Pins (for external clocks) , and not be created on hierarchical pins which are not clock generators. 

Bringing in the practicalities (latency, uncertainty,..) of clock network. Set skew and jitter. This needs to be modified post CTS to reflect only Jitter. 

<img width="442" alt="image" src="https://user-images.githubusercontent.com/118954022/209643968-8d8f28c3-6671-47ec-bdfe-9dafc461bb30.png">

Overall summarize : create_clock; set_clock_latency; set_clock_uncertainty (Pre and Post CTS); set_input_delay; set_input_transition; set_output_delay; set_load; get_ports; get_clocks; get_cells. 

### Clocks waveform.
  
![note22](https://user-images.githubusercontent.com/118954022/209645614-a93df095-7c0d-497e-8386-78b8a5864669.jpg)

### Constraining the IO paths. 
  
Input transition and input delay need to modelled based on what the correct thing it is, depends on the design. So below images , the max min numbers are based on the design , not a constant number to be use anywhere. Input and output constraints :
  
<img width="365" alt="image" src="https://user-images.githubusercontent.com/118954022/209657702-bbeb17ff-16ec-4af3-ae68-5ee98ba0d96b.png">
  
<img width="374" alt="image" src="https://user-images.githubusercontent.com/118954022/209658371-93f69206-0aad-4ac0-b5a4-6a6ad9873db4.png">

## generated_clk 

Let's say the spec for the output out_y as below image. Looking at the output path, the output y is constrained with the clock leaving the module. Logically it is same as MY_CLK defined at port clk but physically it is not. Due to it going to suffer routing delay, uncertainty or latency is not modelled here, so there will be Propogation Delay. 
  
![note23](https://user-images.githubusercontent.com/118954022/209680882-01a56478-747f-40bb-a48e-1ce16b7584be.jpg)

We going to generate clock. Generated clocks are always create with respect to master clock (clock source or primary IO pins). ' -div 1 ' - this telling that there is no clock divider, this is Division Value of generated clock (useful for clock dividers). 
  
![note24](https://user-images.githubusercontent.com/118954022/209681289-961f4da7-8b68-49dc-820b-1b53d71c0503.jpg)

Constraining the design. SEL (selections) is to select which data input to take. SEL wont toggle actively. OUT DATA can come w.r.t CLKA or CLKB. 
  
![note25](https://user-images.githubusercontent.com/118954022/209682235-93baac38-d413-4504-a680-15d92ebccbff.jpg)

IN_DATA, IN_CLK has 2 functionalities:
* In one functionality the IN_DATA and IN_CLK gets the data and clock corresponding to A and in other functionality it gets data and clock corresponding to B.
* Same for OUT_DATA, OUT_CLK (can get from A or B).
* Selection line is common.
  
How the clocks are propogated: 
* Once a clock is created on a pin/port, DC will propogate that clock downstream based on the timing arcs.
* All the timing arcs from the definition point will see the clock propogate by default.
* Both wont work simultaneously, when A works , input only goes thru A. 

## vclk, max_latency, rise_fall IO Delays
  
### INPUT DELAYS : 
set_input_delay -max 3 -clock myclk [gets_port IN_A]
set_input_delay -max -3 -clock myclk [gets_port IN_A]
set_input_delay -min 1 -clock myclk [gets_port IN_A]
set_input_delay -min -1 -clock myclk [gets_port IN_A]
  
### OUTPUT DELAYS :
set_output_delay -max 3 -clock myclk [gets_port IN_A]
set_output_delay -max -3 -clock myclk [gets_port IN_A]
set_output_delay -min 1 -clock myclk [gets_port IN_A]
set_output_delay -min -1 -clock myclk [gets_port IN_A]
  
### IO Constraints revisited 
***No clock definition point -> virtual clock inferred . Note: for virtual clock, there is no latency , no clock definition point. create_clock; set_input_delay; set_output_delay; set_driving_cell; set_input_transition;  -> will discuss in detail in labs. 
  
------------------------------------------------------------------------------------------------

## LABS

### LAB 1 - Loading Designs (get cells, ports and nets)

the code (design diagram) we are going to use >> gvim lab8_circuit.v ; observe the code and try to understand it refering to its circuit design. 3 Regs, Output logic - inverter, input logic - Or and XOR gate, comb logic - NAND gate.

![lab1 0](https://user-images.githubusercontent.com/118954022/209704031-6dac2954-7dfa-4590-81d3-fa3d8cabd34a.jpg)

In dc_shell >> echo $target_library; echo $link_library; read_verilog lab8_circuit.v; (check the reg listed, must be successfull); link; compile_ultra; (opimization completed, design compiled perfectly); get_ports; (get all ports, 6 ports); foreach_in_collection my_port [get_ports *] { set my_port_name [get_object_name $my_port]; set dir [get_attribute [get_ports $my_port_name] direction]; echo $my_port_name $dir; } ; (to know ports with its direction);
  
![lab1 1](https://user-images.githubusercontent.com/118954022/209763412-f172446b-766a-4527-bb3f-1d8e2efa4e3f.jpg)

To get cells and check wether it is hier or not (false means it is not hier), >> get_cells * ('*' - this refers to alll); get_attribute [get_cells REGA_reg] is_hierarchical ; (check one by one),  get_cells * -filter "is_hierarchical == false" ; get_cells * -filter "is_hierarchical == true" ; (check overall (also can replace '*' by '-hier', so there is no hier cell since all false).
  
![lab1 2](https://user-images.githubusercontent.com/118954022/209764727-5d6cecfc-eb2d-4df8-b3b2-23824644a7a1.jpg)

To get reference name of cells in library, >> get_attribute [get_cells REGA_reg] ref_name; (for one), foreach_in_collection my_cell [get_cells * -hier] { set my_cell_name [get_object_name $my_cell]; set rname [get_attribute [get_cells $my_cell_name] ref_name]; echo $my_cell_name $rname; } ; (for all). ' dfrtp ' - df (D flip flop), r (reset) , t (true output, is Q, not Q bar) , p (posedge).
  
![lab1 3](https://user-images.githubusercontent.com/118954022/209766538-924128d3-a2cc-4bc2-962d-ef8168960ee8.jpg)

Write in ddc format and launch design, in dc_shell>> write -f ddc -out lab8_circuit.ddc ; in tab >> csh; design_vision; (in design vision tab); read_ddc lab8_circuit.ddc 
  
![lab1 4](https://user-images.githubusercontent.com/118954022/209769163-d79a45a9-a7f2-4a7d-9a03-9ed54aae4fde.jpg)

### LAB 2 - (get pins and clocks, querying_clocks)

To get pins, dc_shell>> get_pins * ; foreach_in_collection my_pin [get_pins *] { set pin_name [get_object_name $my_pin]; echo $pin_name; } ; get_attribute [get_pins REGA_reg/RESET_B] direction ; (to know the direction attributes), get_attribute [get_pins REGA_reg/RESET_B] clock ; (to know it is a clock pin or not), foreach_in_collection my_pin [get_pins *] { set pin_name [get_object_name $my_pin]; set dir [get_attr [get_pins $pin_name ] direction]; echo $pin_name $dir; } ;(directions for all the pins)
  
![lab2 0](https://user-images.githubusercontent.com/118954022/209784165-46e5b4c4-c9e3-4c5e-a87a-dcace5039956.jpg)

To filter search, like set dir in and clk pin, >> foreach_in_collection my_pin [get_pins *] { set pin_name [get_object_name $my_pin]; set dir [get_attr [get_pins $pin_name] direction]; if { [regexp $dir in] } { if { [get_attr [get_pins $pin_name] clock] } {  echo $pin_name; } } } .The command 'regexp' is for shows that certain pairs pattern are matching, matches(1) or not(0). 
  
![lab2 1](https://user-images.githubusercontent.com/118954022/209794804-d66e2fb5-1723-4bf9-8e1e-62fc512346f5.jpg)

Get_clocks wont show cause clocks not created, will create in next lab. Now, querying clocks, dc_shell>> sh gvim query_clock_pin.tcl (copy the above filter search into this tcl file); source query_clock_pin.tcl

![lab2 2](https://user-images.githubusercontent.com/118954022/209799129-a6370c19-bcba-4220-8425-0e21f23fa6b2.jpg)

>> get_attribute [get_pins REGB_reg/CLK] clocks ; get_attribute [get_pins REGB_reg/CLK] clock .The difference is, clocks -what are the clocks that reaching the pin, clock - wether the pin is meant to be a clock pin or not. 
  
![lab2 3](https://user-images.githubusercontent.com/118954022/209800521-38138cb5-6be9-4c22-8e90-f200e2a4879c.jpg)

### LAB 3 - Create Clock Waveform
  
Check dc_shell >> get_ports * ; current_design (name of top module);Then create clock waveform >> create_clock -name MYCLK -per 10 [get_ports clk] ('1' means clock is successfully created); get_clock * ; get_attr [get_clocks MYCLK] period ; get_attr [get_clocks MYCLK] is_generated (false, cause it is a master clock); report_clocks ;

![lab3 0](https://user-images.githubusercontent.com/118954022/209845466-e3f424ea-4544-4b6f-89bb-7fed61f37cba.jpg)

Now, >> source query_clock_pins.tcl ; get_attribute [get_pins REGB_reg/CLK] clocks ;Now it wil show ' {MYCLK}, due to the clock has created.

Next modify the tcl script, get object name for clk, will get the clock name created, >> sh gvim query_clock_pin.tcl & ; (edit the tcl file); 

![lab3 1](https://user-images.githubusercontent.com/118954022/209853458-3b73a401-1d3c-4b10-9a77-19bab389c20b.jpg)

If say we created a wrong clock, to remove it >> remove_clock <clock name> .Lets see on waveform, new clock named MYCLK1 created with different waveform. 

![lab3 2](https://user-images.githubusercontent.com/118954022/209854709-a7b404ac-bb6f-46c6-8ea3-a576101af229.jpg)

### LAB 4 - Clock Network Modelling (uncertainty, report_timing)

Modelling source for clock in design, >> set_clock_latency -source 1 [get_clocks MYCLK]  (modelling source latency); set_clock_latency 1 [get_clocks MYCLK]  (modelling network latency); Then set uncertainty and min, >> set_clock_uncertainty 0.5 [get_clocks MYCLK] ; set_clock_uncertainty -hold 0.1 [get_clocks MYCLK] ;

![lab4 0](https://user-images.githubusercontent.com/118954022/209857772-14b611b2-6e2a-4d25-93a1-2bc05df8c980.jpg)

If remove all clocks, then >> report_timing ,it will show the (Path is unconstrained). Path will only be constrained when thr is clock. Based on the report, we can observe the timmings. Slack is to be met based on the formula calculation. 

![lab4 1](https://user-images.githubusercontent.com/118954022/209859506-059f5e03-fa12-4cbb-a834-129e94f0164f.jpg)

Model pratical efforts of the clock, >> set_clock_latency -source 2 [get_clocks MYCLK] ; set_clock_latency 1 [get_clocks MYCLK] ; set_clock_uncertainty -setup 0.5 [get_clocks MYCLK] ; set_clock_uncertainty -hold 0.1 [get_clocks MYCLK] ; report_timing ; Then compare the report timing , observe slack and so on. (skew and jitter exists)
 
![lab4 2](https://user-images.githubusercontent.com/118954022/209861143-0a37fbea-73e5-493d-8565-83b27e58000c.jpg)

### LAB 5 - IO Dealys

From previous lab , report_ timing will show the path constrained from regB to RegC. If >> report_timing -from IN_A ,or, -to out_y ; the path is unconstrained. Because no IO delay given to the ports. To review details of all ports, dc_shell >> report_port -verbose .The dash and blanks due to not model some stuffs.
  
![lab5 0](https://user-images.githubusercontent.com/118954022/209864453-27a52426-63b3-4bee-83b5-0b55c05d6dbd.jpg)

So we start modeling, >> set_input_delay -max 5 -clock [get_clocks MYCLK] [get_ports IN_A] ; set_input_delay -max 5 -clock [get_clocks MYCLK] [get_ports IN_B] ; report_port -verbose ;The input delay max is modelled. And report_timing -from IN_A path is constrained now.
  
![lab5 1](https://user-images.githubusercontent.com/118954022/209865559-7314416b-f8b0-4e42-be5a-e8c25ae3886a.jpg)

Modelling transition delay for path, >> report_timing -from IN_A -trans -cap -nosplit ; To see the whole timing, >> report_timing -from IN_A -trans -cap -nosplit -delay_type min , the path is unconstrained, this is because we not model yet any of the min.

![lab5 2](https://user-images.githubusercontent.com/118954022/209866547-053fcb5a-afeb-4253-bd31-90d73d479de8.jpg)

Model the min, >> set_input_delay -min 1 -clock [get_clocks MYCLK] [get_ports IN_B] ; set_input_delay -min 1 -clock [get_clocks MYCLK] [get_ports IN_A] ; report_timing -from IN_A -trans -cap -nosplit -delay_type min ; it is constrained now.
  
![lab5 3](https://user-images.githubusercontent.com/118954022/209867351-01f93736-fa85-4b7c-af42-f0db2a2e5163.jpg)

Now pick input transition, >> set_input_transition -max 0.3 [get_ports IN_A] ; set_input_transition -max 0.3 [get_ports IN_B] ; set_input_transition -min 0.1 [get_ports IN_A] : set_input_transition -min 0.1 [get_ports IN_B] ; report_timing -from IN_A -trans -cap -nosplit > a_trans ; then compare both reports.
  
<img width="35" alt="image" src="https://user-images.githubusercontent.com/118954022/209868287-bce1aba5-f813-459c-bd94-b123a082a5b2.png">

Moddeling output delays, >> set_output_delay -max 1 -clock [get_clocks MYCLK] [get_ports OUT_Y] ; set_output_delay -max 5 -clock [get_clocks MYCLK] [get_ports OUT_Y] ; set_output_delay -min 1 -clock [get_clocks MYCLK] [get_ports OUT_Y] ; report_timing -to OUT_Y -cap -trans -nosplit > out_Y ; Then modelling the output load path, >> set_load -max 0.4 [get_ports OUT_Y] ; report_timing -to OUT_Y -cap -trans -nosplit > out_load ;Then observe the reports.

### LAB 6 -  Generated_clocks

Creating generated clock , dc_shell>> create_generated_clock -name MYGEN_CLK -master MYCLK -source [get_ports clk] -div 1 [get_ports out_clk] ; report_clocks * ;The 'G' in attr refers to 'generated'. MYGEN_CLK , if we do >> get_attr [get_clocks MYGEN_CLK] is_generated , it will show "true" because it is a generated clock, not a master clock. 
  
![lab6 0](https://user-images.githubusercontent.com/118954022/209869001-b2841f39-906f-4f7b-80b5-c5b055f001cc.jpg)

Next, to make timing path capture data at generated clock (MYGEN_CLK) instead of master clock (MYCLK), >> set_output_delay -max 5 [get_ports OUT_Y] -clock [get_clocks MYGEN_CLK] ; set_output_delay -min 1 [get_ports OUT_Y] -clock [get_clocks MYGEN_CLK] ; report_timing -to OUT_Y ; 
  
![lab6 1](https://user-images.githubusercontent.com/118954022/209871886-c41eab82-8957-41c1-9d8a-85dab9f952b2.jpg)

Then, reset design and read another design (lab8_circuit_modified), write a tcl with design constraints and source it, >> sh gvim lab8_circuit_modified.v  (copy from lab8_circuit.v and modify); reset_design ; read_verilog lab8_circuit_modified.v ; sh gvim lab8_cons.tcl & (copy from lab8_cons.tcl and paste, no modify); link ; source lab8_cons.tcl ;  report_clocks (we can see the waveform got automatcally generated).
  
![lab6 2](https://user-images.githubusercontent.com/118954022/209874508-beebb02d-99cf-422c-9152-fa7e0b3970b4.jpg)

See all generated clocks >> get_generated_clocks ,and see full report >> report_port -verbose

### LAB 7 - Set_max_delay

>> reset_design ; The file we going to use is, >> sh gvim lab14_circuit.v ; read_verilog lab14_circuit.v ; current_design (the lab name is still lab8); source lab8_cons.tcl ; report_clocks ; link ; compile_ultra ; report_timing (check all clk is present); everything is proper now. 

![lab7 0](https://user-images.githubusercontent.com/118954022/209948440-429ebfa3-9d5e-40bd-be20-264570bcaeb6.jpg)

So now, >> get_ports * ; report_timing -to OUT_Z ; (path is unconstrained) , 

![lab7 1](https://user-images.githubusercontent.com/118954022/209948794-d05e65ec-c7ff-4403-97d5-fe182c611985.jpg)

Before constrained it , let look at list all commands in the design , >> all_inputs ; all_outputs ; all_registers ; all_clocks ; all_registers -clock MYCLK ; all_registers -clock MYCGEN_DIV_CLK ; 

![lab7 2](https://user-images.githubusercontent.com/118954022/209949937-4b352f33-2be8-4eae-99c0-97739c3e4fa4.jpg)

Then lets constrained it, >> report_timing -from IN_A -to OUT_Z ; report_timing -from IN_B -to OUT_Z ; report_timing -from IN_C -to OUT_Y ; There wont be any path. To see fanout of registers (endpoint) and can review how timing path start and ends, >> all_fanout -flat -endpoints_only -from IN_A ; all_fanout -from IN_A ; foreach_in_collection my_points [all_fanout -from IN_A] { set my_pnt_name [get_object_name $my_points]; set my_cell_name [get_attribute [get_cells -of_objects [get_pins $my_pnt_name]] ref_name]; echo $my_pnt_name $my_cell_name; } ;(to get all 9 listed). All fanout giving the collection of pins, then getting the object and cell name. 

![lab7 3](https://user-images.githubusercontent.com/118954022/209954647-49f1b4d2-7c51-4830-a4f0-80f6ae978043.jpg)

There is only 2 endpoints in the design, >> all_fanout -flat -endpoints_only -from IN_A ( to check in pins of an endpoint, >> all_fanin -to REGA_reg/D )

<img width="255" alt="image" src="https://user-images.githubusercontent.com/118954022/209955141-54901cef-7ca5-4bc5-8373-d9a0e37e7e9e.png">

Lets constrained OUT_Z , >> set_max_delay 0.1 -from [all_inputs] -to [get_port OUT_Z] ; report_timing -to OUT_Z -sig 4 ;(sig - refers to significant digit). We can see the slack is violated and the path is now constrained.  so, >> compile_ultra ;  report_timing -to OUT_Z -sig 4 ;the slack is now met. 

![lab7 4](https://user-images.githubusercontent.com/118954022/209958015-9630fb41-6513-4139-a0d0-255dfcea12e4.jpg)

Write ddc and review the schematic, >> write -f ddc -out lab14.ddc ; reset_design ; read_ddc lab14.ddc ; gui_start ;(the path is added to the schematic). 

![lab7 5](https://user-images.githubusercontent.com/118954022/209964140-0c03114b-3021-461b-bfa6-31ffedb87e5a.jpg)


### LAB 8 - VCLK

Virtual clock dont have definition point (source). The path OUT_Z need to optimize properly. So, >> create_clock -name MYVCLK -per 10 ; reset_design ; read_verilog lab14_circuit.v ; link ; source lab8_cons.tcl ; compile_ultra ; report_timing -to OUT_Z ; then now create virtual clock, >> 

![lab8 0](https://user-images.githubusercontent.com/118954022/209998017-1cdff650-38e5-473c-b45f-0fe9f35c07bb.jpg)

then now create virtual clock, >> create_clock -name MYVCLK -per 10 ; report_clocks ;(There is no source, this is how we know it is virtual clock) 

![lab8 1](https://user-images.githubusercontent.com/118954022/210003103-15ea80a4-2ddf-461d-8ff1-8bcc052d7d0c.jpg)

Set IO delays, >> set_input_delay -max 5 [get_ports IN_C] -clock [get_clocks MYVCLK] ; set_input_delay -max 5 [get_ports IN_D] -clock [get_clocks MYVCLK] ; set_output_delay -max 4.9 [get_ports OUT_Z] -clock [get_clocks MYVCLK] ; report_timing ;(slack is violated with -0.02ns). Then >> compile_ultra ; report_timing -to OUT_Z -sig 4;  report_port -verbose ;

![lab8 2](https://user-images.githubusercontent.com/118954022/210005941-6aeae48f-9646-4913-92fb-991f5b11eb52.jpg)
![lab8 3](https://user-images.githubusercontent.com/118954022/210006277-57564844-d9af-4b0e-b780-80d74e23f407.jpg)


--------------------------------------------------------------------------------------------------

# #Day_9

Recap :
* Combinational Optimization is still very much Boolean optimization.
* In DC, Querying makes job easier for manual cell replacement.
* Replication and reuse of logic can be done for resource sharing, always be cautioned about over-constraining, may lead to explosive area increase.
* Sequential Optimization remains an exercise in timing plus Boolean optimization
* Explicit representation of tie cells to represent constant assignment is an addition here.
* Also, sequential constant propagation can be limited via [compile_seqmap_propagate_constants](#) set as false.

## Synopsys Directives

### Embedding Constraints and Attributes

* Constraints and attributes, usually entered at the dc_shell prompt, can be embedded in your Verilog source code. Prefix the usual constraint or attribute statement with the Verilog comment characters //, and limit the embedded statements with the compiler directives [// synopsys dc_script_begin](#) and [// synopsys dc_script_end](#). 

![note1](https://user-images.githubusercontent.com/118954022/210098943-cb7935d0-5abb-40a9-81eb-609445e7d708.jpg)

The following limitations apply to the use of constraints and attributes in your design:
*Constraints and attributes declared outside a module apply to all subsequent modules declared in the file.
*Constraints and attributes declared inside a module apply only to the enclosing module.
*Any dc_shell scripts embedded in functions apply to the whole module.
*Include in your dc_shell script only commands that set constraints and attributes. **Do not use action commands such as compile, gen, and report**.

### Synopsys Full_case

* When adding "full_case" or "parallel_case" directives to a case statement, the directives are added as a comment immediately following the case expression at the end of the case statement header and before any of the case items on subsequent lines of code.
* From a synthesis tool perspective, a **full case** statement is a case statement in which every possible binary pattern is included as a case item in the case statement.
* Synopsys parses all Verilog comments that start with "// synopsys ..." and interprets the "full_case" directive to mean that if a case statement is not "full" that the outputs are "don't care's" for all unspecified case items. If the case statement includes a case default, the "full_case" directive will be ignored.

### Synopsys Parallel_case

* A **paralle case** statement is a case statement in which it is only possible to match a case expression to one and only one case item. If it is possible to find a case expression that would match more than one case item, the matching case items are called "overlapping" case items and the case statement is not "parallel.“
* In general, use parallel_case when you know that only one case item is executed.
* Under certain circumstances, you might not want to build a priority encoder to handle a case statement. You can use the parallel_case directive to force HDL Compiler to generate multiplexer logic instead.

## Retiming / Pipelining

*	Registers stop glitches from propagating through combinational paths. 
*	Pipelining is a technique that breaks combinational paths by inserting registers. 
*	By reducing logic-level numbers between registers, pipelining can result in higher clock speed operations. However, pipelining increases the latency of a circuit in terms of the number of clock cycles to a first result.

![note2](https://user-images.githubusercontent.com/118954022/210099337-d491c140-6aaa-48a2-a749-55d749cb4194.jpg)

*	Retiming as an algorithm allows shortening of critical paths.
*	After providing a proper timing constraint file (consisting of clock definitions, clock uncertainty modelling, io delays and load) and observing a scope of retiming, we can provide the DC switch [compile_ultra –retime](#), to see the results.

![note3](https://user-images.githubusercontent.com/118954022/210099352-1c56e650-3fe7-460c-a86e-bb41439944b3.jpg)

## Boundary Optimization

* [Set_boundary_optimization module_sub false](#)
* It is helpfull in ECOs.

<img width="159" alt="image" src="https://user-images.githubusercontent.com/118954022/210099543-5770d313-2143-4167-8ad3-54019f42c11e.png">

## Multi-Cycle and False Paths (revisited)

*	[Set_multicycle_path –setup 2 –to prod_reg[*]/D –through [all_inputs]](#)
*	Hold is always checked at 1 edge before setup, if not provided explicit instruction.
*	Setup will move by endpoints.
*	Whenever MCP is applied for setup, provide for hold as well.
*	[Set_multicycle_path –hold 0.5 –to prod_reg[*]/D –through [all_inputs]](#)
*	[Set_false_path –through <>](#)

## Isolation of Ports

*	[Set_isolate_ports –type buffer [get_ports Out_Y]](#)
*	Cell delay is a function of output load, which could impact internal path timing.
*	Possible Solution: Provide a buffer, which drives the external load and decouples it from internal path.

## Optimizations Combinational Operations

### Goals:

* Cost function based optimizations
  * Optimization till the cost is met.
  * Over optimization of one goal will harm other goals.
  * Goal of synthesis, 3 metrics of netlist which will be contradictory : Meet Timing , Meet Area and Meet Power .
* Faster cells only meet timing ; slower cells meet area and power. 
* Cost function is basically about IO delay, clock period, max_delay, area and power goals. 

### Combinational Logic Optimization

* Squeezing the logic to get the most optimized design. 
  * Area power savings.
* Constant propogation.
  * Direct optimization.
* Boolean Logic optimization. 
  * K-map
  * Quine McKluskey 

Example of Boolean equation :
![note4](https://user-images.githubusercontent.com/118954022/210106717-bb015369-e0b5-4f69-b12f-f6e1c407e1f6.jpg)

### Boolean Logic Optimization

Example of equation (nested with 3 Mux) in the pic below. If 'a' is false, then not of c '!c'. If 'a' is treu, it will look at 'b'. 'b' is true, it will pick 'c'. If 'b' is false, it will look at 'c' wether it is true or false, if 'c' is true will pick 'a' else '0'.

![note6](https://user-images.githubusercontent.com/118954022/210107358-34c86f10-31ec-49ec-bac7-eed789f698c7.jpg)

### Resource Sharing

Multiplier are huge in area and power compare to mux. Eg of simplication of it : ( the right circuit is optimized) 

![note5](https://user-images.githubusercontent.com/118954022/210107716-80dea2c1-5387-43b4-a642-1fba06a50c50.jpg)

Another is **Logic Sharing**. Optimizing something that is common between two circuit or path. Eg: ( right circuit is less consume in area and power, so optimized) 

### Balanced vs Preferential Implementation

Eg: assign y = a & b & c & d & e .Compare the delay from an input to output y..If we see, the circuit at left is Balanced because all input has same delay (2 gate delays) . The circuit at right is  Preferential , as we can see the input e is prefered the most compared to other input with the least delay.

![note8](https://user-images.githubusercontent.com/118954022/210108913-fc549257-b274-4a52-b59e-075ea8e4bff1.jpg)

## Sequential Optimizations

## Special Optimizations

## How Paths are Timed MCP ?


------------------------------------------------------------------------------------------------

## LABS

### LAB 1 - Combinational Optimizations

We look at the various comb opt logics,set of opt files , dc_shell >> sh gvim opt_check*.v -o ; (opens 4 opt files). To read the optimised design, >> read_verilog opt_check.v ; link ; compile ; report_timing ; get_cells * ; write -f ddc -out opt_check.ddc ; (then load the design in gui), verilog_files >> csh ; design_vision ; /or/ dc_shell >>  gui_start ; Then double click and view schematic at the gui. >> reset_design (before to other opt.v file). So from what we skeched, the expected optimized circuit, we can see them in gui. 

![lab1 0](https://user-images.githubusercontent.com/118954022/210179769-4268a53e-282f-43b9-8b4a-e7713dacc809.jpg)
![lab1 1](https://user-images.githubusercontent.com/118954022/210182345-4759cb5b-660c-49b5-81d0-c37d676ad2ff.jpg)
![lab1 2](https://user-images.githubusercontent.com/118954022/210182353-f100ec3a-f457-4f20-a8e8-4c1a9d3d7f67.jpg)

Then check report timing, >> report_timing -to y ; set_max_delay .06 -from [all_inputs] -to [get_ports y] ; report_timing -sig 4 ; compile_ultra ; report_timing ; get_lib_cells */sky130_fd_sc_hd__xnor2* ; size_cell U3 sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__xnor2_4 (to up/down the size cell); compile_ultra ; report_timing ; (done set 6ps max delay).

![lab1 3](https://user-images.githubusercontent.com/118954022/210182693-c1147abc-8b0f-4aae-a2a6-6c5219cbfe8a.jpg)

### LAB 2 - Resource Sharing Optimizations

We look in using design vision for better vision, dc_shell >> gui_start ; (in the gui), sh gvim resource_sharing_mult_check.v & ; read_verilog resource_sharing_mult_check.v ; link ; compile_ultra ; (below is the circuit for this code which is same as the notes)

![note5](https://user-images.githubusercontent.com/118954022/210199983-856326ed-8e2e-4742-8ae3-947e4dcce29d.jpg)
![lab2 0](https://user-images.githubusercontent.com/118954022/210200256-43ca5bdb-222d-420c-891e-0f9d80d980bc.jpg)

>> report_area (to know details of the area). 25ports - refers to the bits used ( 16 input bits, 1 sel input bit and 8 output bits). This is RUN 1.

![lab2 1](https://user-images.githubusercontent.com/118954022/210200895-520f99a6-f292-4f39-8435-f27ef858581b.jpg)

The 'select' is at the begining of the logic at input itself. Select should be at the output based on the initial circuit diagram. In optimized circuit, the select is at input, so it is optimized. eg: at U17 , Output = a.sel + c.!sel .The multiplier logic is present at the output. Then, >> report_timing (path is unconstraint), set_max_delay  -from [all_inputs] -to [all_outputs] 2.5 , report_timing (violated 0.31ps); compile_ultra ; report_timing ;  report_area ; (compare with run 1). So all delays from each input to output is sort of similar. Sel delay is only on multiplexer. a to y is through multiplier and mux. 

![lab2 2](https://user-images.githubusercontent.com/118954022/210259715-868fb686-cece-4616-82e4-3dc59ac95ec3.jpg)

Make select more restricted path >>  set_max_delay 0.1  -from sel -to [all_outputs] ; report_timing ; compile_ultra ; report_area .This is RUN 2. Select is very close to output now.

![lab2 3](https://user-images.githubusercontent.com/118954022/210260459-feaee9a3-2c52-4290-9220-300b4c73de5b.jpg)
![lab2 4](https://user-images.githubusercontent.com/118954022/210261177-62da5294-062c-4459-af9f-7dac42147bc5.jpg)

Then constrain the area, >> set_max_area 800 ; compile_ultra ; report_timing -sig 4 ; report_area ,(this is RUN 3). The area cannot go below 800 because maybe the timing constraints are too tight.

![lab2 5](https://user-images.githubusercontent.com/118954022/210261957-4231c02b-bf8b-4b04-b5f6-fedb8a72eb5d.jpg)

### LAB 3 - Sequential Optimizations

The files, in verilog all the 5 dff_const files. 

![lab3 0](https://user-images.githubusercontent.com/118954022/210266461-2c0c5573-3c79-4959-bea1-5390cc7f2db8.jpg)
![lab3 1](https://user-images.githubusercontent.com/118954022/210266533-9e15c9f3-4330-4cea-aa0d-0edcc2af42d9.jpg)

In dc_shell >>  reset_design ; read_verilog dff_const1.v ; link ; compile ; get_cells ; foreach_in_collection my_cell [get_cells *] { set cell_name [get_object_name $my_cell]; echo $cell_name; } ;  foreach_in_collection my_cell [get_cells *] { set cell_name [get_object_name $my_cell]; set rn [get_attribute [get_cells $cell_name] ref_name]; echo $cell_name $rn; } ; .If we see q_reg is a flop, U5 is inv and U4 is conb.

![lab3 2](https://user-images.githubusercontent.com/118954022/210266939-7b1a27dc-7958-4d64-a0c8-e8705706c8a2.jpg)

Then open design vision, >> read_verilog dff_const1.v ; link ; compile ; .The conb cell is a **tie cell**. Inverter to make active high reset in flop. Input are on gate pin of cmos. It is very sensitive due to "gate oxide", so we should never allow gate terminal of cmos to see any surges , thats why we need to use tie cell. Tie cell is a standard cell that designed specially to provide the high or low signal to the input (gate terminal) of any logic gate. The high/low signal can not be applied directly to the gate of any transistors because of some limitations of transistors, especially in the lower node. So tie cell used to drive 1'b1 or the 1'b0.

![lab3 3](https://user-images.githubusercontent.com/118954022/210267292-81b5e0f5-3925-498d-8ec8-adec93158f2e.jpg)

For dff_const2.v , >> reset_design ; read_verilog dff_const2.v ; link ; compile ;

![lab3 4](https://user-images.githubusercontent.com/118954022/210268713-36dcd684-0106-4adb-9bde-88b221580d98.jpg)

It was tie cell, so set seq const = false , >> reset_design ; read_verilog dff_const2.v ; set compile_seqmap_propagate_constants false (we dont want to propogate the constants) ; link ; compile_ultra ; gui_start ; (we control the seq, we prevent the flop from optimize).

![lab3 6](https://user-images.githubusercontent.com/118954022/210270091-c78d0c4a-31ee-47e5-b9fc-bb939228ac84.jpg)

For dff_const3.v , >> reset_design ; read_verilog dff_const3.v ; link ; compile ; .There are 2 flops. D is always 1, q1 and q are both not seq constants, so not getting optimized.

![lab3 5](https://user-images.githubusercontent.com/118954022/210269407-08bec0a7-a4b0-4610-818d-6ed549a4f979.jpg)

For dff_const4.v , >> reset_design ; read_verilog dff_const4.v ; link ; set compile_seqmap_propagate_constants true ; compile_ultra ; Both flop are set d flip flop and get optimized. This is seq const. 

![lab3 7](https://user-images.githubusercontent.com/118954022/210270920-51efd145-cc8a-4657-93d0-53996f1a317c.jpg)

For dff_const5.v , >> reset_design ; read_verilog dff_const5.v ; link ; compile ; .Not seq const.

![lab3 8](https://user-images.githubusercontent.com/118954022/210271141-f04cfc75-317e-4f64-aad5-1ec2065f6068.jpg)

### LAB 4 - Boundary Optimizations

dc_shell >> sh gvim check_boundary.v & ; read_verilog check_boundary.v (2regs with 3bit flop and 4bit flop); link ; compile_ultra ; write -f ddc -out boundary.ddc ; gui_start .There is no internal module (IM) here and no hier because of boundary optimisation.

![lab4 0](https://user-images.githubusercontent.com/118954022/210272137-c28b591c-1276-48c2-bee6-8bf183fa0204.jpg)

>> reset_design ; read_verilog check_boundary.v ; link ; get_cells ; get_pins u_im/* ; set_boundary_optimization u_im false ; compile_ultra ; gui_start ; .Boundary of u_im is maintained. The design hierarchy are also maintained, so if there any ECO, can quickly search for the bug, let tool not optimized fully for flexibility.

![lab4 1](https://user-images.githubusercontent.com/118954022/210272952-ebe5f942-d912-42be-83d3-60132d5b5cc7.jpg)

### LAB 5 - Register Retiming

Open the only file, >> reset_design ; sh gvim check_reg_retime.v & ; .It is a 4bit multiplier, 3 flops.

![lab5 0](https://user-images.githubusercontent.com/118954022/210273570-c7f96fbd-8ebb-410f-b223-c48a35d61328.jpg)

Read the design, dc_shell >> read_verilog check_reg_retime.v ; link ; compile ; report_timing ; gui_start ; 

![lab5 1](https://user-images.githubusercontent.com/118954022/210274154-45fb01c6-acc4-45bb-9964-630c36aadb33.jpg)
![lab5 2](https://user-images.githubusercontent.com/118954022/210274295-d0f096f1-6ffd-4f92-854f-c00dcd8ce4d1.jpg)

Then constraints, >>  sh gvim reg_retime_cons.tcl ; source reg_retime_cons.tcl ; report_clock ; report_timing ; compile_ultra -retime ; .We can see logics between regs and multipliers. It sliced the multiplier and split the logic into partition and nicely optimized it.

![lab5 3](https://user-images.githubusercontent.com/118954022/210274970-e399e1b3-795f-4f6d-a46a-10af88775335.jpg)
![lab5 4](https://user-images.githubusercontent.com/118954022/210275135-30ed3704-329d-4898-95cb-44d5bb5707ad.jpg)

>> report_timing -from [all_inputs] -trans -cap -nosplit -sig 4 ; .Everything is nicely modeled and meeting the time.

![lab5 5](https://user-images.githubusercontent.com/118954022/210275325-05164fa0-b96e-4753-9c07-452f1c6b3776.jpg)

### LAB 6 - Isolating Output Ports
  
Load varries , cell delay will vary. So if load increases, cell delay also increases. This may cause other logic path to fail. We dont want internal paths to fail because of external load. So we need to isolate the output ports. Add buffer before output port, so the load is driven by buffer. Internal path are decoupled from output paths.

File used , >> sh gvim check_boundary.v & (from previous lab), read_verilog check_boundary.v ; link ; compile_ultra ; gui_start ; .We can see the flop is driving the internal load and output load as well, this is not good. 
  
![lab6 0](https://user-images.githubusercontent.com/118954022/210399135-cb154726-5286-454c-a07f-2e07efd038d9.jpg)

Next we isolate the ports, >> set_isolate_ports -type buffer [all_outputs] ; compile_ultra ; .The internal load are driven by the flop and outputs are driven by the buffer. It is not sensitive by the load anymore. Flop delay remain constant, only buffers see variation.
  
![lab6 1](https://user-images.githubusercontent.com/118954022/210400139-260dc7a6-5439-4c59-ae99-a2867c73d016.jpg)

Before isolating ports, dc_shell>> reset_design ; read_verilog check_boundary.v ;  link ; compile_ultra ; create_clock -per 5 -name myclk [get_ports clk] ; set_input_delay -max 2 [all_inputs] -clock myclk ; set_output_delay -max 2 [all_outputs] -clock myclk ; set_load -max 0.3 [all_outputs] ; report_timing -nosplit -inp -cap -trans -sig 4 ,(reg to io path) ; report_timing -to val_out_reg[0]/D -inp -cap -trans -nosplit -sig 4 ,(reg to reg path).There huge load on the flop.
  
![lab6 2](https://user-images.githubusercontent.com/118954022/210402894-a7faf9db-d4d5-4ff7-af26-1cf22b766b59.jpg)

Report timing after isolate the ports, >> set_isolate_ports -type buffer [all_outputs] ; compile_ultra ; report_timing -nosplit -inp -cap -trans -sig 4 ; report_timing -from val_out_reg[0]/CLK -to val_out_reg[0]/D  -inp -cap -trans -nosplit -sig 4 ;  .The flop is nnow driving small load and we can see the presence of buffers.
  
![lab6 3](https://user-images.githubusercontent.com/118954022/210404392-70d2e2a1-6da5-4345-827e-14d430549f3f.jpg)

### LAB 7 - MultiCycle Path 

File used, >> sh gvim mcp_check.v .The path a*b will get loaded into register only when there is a valid and valid is not going to be generated every cycle, then we can multicycle a*b path.

![lab7 0](https://user-images.githubusercontent.com/118954022/210406200-2f884176-a1bc-4322-919a-3ad96cffbaa8.jpg)

Read constraints, >> read_verilog mcp_check.v ,(1bit reg asynch, 16bit async prod_reg); link ; compile_ultra ; sh gvim mcp_check_cons.tcl & ;

![lab7 1](https://user-images.githubusercontent.com/118954022/210411499-c5d9b3ca-5b7c-4d74-8cc4-17dcaa21a7ac.jpg)

Source the constraints and look report, >> source mcp_check_cons.tcl ; report_timing ; compile_ultra ; report_timing ; .We see a huge violation at slack. The input to prod_reg path can be 2 cycles delay because only when en_int coming.

![lab7 2](https://user-images.githubusercontent.com/118954022/210409493-9d7b2d5a-768a-4946-8fbd-c4901e357459.jpg)

All inputs in, >> set_multicycle_path -setup 2 -to prod_reg[*]/D -from [all_inputs]  ; report_timing -to prod_reg[*]/D -from valid_reg/CLK ; report_clock * ; .Valid to prog_reg is a single cycle path. 

![lab7 3](https://user-images.githubusercontent.com/118954022/210411867-a7e83a02-5b52-45ed-bfd2-46d055fd980c.jpg)

Hold check, >> report_timing -delay min .A huge failure, because it is doing single cycle hold check, suppose zero cycle hold check.

![lab7 4](https://user-images.githubusercontent.com/118954022/210412549-e3a249b3-f151-4060-b3b0-4a5a6d006a20.jpg)

So, we have to perform hold MCP, >> set_multicycle_path -hold 1 -from [all_inputs] -to prod_reg[*]/D ; report_timing -delay min -to prod_reg[*]/D -from [all_inputs] ; .Time launch at zero and captured at zero, so it good now. 

![lab7 5](https://user-images.githubusercontent.com/118954022/210413162-3abf003a-a201-4769-b404-0a53183adb0f.jpg)

Port isolated report, >> set_isolate_ports -type buffer [all_outputs] ; compile_ultra ; report_timing -nosplit -inp -cap -trans -sig 4 ; .Did to avoid timing violation (previous lab). 

![lab7 6](https://user-images.githubusercontent.com/118954022/210415207-c069edd6-37d2-4859-b7b1-87898c0ce92b.jpg)


--------------------------------------------------------------------------------------------------

# #Day_10

## Report Timing

### Generating Timing Reports

*	The delays associated with timing parameters are modelled on semiconductor device physics principles. 
*	Transistor sizing, their type, and how they are connected to each other contributes to different cells, and in turn different cell delays.
*	Similarly, wires can be modelled in terms of Resistance and Capacitance, which in turn adds to the path delay. The path with the worst delay is the critical path. 
* [report_timing](#)
  * -to {list of signals} -> Inputs/flipflop outputs to these signals 
  * -from {list of signals} -> Flip-flop outputs/inputs to these signals 
  * -through {list of pins} -> Paths that go through these pins 
  * -max_paths N -> Number of paths to report
* The difference between the clock signal’s arrival time (called data required time in the report) and the data signal’s arrival time (data arrival time) is called the slack. &#x1F539; Slack = data required time - data arrival time
* **Setup Check** - For your circuit to work at the specified cycle time, the clock signal’s rising edge should always arrive later (or at the same time) than your data signal, which means that your slack should be non-negative.
* **Hold Check** - You want your data to change (data arrival time) a hold-time after the clock signal’s rising edge (data required time). Then, for hold checks we want the following slack to be non-negative. &#x1F539; Slack = data arrival time - data required time 
* DC makes a note of all paths (fall to rise, rise to fall, etc.) and uses that for timing path calculations, apart from the provided constraints. 
*	[-max_paths N](#) : Specifies the number of paths to be reported per path group.
*	[-n_worst paths_per_endpoint](#) : Specifies the number of paths to be reported per endpoint per path group.

###	check_design, check_timing and report_constraints

* [check_design](#) checks for design consistency. E.g.: Will report a feedthrough, as we take out_clk in some of our examples directly from the defined clock.
* [check_timing](#) checks for the specification of constraints, and also let us know if the provided constraints are enough. It might not specify proper end-points to be constrained, that we need to justify.
* [report_constraints](#) provide us with a glimpse as to how our design is feasible in terms of electrical parameters such as power and capacitance.

###	HFN (High Fanout Nets)

* In digital electronics, the **Fan-out** is the number of load gate inputs driven by the output of another single logic gate. **Fan-in** is the number of inputs to the gate. 
* Gates with large fan-out are slower. Gates with large fan-in are bigger and slower. 
* Generally, clock nets, reset, scan, enable nets are High Fanout Nets.
* A high fan-out corresponds to a very high capacitance load, which in turn translates to timing violation, because of a high transition time which adds up in the delay calculation.
* [set_max_capacitance](#) helps in breaking or buffering the High fanout net. 

![note1 2](https://user-images.githubusercontent.com/118954022/210059509-310bb124-4a9f-496d-84ca-a07ecdef9f4e.jpg)

###	Summary

* **Constraints** - clock, genclk (if any), vclk (if any), practicalities of the clock (Uncertainty and Latency), input, output delay, transition, load, set_max_capacitance, transition, etc.
* **Synthesis Optimization Parameters** - Boundary Optimization, Retiming, Constant propagation, unused flop removal, isolating ports, etc.
* **Flow** - read_verilog, provide dbs, source constraints, check_design, check_timing, compile or compile_ultra, report_constraints, report_area and report_timing, write.
* **QOR** - Quality of Results, if you are meeting all your design constraints with good margins, the QOR is good. 

###	Synopsys DC UG Flow

![note1](https://user-images.githubusercontent.com/118954022/210058261-650482ee-1523-4126-8ecf-96e5f0ae8b37.jpg)

**QTM** - Quick Time Models
**ETM** - Extracted Time Models 

------------------------------------------------------------------------------------------------

## LABS

### LAB 1 - Report Timing

File used, >> sh gvim lab8_circuit_modified.v & ; sh gvim lab8_cons_modified.tcl & ,(constraints) ; read_verilog lab8_circuit_modified.v ; .4 registers.

![lab1 0](https://user-images.githubusercontent.com/118954022/210417934-ca8ac117-0832-4ef7-bb3f-d0af0e3b8228.jpg)

then, >> link ; source lab8_cons_modified.tcl ; compile_ultra ; report_timing -sig 4 -nosplit -trans -cap -inp -from IN_A ; .It is reporting max path, there is library setip time and slack = required time - arrival time, so it is **Setup Check**. This report showing from fall to rise then fall. 'f' - fall, 'r' - rising, showing negative unate gate. Launch at 0 and capture at 10, so different.

![lab1 1](https://user-images.githubusercontent.com/118954022/210544423-2ee2b848-6578-474c-8a85-60927379eaa7.jpg)

Check worst delay, >> report_timing -rise_from IN_A -sig 4 -trans -cap -nets -inp ; .This report showing from rise to fall the rise. Having more slack. So previous report has less (min) slack , so it is a worst path. 

![lab1 2](https://user-images.githubusercontent.com/118954022/210546184-01e985de-348f-4b11-8452-031855443f14.jpg)

**Hold check** , >> report_timing -delay min -from  IN_A ; .How to know it Hold check, in report,path type is min, there is library old time, and the slack = arrival time - required time. 

![lab1 3](https://user-images.githubusercontent.com/118954022/210970338-3d4d3fea-e557-4220-b8d2-43b9e1e3618e.jpg)

Thru max path, the cell path maybe minimum but overall path maybe taking maximum. So, always look at overall path delay not contribution of a cell only. 

### LAB 2 - Check_timing , Check_design , Set_max_capacitance , HFN


------------------------------------------------------------------------------------------------


# #Day_11

## Lecture

### What is SoC and Why SoC?
  
* **SoC** is a single-die chip that has some different IP cores on it. These IPs could vary from microprocessors (completely digital) to 5G broadband modems (completely analog).
* The design of a system on chip usually includes a central processing unit, memory, ports for input and outputs, secondary storage devices, and peripheral interfaces such as Timers, etc. 
* Depending upon the requirement it can also consist of a digital or analog signal processing system or a floating-point unit.
* SoC with equivalent functionality will have increased **performance** and reduced **power** consumption as well as a smaller semiconductor **die area**.

### Typical Structure of Snapdragon SoC

![note1](https://user-images.githubusercontent.com/118954022/210316889-78dd715c-6745-4c45-ac9c-29bc5bc53ef6.jpg)

### Types of SoC

* SoCs built around a microcontroller.
* SoCs built around a microprocessor, often found in cell phones.
*	Specialized application-specific integrated circuit SoCs designed for specific applications that do not fit into the above two categories.

### Advantages of SoC

* Reduction in overall system design as compare to motherboard based designs.
* Compact and small size chips even the size of a fingertip.
* Better efficiency and performance.
* Less power consumption.
* Less time to market.
  
### SoC Structure

* An SoC consists of hardware functional units, including microprocessors that run software code, as well as a communications subsystem to connect, control, direct and interface between these functional modules.
* **Functional components**: Processor Cores, Memory, Interfaces, Digital Signal Processor, others.
*	**Intermodule communication**: Bus-Based Communication, Network on a chip.
  
### SoC Design Flow 

![note2](https://user-images.githubusercontent.com/118954022/210317133-97571541-02bc-48ac-a410-4a2ab4358955.jpg)
  
### How are Microchips made?

Sorce : https://www.youtube.com/watch?v=bor0qLifjz4 
  
### Introduction to BabySoC

**VSDBabySoC** is a small yet powerful RISCV-based SoC. The main purpose of designing such a small SoC is to test three open-source IP cores together for the first time and calibrate the analog part of it. VSDBabySoC contains one RVMYTH microprocessor, an 8x-PLL to generate a stable clock, and a 10-bit DAC to communicate with other analog devices.

![note3](https://user-images.githubusercontent.com/118954022/210318103-9b658264-d1f7-46db-bba9-d1378fa17935.jpg)
  
###	BabySoC Components

* **RVMYTH**: RVMYTH core is a simple RISCV-based CPU.
* **PLL**: A phase-locked loop or PLL is a control system that generates an output signal whose phase is related to the phase of an input signal. PLLs are widely used for synchronization purposes, including clock generation and distribution.
* **DAC**: A digital-to-analog converter or DAC is a system that converts a digital signal into an analog signal. DACs are widely used in modern communication systems enabling the generation of digitally-defined transmission signals. 

### Introduction to Modelling

* Some initial input signals will be fed into BabySoC module that make the pll start generating the proper CLK for the circuit.
* The clock signal will make the rvmyth to execute instructions in its imem. As a result, the register r17 will be filled with some values cycle by cycle 
* These values are used by dac core to provide the final output signal named OUT.
* So, we have got 3 main elements (IP cores) and a wrapper as an SoC and off course there would be also a testbench module out there.

GitHub Reps for references:
* https://github.com/manili/VSDBabySoC#what-is-rvmyth
* https://github.com/Devipriya1921/avsddac28nm 
* https://github.com/ireneann713/PLL 
* https://github.com/lakshmi-sathi/avsdpll_1v8 


------------------------------------------------------------------------------------------------


# #Day_12

## VSDBabySoC Modelling

### Recap on SoC

* **SoC** is a single-die chip that has some different IP cores on it. These IPs could vary from microprocessors (completely digital) to 5G broadband modems (completely analog).
* SoC with equivalent functionality will have increased performance and reduced power consumption as well as a smaller semiconductor die area.

### Modelling of the VSDBaby SoC

#### What does Modelling mean ??

In electronics terminology, **Modeling** and **Simulation** (M&S) is the use of a **physical or logical** representation of a given system to generate data and help determine decisions or make predictions about the system. Models are representations that can aid in Defining, Analyzing, and Communicating a set of concepts. M&S is widely used in the VLSI domain. 

Purpose of Modelling :

System models are specifically developed to :
a.	support analysis, specification, 
b.	design, 
c.	verification, 
d.	and validation of a system,
e.	as well as to communicate certain information.

What are we Modelling ??

* In VSDBabySoC modelling, we are going to model and simulate the VSDBabySoC.
* Some **initial input signals** will be fed into vsdbabysoc module, that will get the pll start generating the proper CLK for the circuit. 
* The clock signal will make the RVMYTH to execute instructions and some values are generated, these values are used by DAC core to provide the final output signal named OUT.
* So we have 3 main elements (**IP cores**) and a wrapper as an SoC and of course there would be also a testbench module out there.

#### RVMYTH - Risc-V based MYTH(Microprocessors for You in Thirty Hours)  

VSDMemSoC is a small SoC including a RISCV-based processor named **RVMYTH** and an external 1kB SRAM Instruction Memory (IMem) to separate the processor core and the IMem. RVMYTH core is a simple RISCV-based CPU, introduced in a workshop by RedwoodEDA and VSD. Source : https://www.vlsisystemdesign.com/vsd-intern-fpga/ 

**RISC** stands for Reduced Instruction Set Computer. **RISC-V**(pronounced “risk-five”) ISA is defined as a base integer ISA, which must be present in any implementation, plus optional extensions to the base ISA. Each base integer instruction set is characterized by the width of the integer registers and the corresponding size of the address space and by the number of integer registers. There are two primary base integer variants, RV32I and RV64I. Eg: A simple one cycle CPU for Risc-V.
![note1](https://user-images.githubusercontent.com/118954022/211268139-1b7a83b9-755f-468e-8ca9-e856bf3a59e6.jpg)

Waterfall flow diagram for a **pipelined** Risc-v processor instructions :
![note2](https://user-images.githubusercontent.com/118954022/211268291-bb781294-4a09-417e-8199-7e5404319246.jpg)

#### Phase Locked Loop (PLL)

A **Phase Locked Loop** (PLL) is an electronic circuit with a voltage or voltage-driven oscillator that constantly adjusts to match the frequency of an input signal. PLLs are used to generate, stabilize, modulate, demodulate etc.

Now, question is why do we need a PLL for our SoC? Before that how is a clock generated? 
Quartz Crystal Oscillator. For 100Mhz and below off chip oscillator will do, but for 100Mhz and above it won’t be good enough.-how?

Why off-chip clocks can’t be used all the time?
* The clock will be a supply for a lot of blocks on the chip, it will have delays due to long wires(if used only one clock source) - also reasons like **clock jitter**.
* Some blocks might need 200Mhzs and some might need 100Mhz - point is different frequencies just on one small chip.
* A concept of **ppm**(clock accuracy) comes in, when ever quartz is acquired, it comes with a **x ppm error**.

What is this **ppm error**?

**ppm** - parts per million. For ex:  20ppm quartz used in watches this translates as 20/1e6 (2e-5), which  gives an error over a day of 86400 * 2e-5 = 1.73 seconds per day, so in a month it loses 30 x 1.72 = 51 seconds or 1 minute a month. Now, in terms of a chip, just imagine the mishap it will cause just due to very small error for ,microseconds, when the processor works at nanoseconds , it can be a **huge blow**.

PLL used on SoC’s

Main components : 
1.  Phase detector
2.	Loop filter
3.	Voltage controlled oscillator
4.	Frequency divider 

![note3](https://user-images.githubusercontent.com/118954022/211269923-d2d4176d-201c-4ab9-89d2-2c2e5ac15e50.jpg)

Expected outcome:
![note4](https://user-images.githubusercontent.com/118954022/211270098-e09b33c1-be79-42c3-8747-089af043c177.jpg)

#### Digital to Analog Converter (DAC)

A **Digital to Analog Converter (DAC)** converts a digital input signal into an analog output signal. The digital signal is represented with a binary code, which is a combination of bits 0 and 1. A Digital to Analog Converter (DAC) consists of several binary inputs and a single output. In general, the number of binary inputs of a DAC will be a **power of two**.

There are two types of DACs :
* Weighted Resistor DAC.
* R-2R Ladder DAC.

**Weighted Resistor DAC**

A weighted resistor DAC produces an analog output, which is almost equal to the digital (binary) input by using binary weighted resistors in the inverting adder circuit. In short, a binary weighted resistor DAC is called as weighted resistor 
DAC.

![note5](https://user-images.githubusercontent.com/118954022/211270663-aba073dd-855b-49a8-9f88-8b95546e2de4.jpg)

**R-2R Ladder DAC**

The **R-2R Ladder DAC** overcomes the disadvantages of a binary weighted resistor DAC. As the name suggests, R-2R Ladder DAC produces an analog output, which is almost equal to the digital (binary) input by using a R-2R ladder network in the inverting adder circuit. 

![note6](https://user-images.githubusercontent.com/118954022/211270928-1bdc7b87-c1f2-4bf5-af13-d8d0262b60ed.jpg)

Expected output for 3-bit DAC :
![note7](https://user-images.githubusercontent.com/118954022/211271061-425d07c4-5a22-49c7-954f-c51c963d732c.jpg)

For VSDBabySoC, it consists of a 10-Bit DAC.

#### The Task.

To do - module RVMYTH modelling , PLL modelling and DAC modelling. RVMYTH is a digital block, so yes we can use a HDL for designing and check its functionality using a testbench. But, DAC and PLL are analog.

Because verilog can’t synthesis analog design. We are going to simulate it using verilog itself. We will be using data-types such real. Our goal is to be able to simulate “functionality” - **to verify its logical correctness** . So we will be using verilog to model and use **VCS** to simulate. 

### Modelling and Simulating using Synopsys VCS

#### How do we model and simulate ??

We will be using **VCS** - is a high-performance, high-capacity Verilog simulator that incorporates advanced, high-level abstraction verification technologies into a single open native platform.  

Modelling and Simulating on VCS involves 2 main steps :

1.	Compilation - VCS builds the instance hierarchy and generates a binary executable simv. This binary executable is later used for simulation.
2.	Simulation  - During compilation, VCS generates a binary executable, **simv** - to run the simulation. It has 2 types mainly - **Interactive Mode** and **Batch Mode**. For modelling and simulation [Interactive Mode is preferred](#).

In interactive mode, we mean to say **debug the design** and so on. One down side is the compilation will not be “optimized”. VCS has the following compile-time options for debug mode: 
*	-debug_pp,
*	-debug, 
*	-debug_access(+), 
*	-debug_all,
*	-debug_region=()(+)

We will be debugging using tools like **DVE** -  Discovery Visualization Environment. Few tips on modelling our design :
1.	Avoid race Conditions - can use VCS [race detection tool](#).
2.	Use a optimized Testbench for debugging your design.
3.	Creating models that simulate faster.
4.	Case statement behaviour.

![note8](https://user-images.githubusercontent.com/118954022/211277871-979d6476-c326-42be-9ea9-30b16d39162f.jpg)

Basic commands : 

Always start with a `csh` command on your terminal
*	vcs [options] model_file(verilog file)
  *	**-h** or **--help** : lists the most commonly used commands.(GO TO COMMAND) 
* To use GUI version can do `vcs -gui`.

#### Using DVE - 1(normally)

DVE provides you with a graphical user interface to debug your design. Now, first run the design, with a valid testbench using the commands :
* ` csh `
* ` vcs design_file.v design_testbench.v `
* ` ./simv ` - (this should run without any errors and also preferably without warnings in the **simulation report**)
* So one KEEP IN MIND point : in previous sessions, there was a introduction to .vcd file - means **Value Code Dump**.(cross check if its created or not)
* So in the testbench, always have this block
  * Initial 
          Begin
          $dumpfile("design_tb.vcd");
          $dumpvars; end

NOTE : make sure to run these commands in our project directory/design folder.

Now, we are going to open dve :
* `dve &`       // (basically opening the tool).
* Go to “File/Open Database” and select the “.vcd” file from the project folder.
*	Then you will find the name of your test bench model in the Hierarchy box (design_tb). Expand it so that you can find DUT in the options.
* If we click on DUT , select the signals listed(all or partial) and right click, you will find an option “Add to Waves”.
* Click on “Add to New Wave View” to see the waveforms of your Inputs and Outputs. You should see your results in a new window. Then adjust the size of the waveform and explore other options as well.

#### Using DVE - 1(interactive mode)

DVE provides us with a graphical user interface to debug our design. Using DVE, we can debug the design in Interactive Mode or in Post-processing Mode.
Command for using it - `simv -gui`

To run the Testbench and the design file :
* vcs -debug_access<+options> [compile_options] TOP.v
* vcs -lca -debug_access+all design.v design_tb.v

After getting the code dump file :
*	Run `simv -gui`

This should open the dve tool automatically and we can fully run our test bench or debug it step by step. To do this first select **‘inputs’** and **‘outputs’** from variable window and right click “Add to the Waves”. Then click the tool button of blue arrow in brace or press F11 to run the test bench step by step. Or click the tool button of the blue arrow pointing downward or press F5 to run the test bench fully.

![note9](https://user-images.githubusercontent.com/118954022/211282164-02b08839-ef95-4b9b-8e75-4c1fc3847b17.jpg)

#### RVMYTH Modelling 

The steps for modelling RVMYTH :
1.	We have a RISC-V CPU core written in Verilog and an already written testbench code for the same.
2.	The entire C program will be converted into a hex format and and will be loaded into memory.
3.	The CPU will then read the contents of the memory, process it and finally display the output result of sum of numbers from 1 to n.

The steps to model the IP cores separately :

For modelling RVMYTH(RISC-V)
1.	git clone https://github.com/kunalg123/rvmyth/ 
2.	cd rvmyth 
3.	csh
4.	vcs mythcore_test.v tb_mythcore_test.v 
5.	./simv
6.	dve & 
7.	Go to file/File/Open Database” and select the “.vcd” file from the project folder
8.	Add the required waveforms. 

For modelling DAC
1.	git clone https://github.com/kunalg123/rvmyth/     /// ignore if already done once!
2.	cd rvmyth 
3.	csh
4.	vcs avsddac.v avsddac_tb_test.v
5.	./simv
6.	dve & 
7.	Go to file/File/Open Database” and select the “.vcd” file from the project folder
8.	Add the required waveforms. 

Follow the same for pll using design file as - [avsd_pll_1v8.v](#) and testbench - [pll_tb.v](#)

Steps for simulating in interactive mode(debug mode)
1.	git clone https://github.com/kunalg123/rvmyth/  // ignore if already done once 
2.	cd rvmyth 
3.	csh
4.	vcs -lca -debug_access+all mythcore_test.v tb_mythcore_test.v 
5.	./simv -gui &
6.	Add the required waveforms.
7.	You will get to debug line-by-line for the whole code

Note: Understand the code using debug mode(either PLL/DAC/RISC-V -> as per your time).

Now, we have verified each block separately, lets interface blocks together. Lets simulate risc_v and pll : 
1.	cd rvmyth 
2.	csh
3.	vcs rvmyth_pll.v rvmyth_pll_tb.v 
4.	./simv
5.	dve & 
6.	Go to file/File/Open Database” and select the “.vcd” file from the project folder
7.	Add the required waveforms. 

Follow the same for DAC and RVMYTH using design file as - [rvmyth_avsddac.v](#) and testbench - [rvmyth_avsddac_TB.v](#)

Finally lets simulate and model all three IP’s together :
* Simulate [https://github.com/manili/VSDBabySoC/blob/main/src/module/vsdbabysoc.v](#)
* Using VCS with the testbench in [https://github.com/manili/VSDBabySoC/blob/main/src/module/](#)

There will be some errors you will be facing. So time to some DEBUGGING.

Hint : mostly the error will be in ‘include files’ - that are available in [https://github.com/manili/VSDBabySoC/tree/main/src/include](#) and
[https://github.com/manili/VSDBabySoC/blob/main/src/module/](#) , just have to go through the **simulation report** thoroughly.

For cross verification of your simulations (OR) how do we know which outputs to observe for :
1.	PLL/ RVMYTH – [https://github.com/vsdip/rvmyth_avsdpll_interface](#)
2.	DAC/RVMYTH – [https://github.com/vsdip/rvmyth_avsddac_interface](#)
3.	PLL interfacing RVMYTH -  [https://github.com/vsdip/rvmyth_avsdpll_interface](#)
4.	DAC interfacing RVMYTH – [https://github.com/vsdip/rvmyth_avsddac_interface](#)
5.	vsdbabySoC – [https://github.com/manili/VSDBabySoC/blob/main/images/pre_synth_sim.png](#)

Tasks and to be added on to our repo.
1.	Make a difference table for all the modes in interactive mode I,e -debug_pp, -debug, -debug_access(+)... and so on.
2.	To get more used to VCS, each one take an example circuit for example
    a. 4- bit adder
    b.	Counter 
    c.	4x1 mux
    d.	Decoder 
    e.	Encoder 
    f.	Any circuit of your choice -- PREFERRED 
And simultate, attach snippets of code, screenshots of simulation, block  diagrams etc on to the github repo.
3. 	After getting acquainted with VCS, then get into modelling and simulation of VSDBabySoC.

Additional: Synopsys uses needs its proprietary file for post synthesis. Eg: .dc files. In hand we have .lib files - liberty files. How do we convert .lib to .dc file : (try to see for converting **shells**  from synopsys itself).

NOTE : make sure to go through synopsys documentation for VCS. 

References
1.	Risc-v : https://myth3.makerchip.com/sandbox/# 
2.	Risc-v waterfall flow diagram : 
https://www.vlsisystemdesign.com/risc-v-waterfall-diagram-and-hazards/ 
3.	Why PLL :
https://www.mpi-inf.mpg.de/fileadmin/inf/d1/teaching/winter20/how_to_clock/ lecture_13_PLLs_2020_12_14.pdf 
4.	https://github.com/manili/VSDBabySoC 
5.	https://github.com/Devipriya1921/VSDBabySoC_ICC2 

------------------------------------------------------------------------------------------------

## LABS

### BabySoC Modeling
  
### Simulation of basic circuit using VCS

------------------------------------------------------------------------------------------------


# #Day_13

## Recap on Pre-synthesis 

In pre-synthesis - modelled and simulated the IP cores in VSDBabySoC(for checking its functionality). Just a refresh on synthesizable and non-synthesizable constructs in verilog.
![note1](https://user-images.githubusercontent.com/118954022/211336378-4230b2fe-23b2-411f-be85-af29309e6404.jpg)

Why we have to do Pre-synthesis ??

**Pre-Synthesis Simulation** is done according to the logic we have designed for and written -> only functionality.

## Post-synthesis

**Post Synthesis Simulation** - ‘gate level simulation’ is done after synthesis considering each and every gate delays into account. reports the violations in both functionality and timing. 
This also shows the mismatches we are likely to get due to wrong usage of operators and inference of latches. For eg: using ‘X’(simulator terms/ synthesizer terms) - ‘Unknown’/“Don’t care”.

## GLS - Gate Level Simulations

**Gate Level Simulation** is used to boost the confidence regarding implementation of a design and can help verify dynamic circuit behaviour, which cannot be verified accurately by static methods. It is a significant step in the verification process.

*	The term "gate level" refers to the netlist view of a circuit, usually produced by logic synthesis. 
*	So while RTL simulation is pre-synthesis, **GLS is post-synthesis**. 
*	The netlist view is a complete connection list consisting of gates and IP models with full functional and timing behavior. 
*	RTL simulation is a **zero delay** environment and events generally occur on the active clock edge. GLS can be zero delay also, but is more often used in unit delay or full timing mode. 

## How do we do Synthesizing ??

What are we going to synthesize the netlist with ??

We will be using Synopsys’s DC shell (**Design Compiler**). Design Compiler® RTL synthesis solution enables users to meet today's design challenges with concurrent optimization of **timing, area, power** and **test**.

Synthesize using DC:

Will point to the right files for one example. Let us say, we have to do for rvmyth_avsddac.v

Steps in brief : (refer day 6,7 repo)
1.	Invoke DC and Read the verilog file -> [rvmyth_avsddac.v](#)
2.	Read .db file and set target_lib -> [sky130_fd_sc_hd__tt_025C_1v80.lib, avsddac.lib](#)

But, we need a **.db** , we only have **.lib** .So the answer is synopsys’s lc_shell (Library Compiler). Follow these commands to convert .lib to .dc :
1.	lc_shell
2.	read_lib library.lib(if in the same directory as the .lib) Else - > read_lib <your_path>/library.lib
3.	write_lib library -format db -output library.db  (If the program is successfully reading your commend, it will returns '1').
4.	quit

After getting the .db , let us resume 
1.	Invoke DC and Read the verilog file -> [rvmyth_avsddac.v](#)
2.	Read .db file and set target_lib -> [sky130_fd_sc_hd__tt_025C_1v80.db, avsddac.db](#) (use both the timing libraries) 
3.	Write -f verilog command, synthesizing the code. Get the synthesized code.

We need to perform post-synthesis simulations.

Why do it? - To make sure we consider each and every gate delays into account. However the pre-synthesis simulations were done using VCS and DVE(./simv), we do the same and observe the output. The post-simulation output and pre-simulation output **should match**.

Example for post-synthesis simulations(rvmyth_avsddac) :
1.	cd <to the directory with the synthesis file>
2.	csh
3.	vcs  gls.v sky130_fd_sc_hd.v primitives.v https://github.com/vsdip/rvmyth_avsddac_interface/blob/main/iverilog/Post-synthesis/gls.v https://github.com/vsdip/rvmyth_avsddac_interface/blob/main/iverilog/Post-synthesis/primitives.v https://github.com/vsdip/rvmyth_avsddac_interface/blob/main/iverilog/Post-synthesisky130_fd_sc_hd.v/ Understand the codes and makes sure “**include all the dependencies**”
4.	dve -full64 &
5.	Go to file/design file -> expand the DUT’s 
6.	Add the required waveforms.

Additional : Can we optimize what we have synthesized using DC? Hint : use the ‘Optimization’ part from the repos.

References 
1.	https://www.electronicsforu.com/electronics-projects/gate-level-simulation-in creasing-trend#:~:text=Gate%20level%20simulation%20is%20used,step%2 0in%20the%20verificathttps://github.com/vsdip/rvmyth_avsdpll_interfaceion %20process.
2.	https://personal.utdallas.edu/~xxx110230/lc/
3.	https://github.com/vsdip/rvmyth_avsddac_interface - for post synthesis
4.	https://github.com/vsdip/rvmyth_avsdpll_interface - for post synthesis
5.	https://github.com/manili/VSDBabySoC#post-synthesis-simulation-gls - for post synthesis of full VSDBabySoC
6.	http://www.sunburst-design.com/papers/CummingsSNUG1999SJ_SynthMis match.pdf   - Important!


------------------------------------------------------------------------------------------------

## LABS

------------------------------------------------------------------------------------------------

# #Day_14

## PVT

*	**PVT** stands for Process, Voltage and Temperature.
*	Integrated circuits are designed in such a way that they can function in a wide variety of temperatures and voltages, rather than a single temperature and *oltage.
*	To make our chip to work after fabrication in all the possible conditions, we simulate it at different corners of process, voltage, and temperature. 
*	These conditions are called corners. All these three parameters directly affect the delay of the cell.
*	**Process** - There are millions of transistors on the single-chip as we are going to lower nodes and all the transistors in a chip cannot have the same properties. Process variation is the deviation in parameters of the transistor during the fabrication.
*	**Voltage** - As we are going to the lower nodes the supply voltage for a chip is also going to less. Let’s say the chip is operating at 1.2V. So, there are chances that at certain instances of time this voltage may vary.
* **Temperature** - When a chip is operating, the temperature can vary throughout the chip. This is due to the power dissipation in the MOS-transistors.

### PVT Graphs

![note1](https://user-images.githubusercontent.com/118954022/211723498-a1f3f009-6af4-4e2e-abc7-4ce6bafa6e76.jpg)

In Process graph, the delay is more for slow process MOSFETs and delay is less for fast process MOSFETs. In Voltage, more is the voltage, more is the current, hence delays are less. In Temperature, As temperature increase random motion of carriers in channel increases due to collision effect thus degrading mobility of carriers. When temperature is less randomness decreases and due to a better mobility current increases and delay decreases. 

References
*	What are PVT corners in VLSI? - ChipEdge VLSI Training CompanySystem on a chip – Wikipedia
*	PVT (Process, Voltage, Temperature) - VLSI- Physical Design For Freshers (physicaldesign4u.com)

------------------------------------------------------------------------------------------------

## LABS

### TASK 1 

Use the timing libs for different PVT corners by using the following GitHub repo: vsdpcvrd/resources/timing_libs at main · Geetima2021/vsdpcvrd (github.com)

### TASK 2 

Document the different PVT corners WNS, WHS, TNS values in the form of a table as shown below: 170959322-b3c3cedd-1df8-4567-99d3-e905f9bdc393.png (268×418) (user-images.githubusercontent.com)

------------------------------------------------------------------------------------------------

# #Day_15 

**Inception of Open-source EDA, OpenLANE and Sky130 PDK**

## How to talk to computers ??

### Intro to QFN-48 Package

Package : QFN-48 Quad Flat No-leads 7x7mm.

![note1](https://user-images.githubusercontent.com/118954022/212529635-9a192340-6b86-4bff-9caf-234660ba505b.jpg)

**QFN** stands for quad flat no-lead package. It is a leadless package that comes in small size and offers moderate heat dissipation in PCBs. Like any other IC package, the function of a QFN package is to connect the silicon die of the IC to the circuit board. The **QFN packages** come with a die that is surrounded by a lead frame. The lead frame is made up of a copper alloy with a matt tin coating. The die and the frame are usually connected to each other using wire bonding. Copper/gold is usually preferred for wire bonding.

The block diagram (ports):
![note2](https://user-images.githubusercontent.com/118954022/212529687-9d7dc499-e3bc-478c-97cc-0a7239dae378.jpg)

* **IC Package** - the material that contains a semiconductor device. The package is a case that surrounds the circuit material to protect it from corrosion or physical damage and allow mounting of the electrical contacts connecting it to the printed circuit board (PCB).
* **Pad** - a square of top-level metal of approximately 100µm on a side that is either soldered to bond wire connecting to a package or coated with lead solder ball. Pad refers to metal square only or to the complete I/O cell containing the metal.
* **Core** - a core comprises a logical execution unit and functional units. It able to independently execute programs or threads. Consists of main logics.
* **Die** - is the formal term for the square of silicon containing an integrated circuit that has been cut out of the wafer.
* **Macro** - Hard macro, firm macro and soft macro are all known as IP (Intellectual property). They are optimized for power, area and performance. They can be purchased and used in your ASIC or FPGA design implementation flow. Soft macro is flexible for all type of ASIC implementation. Soft macros are synthesizable register transfer level (RTL) design forms, have more flexibility, and can be configured compared to hard complex macros. Using Soft macros in the design is a risk factor because of its being unpredictable behavior in timing, performance and power
* **Foundry IP's** - all Intellectual Property, regardless of when or for what purpose it is developed, pertaining to genetic components, pathways, and strains; and methods and tools for design, genetic engineering, testing and/or small-scale fermentation of microbial strains.Has higher value compared to macro.

![note3](https://user-images.githubusercontent.com/118954022/212530541-01e5ac1a-3719-4758-94ea-90eba5d324d4.jpg)

### Intro to RISC-V

**RISC-V Instruction Set Architecture (ISA)**

![note4](https://user-images.githubusercontent.com/118954022/212535323-092ed139-f3be-4fb9-a231-587636c1b34d.jpg)

**RISC-V** is an ISA based on reduced instruction set computer (RISC) principles. An **Instruction Set Architecture (ISA)** is part of the abstract model of a computer that defines how the CPU is controlled by the software.

RISC-V architecture to layout. C codes will be compiled in RIS-V assembly language program. The assembly language will be converted to machine language, which is binary language that is understood by the computer or hardwares. The converted binary language will be sketched in a layout by the computer program and we will get the required output. However, there is another interface that should be presented between architecture and layout of RISC-V which is **Hardware Description Language (HDL)** where it used in RTL implementing the specifications of RISC-V.

### Software to Hardware Applications

Application Software or apps runs on specific hardware. Apps enters into a block calls System Software. Major components in system software are OS, Compiler and Assembler. The basic flow of sysnthesis process : Software (HLL) -> System software (Assembly language) -> Hardware (Machine language). OS holds the major job of coverting language that understood by the hardware. The instruction files represents the hardware and known as abstrat interface (architecture of the computer) or ISA.
  
**Operating System (OS)**
* Handle IO opertions.
* Allocate memory.
* Low level system functions
  
**Compiler**
*Converting the programming language into the respective intructions. (eg: C++ to instruction file(.exe))
* The syntax of the instruction is depending upon what kind of the hardware is, as eg: if the hardware belongs to RISc-V format, the syntax would have the syntax of RISc-V file format instructions.

**Assembler**
*Take particular instructions and convert it into the respective binary language number which is machine language program.
* Consisting of logic 1 and logic 0 where the computer/hardware understands the language.

![note5](https://user-images.githubusercontent.com/118954022/212858060-85d65ace-ada7-4f85-be0f-bbe886201d33.jpg)

Example of stop watch application flow :
![note6](https://user-images.githubusercontent.com/118954022/212858586-91235528-e8bd-49e2-97ef-2e9948867a02.jpg)

![note7](https://user-images.githubusercontent.com/118954022/212859755-809af203-3893-4c49-b9df-9761c72ed442.jpg)
  
## SoC Design and OpenLANE

### Intro to all components of Open-source Digital ASIC Design 

Open source digital ASIC design

Elements for Designing ASIC Flow :
* Hardware Description Language (HDL) which Register Transfer Level (**RTL**) model of the function we want to implement including **RTL's IP**. (github.com, opencores.org)
* **EDA** Tools (OpenLane, Qflow, OpenRoad.)
* **PDK** (Process Design Kit) data - Collection of files used to model a fabrication process for the EDA tools used to design an IC. The interface between the fabrications and the designers. (OpenPDK SkyWater)
  * Process Design Rules :DRC,LVS and PEX
  * Device Models
  * Digital Standard Cell Libraries
  * I/O Libraries
  
### Simplified RTL2GDS Flow

ASIC Flow objective : 
* RTL to GDSII
* Also, called Automated PnR and/or Physical Implementation

Simplified RTL to GDSII Flow.

![note8](https://user-images.githubusercontent.com/118954022/213150523-5afbb491-378f-4094-8a94-464ad528b8fe.jpg)

[RTL] ( Synthesis -> Floor/Power Planing -> Placement -> Clock Tree Synthesis -> Routing -> Sign OFF ) [GDSII]

Source: http://vlsitechnology.org/
  
SYNTHESIS :
* Converts RTL to a circuit out of components from the standard cell library (SCL).
* Standards cells have regular layout. Each cells comes with different views/models. Eg: Electrical, HDL, SPICE, Layout (abstract and detailed).
* The result of the circuit is described in HDL and usually refered as gate level netlist, also it is functional equivalent to RTL.

![note9](https://user-images.githubusercontent.com/118954022/213353623-1a161dc5-03a5-42f2-b433-d0db80432218.jpg)

FLOOR/POWER PLANNING:
* Chip Floor-planning - Partition the chip die between different system building blocks and place the I/O pads.

  ![note10](https://user-images.githubusercontent.com/118954022/213357779-58d5ff59-b30d-4986-8d09-8dbc863bdebb.jpg)

* Macro Floor-planning - Defines the dimensions, pin locations, rows definition, and routing tracks.

  <img width="118" alt="image" src="https://user-images.githubusercontent.com/118954022/213357900-20ff9887-50f0-455d-9027-ebc973cf4267.png">

* Power Planning - The power is provided to the every macros, standard cells, and all other cells are present in the design. Typically, shift the power by power pads and the power distribution network uses upper metal layers since they are thicker than lower metal layers.

  <img width="317" alt="image" src="https://user-images.githubusercontent.com/118954022/213358030-73a97702-25d8-4071-8207-cb1b91307c03.png">
  
PLACEMENT :
* Place the cells on the floorplan rows, alligned with the sites (finding a suitable physical location for each cell in the block).
* Theoretically, should be place close to each other to reduce/prevent interconnect delays, and enable successful routing.
* Usually done in 2 steps :
  * Global - First stage of the placement where cells are placed inside the core area for the first time looking at the timing and congestion, it aims at generating     a rough placement solution (draft) that may violate some placement constraints like overlapping while maintaining a global view of the whole netlist.
  * Detailed - The position obtained from global placements are minimally altered. 

![note11](https://user-images.githubusercontent.com/118954022/213379397-089326c1-3012-41aa-995b-cfde2e3cd2f2.jpg)

CTS (Clock Tree Synthesis) : 
* Create a clock distribution network
  * To deliver the clock to all sequential elements. (eg: FF)
  * Along with minimum skew (zero is hard to achieve) and in a good shape.
  * Usually a Tree. ( H or X like shaped, etc.)
  
<img width="117" alt="image" src="https://user-images.githubusercontent.com/118954022/213382217-d023467d-274c-4754-b90c-579851826456.png">

ROUTING :
* Implementing the interconnect using the available metal layers.
* Metal tracks form a routing grid.
* Routing grid is huge, so it uses 2 approaches.
* Divide and Conquer approach
  * Global Routing - Generates routing guides.
  * Detailed Routing - Uses the routing guides to implement the actual wiring.

![note12](https://user-images.githubusercontent.com/118954022/213384646-e97ca505-1015-49d3-aa8c-cd502d09eb86.jpg)

SIGN OFF :
* Final layout which undergoes verifications and matches the gate level netlist.
* Physical Verifications
  * Design Rules Checking (DRC) - ensuring the final layout obeys all the design rules.
  * Layout vs Schematic (LVS) - ensuring the final layout matches the gate level netlist of the design.
* Timing Verification
  * Static Timing Analysis (STA) - ensuring all the timing constraints are met and the circuit will run at designated clock frequencies.

### Intro to OpenLANE and Strive Chipsets

Open Source ASIC Flow

The problem is tougher when using open source EDA
* Tools qualification ?
* Tools calibration ?
* Missing tools ?

**OpenLANE** - Started as an Open-Surce Flow for a True Open Source Tape-Out Experiment. **striVe** is a family of open everything SoCs i.e. Open PDK, Open EDA, Open RTL.

![note13](https://user-images.githubusercontent.com/118954022/213392621-edd73777-2676-465a-8074-afafecb58ae6.jpg)

striVe2 is identical with striVe1 but it uses 1 kbytes Open Ram instead of SRAM. striVe5 same as striVe2 but it uses 8x1 open ram banks. striVe6 same as striVe2, it used for design testing with DFT.

Main Goal of OpenLane 
* Produce a clean GDSII with no human intervention (no human in the loop). Clean means:
  * No LVS violations.
  * No DRC violations.
  * Timing Violations.
* Tuned for skywater 130nm Open PDK. Also, supports XFAB180 and GF130G Containerized. **Containerized** - Functional out of the box. Instructions to build and run natively will follow.
* Can be used to harden Macros and Chips. 
* Two modes of operations : Autonomous (push button flow) or Interactive (run command step by step).
* Design Space Exploration : Find the best set of flow configurations.
* Comes up with large number of design examples.

### Intro to OpenLANE detailed ASIC Design Flow

![note14](https://user-images.githubusercontent.com/118954022/213405501-1ae210c6-5f82-4ca9-9c38-2203a7839fe1.jpg)

OpenLANE ASIC Flow (Detailed Design Flow). The flow started from RTL design and ended with final layout in GDSII format by using the function of PDK. OpenLANE is based on several open source project i.e. OpenROAD, KLayout, Yosys, QFlow, ABC, and etc. The steps start with RTL synthesis where RTL is fed into Yosys with the design constraints. Yosys will translate the RTL into logic circuits and be optimized. The optimized circuit will be mapped into cells from the cell library using abc where abc has to be guided during the optimization. OpenLANE comes with several abc scripts.
  
* **RTL Synthesis** (Yosys+ABC)- The design is synthesized into a gate-level netlist using yosys and static timing analysis is performed on the resulting netlist using **OpenSTA**.
* **Synthesis Exploration** - Used to generate reports that shows how the design delay and area (can pick the best strategy base on this). It is also can be used to sweep the design configurations (**Design Exploration**) and generate reports design. The best configurations can be picked from the design.
* **Regression Testing** - The design exploration uitlity is also used of rregression testing (CI). We run OpenLane on ~70 desgn and compare the results to the best known ones.
* **Insertion of DFT Structures** - An open-source Design For Testability (DFT) toolchain, Fault, can **optionally** be used to modify the netlist, inserting scan chains and the necessary IO ports to scan and test the design after fabrication. It performs several steps such as Scan Insertion, Automatic Test Pattern Generation (ATPG), Test Patterns Compaction, Fault Coverage and Fault Simulation.
* **Physical Implementation** - Known as automated PnR (Place and Route). Advancing with the physical implementation, we note that most of the tools in this stage are used from within the **OpenROAD** application in combination with other tools, some of them are custom and based on the OpenDB infrastructure, while others are indpendent.
* **Logic Equivalent Check (LEC)** - Everytime the netlist is modified, verifications must be performed. CTS and Post Placement Optimization modifies the netlist. LEC is used to formally confirm that the function did not change after modifying the netlist. Uses Yosys. 
* **Antenna Diodes Insertion** - Special step during physical implementation. When a metal wire segment is fabricated and it is long enough, it can act as antenna. Reactive ion etching causes charge to accumulate on the wire. Transistor gates can be damaged during fabrication. 2 Solutions : Bridging attaches a higher layer intermediary (requires router awareness) ; Add antenna diode cell to leak away charges (antenna diodes are provided by SCL).
  
![note15](https://user-images.githubusercontent.com/118954022/213417580-77297663-e7ca-45e9-8884-09b3b0de0f05.jpg)

* With openLane, we took preventive approach by :
   * Adding a fake antenna diode next to every cell input after placement.
   * Run the antenna checker (Magic) on the routed layout.
   * If the checker reports violations on the cell input pin, replace the Fake Diode Cell by a real one.

* **Static Timing Analysis (STA)** - RC Extraction: DEF2SPEF. STA: OpenSTA (using OpenROAD). Involving timing reports to check violations in timing paths.
* **Physical Verification DRC & LVS** - Magic is used for Design Rule Checking and SPICE Extraction from Layout. Magic and Netgen are used for LVS where extracted SPICE by Magic vs verilog netlist are used.
* **Post Routing Evaluation** of results - DRC and LVS are then performed using magic and netgen. Antenna checking is performed by either OpenROAD’s ARC (Antenna Rule Checker) or using magic. Extraction of parasitics from the routed layout is then done using SPEF EXTRACTOR, followed by another round of static timing analysis to have more accurate timing reports that correspond to the actual physical layout.

The Final outputs of the flow, among various physical views and reports, are mainly GDSII and LEF views, which can be used in bigger designs.
 
Source : https://woset-workshop.github.io/PDFs/2020/a21.pdf
  
OpenRoad Project : https://www.youtube.com/watch?v=p2HVoj6OhaI&t=9s 
  
------------------------------------------------------------------------------------------------

## LABS 

**Open-source EDA Tools**

### OpenLANE Directory Structure

OpenLANE is not a tool but a flow that is comprises to many EDA tools i.e. Yosys, etc. We will see on onvoking OpenLane.

Home work dirctory listing.

![1 0](https://user-images.githubusercontent.com/118954022/213520082-67b09e60-ebb6-4749-aaa6-d053130c4204.jpg)

Note : To know more info about the command in linux, >> <command> -- help ,eg: >> ls --help

Then , cd openlane and explore. 'pdks' - process design kits. skywater-pdk : contains pdk dedicated files like timing_lib. 'open_pdks' : needed to convert commercial foundry to be compatible with its tools. 'sky130A' : to make compatible to open source environment (pdk variant). 

![lab1 1](https://user-images.githubusercontent.com/118954022/213520134-5507c664-6398-494b-9df3-d56d0d982e0b.jpg)

'libs.ref' contains all technology and process specific files. 'libs.tech' are specific to the tools.

![lab1 2](https://user-images.githubusercontent.com/118954022/213524696-f92ce07a-5cfe-474d-a999-9ec35694b984.jpg)

In sky130_fd_sc_hd/lib , contains all libs that are to know all PVT corners. 

![lab1 3](https://user-images.githubusercontent.com/118954022/213526098-772a233e-8500-47be-a488-494b35eb7e3b.jpg)

### Design Preparation Step

Invoke the tool (steps need to be done everytime), >> cd openlane ; make mount ; bash. >> pwd ; ls -ltr ; ./flow.tcl -interactive ; package require openlane 0.9 (import the packages we need); prep -design picorv32a (design choosed and taken);

![lab2 0](https://user-images.githubusercontent.com/118954022/213531475-30cef3e8-612c-429e-8c16-fe0ec47b7dc8.jpg)

The designs all are at cd .../openlane/designs . Design name 'picorv32a' was taken from here. In cd picorv32a, vim config.tcl (bypass default value, contains clock values) and vim sky130A_sky130_fd_sc_hd_config.tcl . 'tlef' - technology LEF.

![lab2 1](https://user-images.githubusercontent.com/118954022/213538385-7d05cb91-d20b-425b-b127-d69f2953dcfb.jpg)

### Review Files after Run Synthesis

In terminal, opnelane >> cd ../openlane/designs/picorv32a/runs/19-01_18-36/tmp ; ls -ltr ; vim merged.lef (the file created merging lef in openlane); cd .. ; vim cmds.log ;

merged.lef (contains layer, wire, cell, macro level related info)
![lab3 0](https://user-images.githubusercontent.com/118954022/213547668-6f2b370a-b0a6-4911-81e3-40bc4b1b113e.jpg)

cmds.log
![lab3 1](https://user-images.githubusercontent.com/118954022/213548982-569be465-2ed3-48e9-ab73-cf4bbb66eaee.jpg)  

Synthesis results will be in ../picorv32a/runs/19-01_18-36/results once it done. There will be reports also in 'cd reports' . 'config.tcl' is important where any modifications or updates made, we can refer wether it has made the changes or not. It shows the default parameter taking by run basically.
  
In opnelane (after preparation complete), >> run_synthesis ; 
  
<img width="185" alt="image" src="https://user-images.githubusercontent.com/118954022/213551111-62d7c3c4-66ca-4519-ade9-215456a49a12.png">
  
### OpenLANE Project Git Link Description

More about OpenLANE (Setting up and running openlane,openlane architecture,regression,hardening macro, etc.) : https://github.com/efabless/OpenLane

The OpenLane Documentation : https://openlane.readthedocs.io/en/latest/

OpenLANE Workshop : https://gitlab.com/gab13c/openlane-workshop

Youtube : https://www.youtube.com/watch?v=EczW2IWdnOM and https://www.youtube.com/watch?v=Vhyv0eq_mLU

### Steps to Characterize Synthesis Results

The synthesis is successfull. From the statistic report, we can observe that **Flop Ratio** = Num of Flop/Num of cells = 1613/14876 = 10.84% .

![lab5 0](https://user-images.githubusercontent.com/118954022/213555473-f5749da5-7aaa-4c17-a38e-4052f2891049.jpg)

View the results, in terminal, >> cd ../picorv32a/runs/13-01_14-09/results/synthesis ; vim picorv32a.synthesis.v ; (mapping all done, netlist is synthesized)
  
![lab5 1](https://user-images.githubusercontent.com/118954022/213557696-92de397a-827c-4cdf-9345-401722da1c3f.jpg)
  
Then, >> cd ../picorv32a/runs/13-01_14-09/reports/synthesis ; vim 1-yosys_4.stat.rpt ; vim 2-opensta.rpt ;

Statistic report :
![lab5 2](https://user-images.githubusercontent.com/118954022/213558673-a2a39733-28e9-45a9-b230-9dcb685d1bb1.jpg)

STA report :
![lab5 3](https://user-images.githubusercontent.com/118954022/213558639-21cb606c-8517-4858-8e23-e5876e16fb78.jpg)


------------------------------------------------------------------------------------------------

# #Day_16 

**Good Floorplan vs Bad Floorplan and Intro to Library Cells**

## Chip Floor Planing Considerations
  
**Floorplan** is the process of deriving the die size, allocating space for soft blocks, planning power, and macro placement etc. We specify the floorplan by Size or Die/IO/Core Coordinates. We derive core and module sizes based on the standard cell utilization.

Floorplan Stages :
1. Find Height and Width of Core and Die.
2. Define Location of Preplaced Cell.
  
### **Utilization Factor and Aspect Ratio**

Defining Width and Height of the Core and Die :

![note1 0](https://user-images.githubusercontent.com/118954022/214104347-908ac5f9-dbcb-4017-8684-a2cbefc0c001.jpg)

Lets take a netlist as example, with 2 flops and 2 gates(comb logic). Netlist basically decribes the connectivity of an electronic design.

![note1 1](https://user-images.githubusercontent.com/118954022/214105712-484e4d05-82db-4f91-a493-f1b2f563a67c.jpg)

We are dependent on the dimensions of logic gates. Convert the components/symbols into physical dimension.

![note1 2](https://user-images.githubusercontent.com/118954022/214106452-9d301301-69c4-4f66-a904-e265bdb31280.jpg)

Focus on the dimensions of the standard cells, not the wires. So, lets give a rough dimensions (assume).

![note1 3](https://user-images.githubusercontent.com/118954022/214107459-342ea8e3-e42b-4afd-bab0-4b7570691394.jpg)

Lets calculate the area occupied by the above netlist on a Silicon Wafer. Brakes the wire and place it in sigle grid. Min area assumed is 2x2 = 4 unit^2.

![note1 4](https://user-images.githubusercontent.com/118954022/214108125-a94fe89f-132c-4139-80ec-b9fcc7111fa1.jpg)

**Core** - The section of the chip where the fundamental logic of the design is placed. **Die** - Consists of core (encapsulate the core), it is a small semiconductor material specimen on which the fundamental circuit is fabricated. Utilize it by placing above netlist in the core. Note: in some cases, if there is some areas left out, it will not be 100% utilization.

![note1 5](https://user-images.githubusercontent.com/118954022/214110104-3a8ffe66-aa29-41ef-9511-22e0e23ff802.jpg)

![note1 6](https://user-images.githubusercontent.com/118954022/214110587-f17ad5b8-aac5-4efa-9fe3-6c4f089ea553.jpg)

**Utilization factor** - area occupied by netlist / total area of core. Since utilization factor = 1, equivalent to 100% utilization, and if there is some extra logic needs to be added, that is not allowed because there is no space left. This 100% (1) utilization is usually as an ideal scenario, but in practical scenario, we only utilized up until 50% (0.5) to 60% (0.6) utilization. Whenever the aspect ratio = 1, it signifies that the chip is in square-shaped. Else if aspect ratio is other than 1, it signifies that the chip is in rectangular-shaped.

![note1 7](https://user-images.githubusercontent.com/118954022/214112975-4ace871e-e986-43ad-81cf-3f5df051cf27.jpg)

Another example with rectangle core. With 50% utilization, can futher place extra logics in the core. 

![note1 8](https://user-images.githubusercontent.com/118954022/214114437-d8203539-9b7f-49dc-96d7-cb3fced7f504.jpg)

### **Concept of Pre-placed Cells**

Continue on defining width and height of the core and die. Anothe example, let say the core and die is bigger. The core has been utilized with 25% of the combinational logic and it has another 75% space which can be used for any additional cells. The free space can be used for more additional layers of routing.

![note2 0](https://user-images.githubusercontent.com/118954022/214367290-9da95745-52cf-4a76-b029-0d5123275036.jpg)

Define Location of Preplaced Cell : 

![note2 1](https://user-images.githubusercontent.com/118954022/214367539-84922700-4db3-4b35-a06c-72193fc7e7b0.jpg)

Lets look on **Pre-placed Cell** means. Combinational logic basically does some amount of functions, eg: memory, multiplier, mux, complex clock divider or etc. It does big task and the output is some huge circuits. Therefore, we need to extract it out and divide that huge output circuits into multiple blocks and then separate the netlist out into different blocks and implement seperately.

![note2 2](https://user-images.githubusercontent.com/118954022/214369099-f3c99140-23b2-4f6e-a83a-90d07b3c384f.jpg)

Next, with the 2 seperate block, extend the i/o pins. Block 1 with input pins and Block 2 with output pins. Then, detached those blocks with the black boxes (invisible at top level netlist). We will now separate the black boxes as two different IP's or modules. Basicaly is reused model concept. The advantages : More convenient to use them for multiple times when needed with different users where they will be implemented separately based upon their functionalities. Also, those blocks can be reused separately for each block for multiple times when needed. 

![note2 3](https://user-images.githubusercontent.com/118954022/214371017-0393e404-191a-49c4-b3d2-1030328cc00b.jpg)

Once being placed, it will fixed at the same location, will not affect by routing or any changes). All of the IPs can be implemented once and can be instantiated multiple times onto a netlist. However, this is no need to be implemented for multiple times because this is a part of top-level netlist where they perform some functions, where they receive some inputs signals, they deliver some output signals, but the functionality of the particular cells will be implemented only once. Since they are being placed before the routing, they are called pre-placed cells. All above are Macro/IP cells which are complex logic and reused multiple times in the circuit but only implemented once.

![note2 4](https://user-images.githubusercontent.com/118954022/214373225-b5b84304-a012-4ce0-878b-a69f72242cb7.jpg)
  
### **De-coupling Capacitors**

Continue on defining on pre-placed cells. A **Decoupling Capacitor** is a capacitor used to decouple (Eg: prevent electrical energy from transferring to) one part of a circuit from another. For higher frequencies, an alternative name is bypass capacitor as it is used to bypass the power supply or other high-impedance component of a circuit. 
  
Now as example, consider there are three pre-placed cell blocks, block A, block B, and block C where we implemented memories for once and they will be reused for multiple times in the circuit. Most of the blocks are communicating with input pins. Hence, the blocks will be usually being placed near the input side depending on the design scenario/background. Once the location has been set to place the blocks, the location can't be changed. Therefore, the location needs to be very well defined.

![note3 0](https://user-images.githubusercontent.com/118954022/214513462-6dcfeb90-db62-4961-8d29-2284f1da36b5.jpg)

Surround Pre-placed Cells with Decoupling Capacitors :

The circuit represents any of one block. Example at F (green block) at the capacitor, when there is transition 0 - >1, this capacitor need to charge to represent logic 1 (current demand). When Vdd flows and drops happens due to resistance and inductance, Vdd' refers as the voltage drop. 
  
![note3 1](https://user-images.githubusercontent.com/118954022/214519018-68f132d6-f8e9-465a-ab26-48edccd52027.jpg)

If Vdd' goes below the noise margin, due to Rdd and Ldd, the logic '1' at the output of circuit won't be detected as logic '1' at the input of the circuit following this circuit. Huge physical distance among power supply and circuit.
  
**Noise Margin summary**. Anything that lies between Vol and Vil it is called as logic 0. Any voltage that lies between Vil and Vih is called as undefined region. **Undefined Region** - The logic can either moved from logic 1 to logic 0 or from the interception point of (b) to logic 0. Undefined region is a danger case. Anything that lies between Vih and Voh it is called as logic 1 or 1V. Therefore, we have to ensure that the voltage didn't enter in undefined region since it cannot be identified whether the voltage might be in logic 1 or not. That is the problem when we are having a large physical distance from the main power supply to the circuit.
  
![note3 2](https://user-images.githubusercontent.com/118954022/214522258-f4e7f57c-a7d8-4a99-9242-e62339a55361.jpg)

So, the solution is to add decopuling capacitors in parallel with the circuit. It decouple the circuit from the supply. The decoupling capacitor is a huge capacitor which is completely be filled with the charge and the equivalent voltage across the decoupling capacitor is similar to what we have in the power supply. When there is switching activity in the circuit, the decoupling capacitor will supply current. Now there is low possibility of having voltage drop since it is nearer to the circuit. 
  
![note3 3](https://user-images.githubusercontent.com/118954022/214528363-4a7dadbd-1461-4489-88b6-468b8937817c.jpg)

So, now no switching activity will miss out and no cross talk. We have taken care the local communication. The overall view of pre-placed cells on a top-level netlist across the decoupling capacitors and the blocks.
  
![note3 4](https://user-images.githubusercontent.com/118954022/214530123-8da846c2-bd8a-4b58-94a2-e15bb85cd859.jpg)
  
### **Power Planning**
  
Let's take the previous circuit and treat it as a black box and denoted it as a macro/block. 

![note4 0](https://user-images.githubusercontent.com/118954022/214611490-2cf9aa4b-c1da-4bb9-8773-c609089e6e78.jpg)

Let say there are 4 different macros/blocks (so 4 Cd) containing driver, load, and etc that are usually available in a complete chip with different functionalities. The voltage source was supplied for 4 blocks. Hence, the supply from the source will not be stable where it is impossible to put all the decoupling capacitors. Let's assume the orange and blue line was 16-bit bus. Logic '1' indicates that the capacitor is being charged to Vdd while logic '0' will be discharged to the ground. This 16 bit bus is connected with the inverter, so the output will be inverted from the input. Logic '1' will be discharged and while logic '0' will be charged. All the capacitors that were charged to Volts will be discharged to 0V through single Ground tap point and this will cause a bounce/bump at Ground tap point. If this bounce exceeds the noise margin level, it will reaches undefined state, where the voltage might be changed from logic 1 to 0 and it is unpredictable. All capacitors which were '0' volt will have to charge to 'V' volts through single Vdd tap point. This will cause lowering of voltage at Vdd tap point. The level of Ground Bounce and Voltage Droop will be increased due to the multiple process of tap points happened at the same time. If this voltage droop is within the noise margin level, it is ok but if it exceeds undefined region in the noise margin level, it will be a danger zone. 

![note4 1](https://user-images.githubusercontent.com/118954022/214627248-1ffcb0e8-cb09-46c7-a39a-21c3a1774759.jpg)

With example circuit and with 16-bit bus. The output will be inverted once it is being fed into inverter. '1' refers to the capacitor is charged by Vdd and 0 is discharged to ground.

![note4 2](https://user-images.githubusercontent.com/118954022/214629428-1b2801a5-a769-4511-886f-daf3744445cd.jpg)

Ground bounce phenomena. If ground bounce exceed noice margin level, it is entering undefined state.

![note4 3](https://user-images.githubusercontent.com/118954022/214630885-2d128464-acad-494f-b9e2-8e7636488e79.jpg)

Voltage Droop phenomena. During charge, each of them demanding supply  at the same time. If this voltage droop is within the noise margin level, it is ok but if it exceeds undefined region in the noise margin level, it will be a danger zone.

![note4 4](https://user-images.githubusercontent.com/118954022/214632086-a04022d3-0e4c-4f03-958a-d79741c51b1e.jpg)

To solve this single power supply problem, we need to use multiple power supply (eg: multiple Vdd and Vss) instead of using 1 power supply only. Multiple power supply will be sourced to the nearest block and it will prevent the block from being missed to get the power supply. Therefore, all the logics will take the nearest power supply. The driver and the load also can be brought closed to each other in 'L' sense. Even the new logic, it can take the nearest supply and discharge to nearest ground.

![note4 5](https://user-images.githubusercontent.com/118954022/214638777-6193de46-977b-47f2-8cd3-c1bebf06cb1e.jpg)

### **Pin Placement and Logical Cell Placement Blockage**
  
Let's take some designs as examples that need to be implemented. Along with the circuit, there are some pre-placed blocks as well that is being connected to the input circuit and being clocked out. There are 4 designs in total with different connections to be looking through in this section. Each flops having different clock, so focus on the clock port and simplyfying it when merging complete design. By merging all of the four designs, it will be a complete design. The connectivity information between the gates are coded using VHDL/Verilog language and is called as **Netlist**.

![note5 0](https://user-images.githubusercontent.com/118954022/214643891-b7717a38-e1af-4e0f-b05f-2bd7b8308137.jpg)

The connectivity information between the gates are coded using VHDL/Verilog language and is called as **Netlist**.

Pin Placement : Pin Placement of complete design. In this design, the left side are all input ports and the right side are all output ports. Input ports and output ports are placed randomly since it is depending on our the design planning. The pins are placed randomly depending on the blocks. No cells/flip flops can be placed on the block a, block b and block c area. Clock ports which are CLK1, CLK2 and Clkout are bigger in size as compared to Data ports, since the clock is the ports that are driving all the cells and sending the signals to all flip flops. Bigger the size, least the resistance. Therefore, clock ports need to be bigger in size to avoid resistance during signal transmission since clock plays an important role in sending the signals. This is a work together where front end team defines netlist connectivity while the back end team decides pin placements. 

Logical Cell Placement Blockage : We block the particular area between core and die (the orange stripes) from placement and routing. This is to prevent automated routing tool place cell inside it. This area is reserved for the pin locations.

![note5 1](https://user-images.githubusercontent.com/118954022/214648326-47119e9e-2c59-402c-bb18-55c8a851b33e.jpg)

The Floor Plan is ready for Placement and Routing step.

## Library Binding and Placement
  
### **Netlist Binding and Initial Place Design**
  
### **Final Placement Optimization**
  
### **Need for Libraries and Characterization**
  

## Cell Design and Charcterization Flows 
  
### **Inputs for Cell Design Flow**
  
### **Circuit Design Step**
  
### **Layout Design Step**
  
### **Typical Characterization Flow**
  

## General Timing Charcterization Parameters
  
### **Timing Threshold Definitions**
  
### **Propagation Delay and Transition Time**

------------------------------------------------------------------------------------------------

## LABS

### **Steps to Run Floorplan using OpenLANE**

After completion of synthesis, now work on floorplan, >> cd ../Desktop/work/tools/openlane_working_dir/openlane/configuration ; vim README.md (file consists of all variables for each stage such as synthesis flow, floorplan decription, pins and ports placement, etc.). Variable in placement need to check congestion and make sure timing is met. PL - placement , FL - floorplan. 

![lab1 0](https://user-images.githubusercontent.com/118954022/214676295-a006fd71-d506-41b4-a3db-c25c0080b26b.jpg)

Then next, >> vim floorplan.tcl; (view floorplan parameters and switches). The metal hmetal and vmetal number is always add 1 in openLANE (in pic). 

![lab1 1](https://user-images.githubusercontent.com/118954022/214680519-26899186-0fb7-46ff-b6b2-18fe4b04ddea.jpg)

Previously in openlane/designs/picorv32a, >> vim config.tcl ; if we see there is no vertical and horinzontal metal showed. Usually it is shown.

![lab1 2](https://user-images.githubusercontent.com/118954022/214681011-0a6c632f-4924-460b-bb91-2cc03bf2eb36.jpg)

In Openlane terminal, >> run_floorplan 
  
<img width="263" alt="image" src="https://user-images.githubusercontent.com/118954022/214682175-0800ac4f-3a37-4658-8ae4-52a390079caf.png">
  
### **Review Floorplan Files and Steps to View Floorplan**
  
Define metal layer for I/O, then review this log file, >> cd .../openlane/designs/picorv32a/runs/13-01_14-09/logs/floorplan ; vim 4-ioPlacer.log ; There is no metal layers shown. Usualy got and the number is added with 1 compare to the metal layers number in config.tcl file.  
 
Next, >> cd .../openlane/designs/picorv32a/runs/19-01_18-36 ; vim config.tcl ; This is in run directory, tells us the configuration details taken by the flow. We can the parameters that is included in the current flow. We can see the core util value is same as the in sky..config.tcl in picorv32a directory. So the taken parameter are correct for the current run.
  
![lab2 0](https://user-images.githubusercontent.com/118954022/214687905-4a03a7a7-9aaa-4ec5-b558-753da95fc2a1.jpg)

List out location, >> cd .../openlane/designs/picorv32a/runs/19-01_18-36/results/floorplan ; vim picorv32a.floorplan.def ; The (0 0) is origin and ( x-axis y-axis ). So basically with this info, we calculate the area of die.
  
![lab2 1](https://user-images.githubusercontent.com/118954022/214689743-593c29a5-b089-4957-944c-eb2553b5f73e.jpg)

### **Review Floorplan Layout in Magic**
  
Invoke magic, >> magic -T ~/Desktop/work/tools/openlane_working_dir/pdks/sky130A/libs.tech/magic/sky130A.tech lef read ../../tmp/merged.lef def read picorv32a.floorplan.def & ;
  
![lab3 0](https://user-images.githubusercontent.com/118954022/214691550-32b09f60-3b5f-4757-9b2e-be809d7411be.jpg)
  
Press 'S' for select and press 'V' for centre. Left click then right click to select an area(a box formed). Press 'Z' to zoom in. Then place cursor above a component and press S, then above open tkcon tab and >> what ; to display info of the component. It is attached to metal layer 3.
  
![lab3 1](https://user-images.githubusercontent.com/118954022/214693847-3627aa0d-7149-40a2-a0c7-7625599769fe.jpg)

We can press on sub cells and other. Like this one is decap cell at side row named 'PHY_166'.
  
![lab3 2](https://user-images.githubusercontent.com/118954022/214694842-89054adc-8a97-4e52-b78f-6db6f2742457.jpg)

These are tap cells, to avoid the latches condition on CMOS devices. Their arrangement are diagonal to each other. 
  
![lab3 3](https://user-images.githubusercontent.com/118954022/214695127-7f7d1f1a-9c94-4c08-bff5-2b30a5d5db0c.jpg)

During floorplan, all standard cells are not placed in the design, all will be located at bottom left area. 
  
![lab3 4](https://user-images.githubusercontent.com/118954022/214696429-16b7cdc4-151a-460f-900e-5c0447e59b9c.jpg)

### **Congestion Aware Placement using RePlAce**
 
We are constraining the timing and make sure the congestion is less. There are 2 type of placements :
* **Global placement**: assigns general locations to movable objects. It used to reduce wire length.
* **Detailed placement**: refines object locations to legal cell sites and enforces non-overlapping constraints.
  
The detailed locations enable more accurate estimations of the circuit delay for the purpose of timing optimization. **Legalization** is an essential step where the overlaps between gates/macros must be removed in timing point of view. 
  
In openLane, >> run_placement ; Half Parameter Wire Length (HPWL) is applied to reduce wire length in OpenLANE. Our objective is to converge the overflow. If the overflow value is decreases, it means the design will converge (placement is going on).
  
![lab4 0](https://user-images.githubusercontent.com/118954022/214759143-f00ba8ab-c7e4-4e4c-a857-94d94e7d566b.jpg)

Lets se how design is palced. In terminal, >> cd ../openlane/designs/picorv32a/runs/19-01_18-36/results/placement ; magic -T ~/Desktop/work/tools/openlane_working_dir/pdks/sky130A/libs.tech/magic/sky130A.tech lef read ../../tmp/merged.lef def read picorv32a.placement.def & ; Now it is centralised floorplan and standard cells placement are get fixed(not movable). 

![lab4 1](https://user-images.githubusercontent.com/118954022/214761493-fea80ff0-a8a2-462b-90e7-6843a2a3a968.jpg)
  
  
------------------------------------------------------------------------------------------------

# #Day_17

**Design and Characterise Library Cell using Magic Layout and Spice Simulator**

References :
1. Github - https://github.com/nickson-jose/vsdstdcelldesign 
2. Overview of Physical Design flow - https://github.com/nickson-jose/vsdstdcelldesign#overview-of-physical-design-flow
3. Magic file - https://github.com/nickson-jose/vsdstdcelldesign/blob/master/sky130_inv.mag
4. .lib file - https://github.com/nickson-jose/vsdstdcelldesign/tree/master/libs

## Labs for CMOS Inverter ngspice Simulation

### **SPICE Deck Creation for CMOS Inverter**

### **SPICE Simulation Lab for CMOS Inverter**

### **Switching Threshold Vm**

### **Static and Dynamic Simulation of CMOS Inverter**


## Inception of Layout and CMOS Fabrication Process

### **Create Active Regions**

### **Formation of N-well and P-well**

### **Formation of Gate Terminal**

### **Lightly Doped Drain (LDD) Formation**

### **Source and Drain Formation**

### **Local Interconnect Formation**

### **Higher Level Metal Formation**


------------------------------------------------------------------------------------------------

## LABS

### **IO Placer Revision**

Cntinue of Day 16 lab. We going to use Inverter cell as example. We can change configuration, like input output strategy. In terminal, >> cd ../openlane/configuration ; vim floorplan.tcl ; The default is 1. Now we set it to 2 in openLane, >> set ::env(FP_IO_MODE) 2 ; run_floorplan ; 

![lab1 0](https://user-images.githubusercontent.com/118954022/214787227-cb9994ef-c500-4937-b9ca-e2f94dbb29a5.jpg)

Then invoke magic, >> cd ../openlane/designs/picorv32a/runs/19-01_18-36/results/floorplan ; magic -T ~/Desktop/work/tools/openlane_working_dir/pdks/sky130A/libs.tech/magic/sky130A.tech lef read ../../tmp/merged.lef def read picorv32a.floorplan.def & ; When default is 1 , it arraged in equal manner all over the side. After modified (=2), all stack at the left bottom.

![lab1 1](https://user-images.githubusercontent.com/118954022/214789751-210b9946-7478-4b6d-98d7-398f48c6dae9.jpg)

### **Steps to Git Clone vsdstdcelldesign**

In terminal, >> cd ../openlane_working_dir/openlane ; git clone https://github.com/nickson-jose/vsdstdcelldesign.git ; cd vsdstdcelldesign/ ;

![lab2 0](https://user-images.githubusercontent.com/118954022/214791640-75209d37-3e79-4a46-a1db-800681d550f8.jpg)

Tech file, >> cd ../openlane_working_dir/pdks/sky130A/libs.tech/magic ; cp sky130A.tech /home/parvin.rao.puspa.rao/Desktop/work/tools/openlane_working_dir/openlane/vsdstdcelldesign ;  .Then invoke magic to view CMOS Inverter, >> cd ../vsdstdcelldesign/ ; magic -T sky130A.tech sky130_inv.mag & ;

![lab2 1](https://user-images.githubusercontent.com/118954022/214795260-8235f49c-a45e-4621-9428-e3bbf6ee27ca.jpg)

### **Introduction to Sky130 Basic Layers Layout and LEF using Inverter**

CMOS Inverter 

![lab3 0](https://user-images.githubusercontent.com/118954022/214809828-129985f0-f3fc-4bc8-86bc-0fb6dbb1d8ea.jpg)

Press'S' 3 times to check connection : 

![lab3 1](https://user-images.githubusercontent.com/118954022/214812075-621881cd-a149-42c6-be66-2822c174daa3.jpg)

LEF only have metal layer, no information on logic path, only provide information on boundary/cell/length to place a cell. **Cell LEF** - an abstract view of the cell and only gives information about PR boundary, pin position and metal layer information of the cell.

More infromation on LEF - https://github.com/nickson-jose/vsdstdcelldesign#introduction-to-lef
 
### **Steps to Create std Cell Layout and Extract Spice Netlist**

The first step in magic layout tool is to create a bounding box (rectangle) with a width of 1.38 (3 x width(unithd)) and height of 2.72. This can be done by using command >> property FIXED_BBOX {0 0 138 272} ; in magic tkcon window. llx - lower left of x, lly - lower left of y, urx - upper right of x and ury - upper right of y value. 
  
![lab4 0](https://user-images.githubusercontent.com/118954022/214815723-59977bb6-79c2-454c-984d-000392cb836f.jpg)
  
This is followed by defining the ground and power segments (in metal 1), the respective contacts and finally the layout of the logic part. Same procedure can be followed for any standard cell layout. 
  
![lab4 1](https://user-images.githubusercontent.com/118954022/214816191-95b56c38-3030-457c-8382-1b6d5e22692e.jpg)

Checking DRC Violation. Click DRC tab -> DRC find next error. It will auto zoom to the area that need to fix error. Open and read the information regarding the violations through tkcon. To fix the violations, select the area (left click right click) and click the layer on the right. Then ensure the final design needs to be DRC clean (green light on at DRC).
    
![lab4 2](https://user-images.githubusercontent.com/118954022/214845447-fac57250-a401-4271-8352-7b227897dbb2.jpg)

In order to know logical fuctional, need to extract to SPICE and simulation in it. In tkcon, >> extract all  (To extract inverter); ext2spice cthresh 0 rthresh 0  (To extract all parasitic capacitance); ext2spice ; In the terminal in ../openlane/vsdstdcelldesign, a .spice file has created.
  
![lab4 3](https://user-images.githubusercontent.com/118954022/214846135-fef50b5a-98ec-4b23-8ffd-6792445a37fb.jpg)

## Sky130 Tech File Labs 

### **Steps to Create Final SPICE Deck using Sky130 Tech**
  
View sky130_inv.spice, in terminal >> vim sky130_inv.spice ;The C0 until C4 is drain gate source substrate. 'A' refers to Drain, 'Y' refers to Gate and 'VPWR' refers to Source. pshort and nshort refers to pmos and nmos respectively.

![lab5 0](https://user-images.githubusercontent.com/118954022/214880498-4bb0fbf4-5aa5-4d78-b421-327a008dd9ff.jpg)

Size of grid :

![lab5 1](https://user-images.githubusercontent.com/118954022/214881801-89546cd1-cb14-490a-bf49-3f90070c8db3.jpg)

Then check for must include nmos and pmos .lib files.

![lab5 2](https://user-images.githubusercontent.com/118954022/214882503-94a2f0fb-c69b-4863-aa54-3220b0bf5acc.jpg)

Then modify sky130_inv.spice file. Rename pmos -> pshort_model which in libs, same goes to nmos. Define supply voltages, comment out the //.subckt and //.ends .Then specify the input pulse and the specification for transient analysis.

![lab5 3](https://user-images.githubusercontent.com/118954022/214893966-5acdc225-ca0f-4a64-a1b1-ab07b0f0572a.jpg)

### **Steps to Characterize Inverter using Sky130 Model Files**

Plot graph. In terminal ../openlane/vsdstdcelldesign >> ngspice sky130_inv.spice ; plot y vs time a ;

![lab6 0](https://user-images.githubusercontent.com/118954022/214894744-49e569c7-38c1-42b6-9272-eb81ecef22cf.jpg)

To characterize cell, Find value of 4 parameters
* **Rise transition** - time taken for the output waveform to rise from 20% of max value to 80% of max value Vdd.
* **Fall transition** - time taken for output to fall from 80% to 20%.
* Cell rise/fall delay/propagation delay: the propagation delay where the output is rising/falling (50%).

Right click will create a box in the graph. Then it will open a new window. The axis value of the graph displayed at spice terminal.

**Rise transition output** (take the red line)

From 20% to 80%

**Fall transition input** (take the blue line)

From 80% to 20%

Cell delay (propagation delay)

**Rise delay**

**Fall delay**

### **Introduction to Magic Tool Options and DRC Rules**

Explore more about open circuit design at http://opencircuitdesign.com/ and browse through http://opencircuitdesign.com/magic/index.html and http://opencircuitdesign.com/magic/tutorials/tut9.html for some tutorial on Magic/Tech files/DRC.

**Magic**

Magic is an interactive system for creating and modifying VLSI circuit layouts. Magic has built-in knowledge of layout rules; as you are editing, it continuously checks for rule violations. Magic also knows about connectivity and transistors, and contains a built-in hierarchical circuit extractor.

**Caltech Intermediate Form (CIF)**

CIF and GDSII Stream Format are standard layout description languages used to transfer mask-level layouts between organizations and design tools. Magic can be used to read and write files in CIF and GDS formats. CIF is a file format for describing integrated circuits. CIF provides a limited set of graphics primitives that are useful for describing the two-dimensional shapes on the different layers of a chip. The format allows hierarchical description, which makes the representation concise. In addition, it is a terse but human-readable text format.

**Design Rule Checking (DRC)**

DRC verifies whether a specific design meets the constraints imposed by the process technology to be used for its manufacturing or not. 
* Examples of DRCs :
  * Minimum width and spacing for metal
  * Minimum area
  * Different net spacing
  * Short violation
  * Less than min edge length
  
More details on DRC - https://www.design-reuse.com/articles/41504/design-rule-checks-drc-a-practical-view-for-28nm-technology.html#:~:text=Description%3A%20This%20type%20violation%20pops,are%20seeing%20the%20VIA%20misalignment

### **Introduction to Sky130 pdk's and Steps to Download Labs**

In ~~/Desktop/work/tools >> wget http://opencircuitdesign.com/open_pdks/archive/drc_tests.tgz (To import magic layout into the tool); ls ; tar xfz drc_tests.tgz (to extract the file); cd drc_tests ; ls ; cat .magicrc  (info on whr to find tech file); 

![lab7 0](https://user-images.githubusercontent.com/118954022/214918940-97282f52-127c-4f48-8d3c-81f95a383313.jpg)

Start-up script for Magic. In terminal ../drc_tests, >> magic -d XR (for better graphics); .Then, select file --> open --> met3.mag. Note: select any object, press ";" to auto switch to another terminal.

![lab7 1](https://user-images.githubusercontent.com/118954022/214923346-812a55e1-095f-4818-abbb-5561c32ec73a.jpg)

In tkcon, >> drc why  (To check the violations on selected object);

![lab7 2](https://user-images.githubusercontent.com/118954022/214923215-dd9c79c6-5e11-45b4-a062-ac2fb2368f27.jpg)

### **Introduction to Magic and Steps to Load Sky130 Tech-rules**

* SkyWater Open Source PDK documentation - https://skywater-pdk.readthedocs.io/en/main/ and https://github.com/google/skywater-pdk 
* Periphery rules details - https://skywater-pdk.readthedocs.io/en/main/rules/periphery.html#denmos 

Select any area, click scroller of the mouse, and select m3contact using scroller. In tkcon, >> cif see VIA2  (to create VIA within m3contact); what ; feed clear  (to clear and undo); snap int ;

![lab8 0](https://user-images.githubusercontent.com/118954022/214927836-8f541237-a4a4-4f4c-b2e9-eb9d4784f6b5.jpg)

The distance between the cut and the edge is always larger and will never be smaller than 0.065. Via must enclosed with metal 3 atleast 0.065 micron, else will cause DRC violation.

### **Exercise to Fix Poly.9 Error in Sky130 Tech-file**
  
COntinue, In tkcon, >> load poly ; 

![lab9 0](https://user-images.githubusercontent.com/118954022/217039800-f09403f4-718b-4765-843d-35012bc0b99e.jpg)

There is one incorrect, which is Poly.9 .then, >> what; box; .It is a poly and npolyres. The distance ~ 0.22 microns. Based on the rules the poly spacing should be more than 0.48 microns. 

![lab9 1](https://user-images.githubusercontent.com/118954022/217043466-c7a175e7-f307-47c7-9ecf-624af15cafc2.jpg)

Let's correct it. In lab terminal, >> cd ../Desktop/work/tools/drc_tests ; vim sky130A.tech ; 

![lab9 2](https://user-images.githubusercontent.com/118954022/217045468-56a95bdf-41a4-4c13-954a-3b57c0cc625b.jpg)

Modifying sky130A.tech. Adding in allpolynonfet in a new line.

![lab9 3](https://user-images.githubusercontent.com/118954022/217045630-d7c10b55-3461-4520-acc5-b55ad638ecf0.jpg)

Then in tkcon >> tech load sky130A.tech (Reload tech file in Magic, easier); drc check  (Do drc checking); drc why ; .The spacing for the poly has been resolved. But, further action for diffusion and tap need to take.

![lab9 4](https://user-images.githubusercontent.com/118954022/217049494-53ccb4d7-96f5-42ba-a325-c4f52f3376da.jpg)

### **Exercise to Implement Poly Resistor Spacing to Diff and Tap**
  
Copy the resistor into 2 since there are several types of diffusion and tap. Add several things. Note: Green - ndiffusion and Brown - pdiffusion. The spacing length is > 0.33 microns. 

![lab10 0](https://user-images.githubusercontent.com/118954022/217052526-e94f25ec-21d3-4621-98f2-e2daca8b03af.jpg)

Then modify the tech file, in terminal >> vim sky130A.tech ; change '*nsd' --> 'alldiff'.

![lab10 1](https://user-images.githubusercontent.com/118954022/217053453-40d30742-14e9-4f39-ab6c-965229428d2b.jpg)

Then check in magic. All the rules are identified. 

![lab10 2](https://user-images.githubusercontent.com/118954022/217054166-182d894a-01b6-4cea-b035-f02857e0aff8.jpg)

### **Challenge Exercise to Describe DRC Error as Geometrical Construct**
  
in >> vim sky130A.tech, there is 'cifmaxwidth' - to check the layer as that appears in gds eventhough the layer can be drawn directly in the layout. 'nwell_missing' - defining special tech file, layer that defines a special cif output section in the tech file. Can refer to the rules in nwell part. 
  
![lab11 0](https://user-images.githubusercontent.com/118954022/217899971-a0660d4e-08f4-431a-b6b3-38bf9ec38da6.jpg)

In tkcon, >> load nwell.mag; .Look through nwell.6, deep nwell(dnwell) - yellow stripes and nwell - green dots pattern. The point of the rule is the edge of the dnwell needs to be covered with overlap all the way around by a ring of regular n-well. The outside distance rule could be implemented by a simple surround of drc rule, but the inside distance cannot be captured with a simple edge type rule. 
  
![lab11 1](https://user-images.githubusercontent.com/118954022/218026432-b0e3718c-f65b-4072-b3c9-47a2d7c6dde8.jpg)
  
We edit the tech file at the style drc section. The way the cifmaxwidth drc rules are implemented with width = 0, implies that the nwell_missing layer is whats leftover, if either the inside or outside dimension of nwell overlap dnwell doesn’t reach the required distance. Evrything in the difoutput drc style is implemented as a temp layer rather than a layer, all temp layers are basically support layers that are needed to get the right results for an output layer, but not appearing in the output themselves. The dnwell_shrink represents the largest open area that you can have inside the drawn dnwell. The nwell_missing layer starts with the dnweel layer, then it grows it by 400, which is the distance required by the surround rule, which gives us the smallest nwell variant that is needed to cover the dnwell.
  
![lab11 2](https://user-images.githubusercontent.com/118954022/218044216-458e15e8-e087-4519-b792-3fbd7764fc52.jpg)

Then in tkcon, >> cif ostyle drc  (Can only see layers for the cif layer style that is selected for the output); cif see dnwell_shrink  (To see the selected area); feed clear ;  cif see nwell_missing  (Shows the area which gets flagged with the error).
  
![lab11 3](https://user-images.githubusercontent.com/118954022/218045284-90e8d1f4-ee8e-4b0a-a9fc-c68a58be3af3.jpg)
  
In the tech file, we can see that there is 2 modes variables of drc can be choose to save compute time, fast (works for backend metal layers and large designs) and full ( for small layout design that can select full where Magic will check everything and suggest to use in interactive).

### **Challenge to Find Missing or Incorrect Rules and Fix them**

Lets see on rule nwell.4. So, since there is no distance associated with the rule, its impossible to write this as a simple edge based drc rule, but it does lend itself to a cifoutput rule very easily.
  
![lab12 0](https://user-images.githubusercontent.com/118954022/218054625-c1d94396-82b5-4d9c-91da-7a737d24c6ea.jpg)

We cannot directly placed in nsubstratecontact due to no distance association. 
  
Modify in tech file, terminal >> vim sky130A.tech ; 
  
![lab12 1](https://user-images.githubusercontent.com/118954022/218056864-4844acef-5525-4191-add0-6396b8f2b041.jpg)

Then in tkcon, >> tech load sky130A.tech  ; drc check ; drc style drc(full) ; drc check ; .If still have error so copy the nwell and add in the nsubstratencontact (blue x box) and recheck(drc style drc(full), the error is no more.
 
  
------------------------------------------------------------------------------------------------

# #Day_18

**Pre-layout Timing Analysis and Importance of Good Clock Tree**

Good Clock Tree must Skew Balance
* Timing point of view : Good clock tree converging the design, reduce the work load/timing spend to resolve the setup/hold violation.
* Power point of view : Good clock tree help in reduce power consumption. Clock signal consuming 70-80% power because signal keep changing throughout the chip.
* Area point of view : If bad clock tree will cause unclock sequential clock, need more buffer, clock gating issue that will lead to huge area.

More details on Clock Tree & PPA : https://semiwiki.com/ip/movellus/305173-performance-power-and-area-ppa-benefits-through-intelligent-clock-networks/ 

Good clock tree will achieve good result in PPA. Before clock trees is build only have setup. Hold will be in ideal (0 in value).

Engineering Change Order (ECO)
* Refers to a practice in the VLSI design flow to accommodate specification changes, to rectify functional errors, or to fix non-functional design requirements, such as timing and power, with minimal disturbance to the existing implementation, to save as much as possible the already-spent optimization efforts.

## Timing Modelling using Delay Tables

### Introduction to Delay Tables

### Delay Table Usage Part 1 and 2


## Timing Analysis with Ideal Clocks using OpenSTA

### Setup Timing Analysis and Introduction to Flip-flop Setup Time

###  Introduction to Clock Jitter and Uncertainty


## TritonCTS and Signal Integrity

### Clock Tree Routing and Buffering using H-Tree Algorithm

### Crosstalk and Clock Net Shielding


## Timing Analysis with Real Clocks using OpenSTA

### Setup Timing Analysis using Real Clocks

### Hold Timing Analysis using Real Clocks


------------------------------------------------------------------------------------------------

## LABS
  

## Timing Modelling using Delay Tables

### Lab Steps to Convert Grid Info to Track Info
  
**Library Exchange Format (LEF)**

A specification in which representing the physical layout of an integrated circuit in an ASCII format. It includes design rules and abstract information about the standard cells. LEF only has basic information required at that level to serve the purpose of the concerned CAD tool. Containing information on input, output, power and group port, does not consists logic path informations. Its objective is to extract LEF file from .mag file and then plug the file into the picorv32a flow (previous is standard cell library). There is a guidelines that need to be follow in creating a std cell set. The main one, is that the input and output ports must lie on the vertical and horizontal tracks. Second, the width of std cell should be based on the track pitch, and the height should be based on the track vertical pitch.

Open, ~/Desktop/work/tools/openlane_working_dir/pdks/sky130A/libs.tech/openlane/sky130_fd_sc_hd vim tracks.info ; This file provide information/specification for PnR flow, where does the route to growth for each metal layer. Then, cd ~/Desktop/work/tools/openlane_working_dir/openlane/vsdstdcelldesign magic -T sky130A.tech sky130_inv.mag ; Track information (using during routing stage) routes can go over the track/layer (metal traces). 

![lab1 0](https://user-images.githubusercontent.com/118954022/218837100-b64e7bc9-dd23-4d44-81b3-bc8d8e389732.jpg)

Set the grid based on the tracks.info (grid) converted the track into grid. Ports are on the intersection of the horizontal and vertical tracks. It ensures that the routes can reach the ports from x and y direction. Verified that both input and output ports have fulfilled the guideline where input and output ports lies at the intersection of horizontal and vertical tracks. Note: press "g" to activate grid (zoom in to see the grid). We can see after look after set the grid setting based on the track info as shown using the command “grid 0.46um 0.34um 0.23um 0.17um”.

![lab1 1](https://user-images.githubusercontent.com/118954022/218849422-a21eb1f4-86e1-4640-8c2e-9bd2930984dd.jpg)

![lab1 2](https://user-images.githubusercontent.com/118954022/218850475-afbc2383-b4ad-4bd6-b16d-cc98866856cc.jpg)

Confirm that both input and output ports are must lies on the intersection of vertical and horinzontal tracks.

![lab1 3](https://user-images.githubusercontent.com/118954022/218851798-4101f4e0-8ed6-4b82-b35f-8901aa8dc042.jpg)

Now we need to extract LEF to plug into design flow instead of using standard cell library as previous training. Guideline for making standard cell set:
* The input and output ports must lies on the intersection of vertical and horizontal tracks.
* The width/height of std cell should be in odd multiples of the x/y pitch of the tracks (the distance between two tracks is called a pitch).

Reference for more on pitch details : https://signoffsemiconductors.com/standard-cell-library/#:~:text=Pitch%20%3A%20The%20distance%20between%20two,layers%20as%20shown%20in%20Fig

### Steps to Convert Magic Layout to std Cell LEF
  
We follows second guideline where the width of std cell should be in odd multiples of the x and theheight of std cell should be in odd multiples of the y.
  
![lab2 0](https://user-images.githubusercontent.com/118954022/219095895-b1e668c8-b5aa-49b4-b06c-d4a47e4e1db5.jpg)

We need to only define layers, not ports in layout. Ports definitions are required when we want to extract LEF file. Ports will be defined as pins of a macro. We can use text helper to create the port in our design. The port number refers to the order in which the port is written in the lef file. This is how we define the ports for all the layers in the design.

**How to define ports?**
  
Select port --> Edit --> Text --> Fill those required information. Note: For A,Y in locali while for VPWR,VGND in metal1. 
  
![lab2 1](https://user-images.githubusercontent.com/118954022/219097101-901136a3-2a26-4b54-b041-fe7054224d48.jpg)

Then, define classes of ports (eg: let tool know VGND is ground).    

![lab2 2](https://user-images.githubusercontent.com/118954022/219098389-18e21fa9-236d-4367-af43-9b7b79b5f514.jpg)

Then, extract the LEF file. In tkcon, >> save sky130A_vsdinv.mag ; Then check the saved file in terminal lab, >> cd ~/Desktop/work/tools/openlane_working_dir/openlane/vsdstdcelldesign ; ls
  
Then,>> magic -T sky130A.tech sky130_vsdinv.mag ; In tkcon, >> lef write ;
  
![lab2 3](https://user-images.githubusercontent.com/118954022/219099837-89fa1cb6-3dbb-4811-b8a4-52f0be53279a.jpg)
  
Then, >> vim sky130_vsdinv.lef ; (port stated as pin in LEF)
  
![lab2 4](https://user-images.githubusercontent.com/118954022/219101103-0d95f8a5-4462-44ff-a7f7-16f4ce3d73df.jpg)

### Introduction to Timing Libs and Steps to Include New Cell in Synthesis
  
Modifying config.tcl file.First copy .lef file into src directory, >> cd ~/Desktop/work/tools/openlane_working_dir/openlane/vsdstdcelldesign ; cp sky130A_vsdinv.lef ~/Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/src ;.Then copy .lib file into src directory, >> cd ~/Desktop/work/tools/openlane_working_dir/openlane/vsdstdcelldesign/libs ; cp sky130_fd_sc_hd__* ~/Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/src ;.Then open, >> cd ~/Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/ ; vim config.tcl ; 
  
![lab3 0](https://user-images.githubusercontent.com/118954022/219103762-e4a03c9c-0ac2-4cd9-8974-93066a648b5b.jpg)
  
We did copy the newly written lef file into our design folder for picorv32a. This is so we can include the custom cell into the openlane flow, starting with the synthesis step. We need to ensure the abc step maps the cell appropriately, thus we need to have a library which has the cell definition.

Lastly, we need to modify our config.tcl to ensure the extra lef is read in frm the folder, based on the two commands that need to be run. The -tag and -overwrite options during prep -design is used to take in the new values and overwrite the old values in the runs. During synthesis, we can see the custom cell can be shown to be mapped in.
  
In terminal, >> cd ~/Desktop/work/tools/openlane_working_dir/openlane ; make mount ; ./flow.tcl -interactive ; package require openlane 0.9 ; prep -design picorv32a -tag 19-01_18-36 -overwrite  (Check run date at ls ~/Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/runs); set lefs [glob $::env(DESIGN_DIR)/src/*.lef] ; add_lefs -src $lefs ; run_synthesis ; Successfully invoke openlane and doing synthesis. In our synthesis we have a worst negative slack (wns) of -24.89, and total negative slack (tns) of -759.46.
  
![lab3 1](https://user-images.githubusercontent.com/118954022/219108808-0e522ef5-e11d-45e2-aa75-dead9542e683.jpg)
  
We need to try to find out how we can reduce these values by making the synthesis timing driven, by trying to strike a balance between the delay and the area. Will see in next lab.

### Steps to Configure Synthesis Settings to Fix Slack and Include vsdinv
  
Reference github: https://github.com/AngeloJacobo/OpenLANE-Sky130-Physical-Design-Workshop#day-5-final-steps-for-rtl2gds-using-tritonroute-and-opensta
  
In terminal, >> cd ~/Desktop/work/tools/openlane_working_dir/openlane/configuration ; vim README.md ; 
  
![lab4 0](https://user-images.githubusercontent.com/118954022/219110581-0e372f22-9400-4cd1-a10a-c52475fbdbd4.jpg)

**SYNTH_STRATEGY** : control the area and timing. **SYNTH_BUFFERING** : control if we want to buffer high fanout net. **SYNTH_SIZING** : control in cell sizing instead of buffering. **SYNTH_DRIVING_CELL** : ensure more drive strength cell to drive input.
  
In OpenLane terminal, perform refer to: https://github.com/AngeloJacobo/OpenLANE-Sky130-Physical-Design-Workshop#lab-part-3-day-4---fix-negative-slack 

![lab4 1](https://user-images.githubusercontent.com/118954022/219111850-08d95069-aefc-4e82-84d4-7d77d14cf1db.jpg)

**SYNTH_STRATEGY of Delay 0** -> the tool will focus more on optimizing/minimizing the delay, index can be 0 to 3 where 3 is the most optimized for timing (sacrificing more area). **SYNTH_BUFFERING of 1** -> ensures cell buffer will be used on high fanout cells to reduce delay due to high capacitance load. **SYNTH_SIZING of 1** -> will enable cell sizing where cell will be upsize or downsized as needed to meet timing. SYNTH_DRIVING_CELL is the cell used to drive the input ports and is vital for cells with a lot of fan-outs since it needs higher drive strength (larger driving cell needed).
  
Then, >> cd ~/Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/runs/19-01_18-36/results/synthesis ; rm -rf picorv32a.synthesis.v .In OpenLane, >> run_synthesis ; There is no more timing violation. 
  
![lab4 2](https://user-images.githubusercontent.com/118954022/219114167-6b04df42-f83f-4086-ba5d-e3fe9cf5795f.jpg)

In OpenLane, >> run_floorplan ; We will encounter with some errors. There is solution for this error. basic_macro_placement command is failing since EXTRA_LEFS variable inside config.tcl is assumed as a macro which is not. The temporary solution is to comment call on basic_macro_placement inside the OpenLane/scripts/tcl_commands/floorplan.tcl (this is okay since we are not adding any macro to the design). After that run_placement, another error will occur relating to remove_buffers, the solution is to comment the call to remove_buffers_from_nets in OpenLane/scripts/tcl_commands/placement.tcl. After successfully running placement, runs/[date]/results/placement/picorv32.def will be created.
  
So, modification goes on. In terminal, >> cd ~/Desktop/work/tools/openlane_working_dir/openlane/scripts/openroad ; vim or_basic_mp.tcl ; cd ~/Desktop/work/tools/openlane_working_dir/openlane/scripts/tcl_commands ; vim floorplan.tcl ;
  
![lab4 3](https://user-images.githubusercontent.com/118954022/219117412-4aca8f55-c94a-4622-a059-348de22f7dd1.jpg)

Then, in OpenLane >> run_floorplan ; run_placement ; Then in terminal, >> cd ~/Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/runs/19-01_18-36/results/placement ; magic -T ~/Desktop/work/tools/openlane_working_dir/pdks/sky130A/libs.tech/magic/sky130A.tech lef read ../../tmp/merged.lef def read picorv32a.placement.def ; 
  
![lab4 4](https://user-images.githubusercontent.com/118954022/219124585-f3a8d185-abac-4d23-a243-33cfbe65f497.jpg)
  

## Timing Analysis with Ideal Clocks using OpenSTA

### Steps to Configure OpenSTA for Post-synth Timing Analysis
  
In terminal, >> cd ~/Desktop/work/tools/openlane_working_dir/openlane ; vim pre_sta.conf (For pre-layout timing analysis). Then, >> cd ~/Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/src ; vim my_base.sdc (crete my_base.sdc file); cd ~/Desktop/work/tools/openlane_working_dir/openlane/vsdstdcelldesign/libs ; vim sky130_fd_sc_hd__typical.lib ;

![lab5 0](https://user-images.githubusercontent.com/118954022/219464253-db281120-c31c-421e-8659-920a9c29c134.jpg)

Then check for negative slack, >> cd ~/Desktop/work/tools/openlane_working_dir/openlane ; sta pre_sta.conf (invoke sta to check timing);

![lab5 1](https://user-images.githubusercontent.com/118954022/219464686-70197dea-5754-4f63-9ac9-c22a83f8d8e2.jpg)

### Steps to Optimize Synthesis to Reduce Setup Violations
  
Ignore hold report first, will review it after post-CTS. Currently is ideal. 

![lab6 0](https://user-images.githubusercontent.com/118954022/220564180-2919720b-4f02-42d9-9b84-ecb90befc027.jpg)

Then, >> cd ~/Desktop/work/tools/openlane_working_dir/openlane/configuration ; vim README.md ;

![lab6 1](https://user-images.githubusercontent.com/118954022/220565870-950e966a-de9b-45fc-a4f4-f7ed2e7de800.jpg)

In OpenLane, >> cd ~/Desktop/work/tools/openlane_working_dir/openlane ; echo $::env(SYNTH_MAX_FANOUT) ; set ::env(SYNTH_MAX_FANOUT) 4 (this to set to 4 and rerun synthesis);Then, cd ~/Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/runs/19-01_18-36/results/synthesis ; rm -rf picorv32a.synthesis.v ;We can see the value of tns decrease. 

<img width="281" alt="image" src="https://user-images.githubusercontent.com/118954022/220567747-001ee6c8-7ab9-48f1-99f5-a2a7311f9269.png">
![lab6 2](https://user-images.githubusercontent.com/118954022/220568650-bd6faef9-93c6-49da-9005-f53d84d7c24f.jpg)

Then in openlane, >> run_synthesis ;Then, >> cd ~/Desktop/work/tools/openlane_working_dir/openlane ; sta pre_sta.conf ; report_net -connections _18242_ ; replace_cell _41952_ sky130_fd_sc_hd__dfxtp_4 (This picks the highest fanout, cap, slew and replace the worst violations of the cell by increasing drive strength, upsize cell from 2 to 4); report_checks -fields {net cap dlew input pins} -digits 4 ; report_tns ; report_wns ;. We can after upsized, the timing violation has been improved and decreased. 

![lab6 3](https://user-images.githubusercontent.com/118954022/220570534-4c2cecde-7033-464e-8bec-993196946535.jpg)

There is huge load with cap 0.11 and causing slew 0.87. After upsive we can see timing violations has improved along with tns and wns. 

![lab6 4](https://user-images.githubusercontent.com/118954022/220571769-8765dbe1-8ea0-4021-a720-b0e17ddb2a2e.jpg)

### Steps to do Basic Timing ECO
  
We can use 'report_checks -from -through'. >> report_checks -from _41952_ -through _41879_ ;. After upsize cell, we can see the delay reduced to 0.99 from 1.20(previous).

![lab7 0](https://user-images.githubusercontent.com/118954022/220574539-94e4577b-b807-4795-b195-50fed59b9914.jpg)

## TritonCTS and Signal Integrity

### Steps to Run CTS using TritonCTS
  
In Terminal, >> write_verilog ~/Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/runs/19-01_18-36/results/synthesis/picorv32a.synthesis.v (overwrite the file after ECO netlist file done save); cd ~/Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/runs/19-01_18-36/results/synthesis ; ls -lrt picorv32a.synthesis.v ; date ;

Then in Openlane, >> run_floorplan ; run_placement ; run_cts ; Then, >> cd ~/Desktop/work/tools/openlane_working_dir/openlane/configuration ; vim README.md ;. Here is the variables for CTS. 

![lab8 0](https://user-images.githubusercontent.com/118954022/220578093-5a73e862-340a-4f3a-89c8-113f0cbef140.jpg)

After run cts, there will be new file generated " picorv32a.synthesis_cts.v ".

### Steps to Verify CTS Runs
  
>> cd ~/Desktop/work/tools/openlane_working_dir/openlane/scripts/tcl_commands ; vim cts.tcl ;. In this directory, it consists all commands used in each stage. There is proc run_cts. 

![lab9 0](https://user-images.githubusercontent.com/118954022/220581375-68ea78d8-94c7-4c80-addc-5e0440c12512.jpg)

In cts.tcl, it will further pass control to another file.

![lab9 1](https://user-images.githubusercontent.com/118954022/220581785-0be7edf2-95a2-4c9b-9984-71e3737d4aeb.jpg)

Each stage has its own .tcl file, except synthesis since it is not in openROAD. >> cd ~/Desktop/work/tools/openlane_working_dir/openlane/scripts/openroad ; vim or_cts.tcl ;

![lab9 2 0](https://user-images.githubusercontent.com/118954022/220582750-0e46951f-22f9-4295-bb5f-1f6d1c4b4b08.jpg)

In openLane, >> echo $::env(LIB_TYPICAL) ; echo $::env(CURRENT_DEF) ; echo $::env(CTS_MAX_CAP) ; echo $::env(CTS_CLK_BUFFER_LIST) ; echo $::env(CTS_ROOT_BUFFER) ;. We can check variables, value for cap , trans and etc. The max_cap value is the value at output pin of *_clkbuf_16. The value of capacitance is pick from .lib. The .def file will be use for future few stages like for power distribution and routing.

![lab9 3](https://user-images.githubusercontent.com/118954022/220585511-841ee314-ad3a-4628-8f8a-265834866078.jpg)
  

## Timing Analysis with Real Clocks using OpenSTA

### Steps to Analyze Timing with Real Clocks using OpenSTA
  
Reference : https://github.com/AngeloJacobo/OpenLANE-Sky130-Physical-Design-Workshop#timing-analysis-with-real-clocks 
  
In OpenLane invoke openRoad, >> openroad ; read_lef /openLANE_flow/designs/picorv32a/runs/19-01_18-36/tmp/merged.lef ; read_def/openLANE_flow/designs/picorv32a/runs/19-01_18-36/results/cts/picorv32a.cts.def ; write_db pico_cts.db ; read_db pico_cts.db ; 
read_verilog /openLANE_flow/designs/picorv32a/runs/19-01_18-36/results/synthesis/picorv32a.synthesis_cts.v ; read_liberty -max $::env(OPENLANE_ROOT)/designs/picorv32a/src/sky130_fd_sc_hd__slow.lib ; read_liberty -min $::env(OPENLANE_ROOT)/designs/picorv32a/src/sky130_fd_sc_hd__fast.lib ; set_propagated_clock [all_clocks] ; read_sdc designs/picorv32a/src/my_base.sdc ; report_checks -path_delay min_max -format full_clock_expanded -digits 4 ;.This step is not practical, therefore it violated. 
  
![lab10 0](https://user-images.githubusercontent.com/118954022/220589661-644ab86e-1448-4ea8-a084-f569607481d1.jpg)
  
This step is basically invoke openroad, read lef & def (from post cts), then write_db, read all, calculate actual cell delay, report timing (ignore hold-still no actual clock). In next routing stage will introduce resistance and capacitance. This will cause the delay to increase further. 

### Steps to Execute OpenSTA with Right Timing Libraries and CTS Assignment
  
Continue from previous lab, >> exit ; openroad (exit then open new openroad); read_db pico_cts.db ; read_verilog /openLANE_flow/designs/picorv32a/runs/19-01_18-36/results/synthesis/picorv32a.synthesis_cts.v ; read_liberty $::env(LIB_SYNTH_COMPLETE) ; link_design picorv32a ; read_sdc designs/picorv32a/src/my_base.sdc ; set_propagated_clock [all_clocks] ; report_checks -path_delay min_max -fields {slew trans net cap input pin} -format full_clock_expanded ; echo $::env(CTS_CLK_BUFFER_LIST) (view list of buffers);
  
![lab11 0](https://user-images.githubusercontent.com/118954022/220591350-522fdadc-08a6-4015-acad-6859de122c42.jpg)
  
The timing report generated previously was not proper, because in CTS stage is built based on typical corner, but the libraries that used for this analysis is min and max corner, so we need to set to typical library. Both timing are met after post CTS. The flow is not support analyze multicorner, so need to run seperately for each corner. The tool picked small cell first to meet the skew and area. Skew values are within 10% of the max clock period. 

### Steps to Observe Impact of Bigger CTS Buffers on Setup and Hold Timing
  
In openLane rerun cts, >> exit ; echo $::env(CTS_CLK_BUFFER_LIST) ; set ::env(CTS_CLK_BUFFER_LIST) [lreplace $::env(CTS_CLK_BUFFER_LIST) 0 0] ; echo $::env(CURRENT_DEF) ; set ::env(CURRENT_DEF) /openLANE_flow/designs/picorv32a/runs/19-01_18-36/results/placement/picorv32a.placement.def (point back to placement def); run_cts ; 
  
Then invoke openRoad, >> read_lef /openLANE_flow/designs/picorv32a/runs/1/tmp/merged.lef ; read_def /openLANE_flow/designs/picorv32a/runs/19-01_18-36/results/cts/picorv32a.cts.def ; write_db pico_cts1.db ; read_db pico_cts1.db ; read_verilog /openLANE_flow/designs/picorv32a/runs/19-01_18-36/results/synthesis/picorv32a.synthesis_cts.v ; read_liberty $::env(LIB_SYNTH_COMPLETE) ; link_design picorv32a ; read_sdc designs/picorv32a/src/my_base.sdc ; set_propagated_clock [all_clocks] ; report_checks -path_delay min_max -fields {slew trans net cap input pin} -format full_clock_expanded ;. We can see now that all buffer changed from '1' to '2'and slack has been improved.
  
![lab12 0](https://user-images.githubusercontent.com/118954022/220602273-45e9f44a-8af9-4b27-b271-e94c91df8b78.jpg)

Then, >> report_clock_skew -hold ; report_clock_skew -setup ; set ::env(CTS_CLK_BUFFER_LIST) [linsert $::env(CTS_CLK_BUFFER_LIST) 0 sky130_fd_sc_hd__clkbuf_1] (Adding back clkbuf1); 
  
![lab12 1](https://user-images.githubusercontent.com/118954022/220603839-226fec20-6fd0-467a-9720-830fdb331a82.jpg)


------------------------------------------------------------------------------------------------

# #Day_19

**Final Steps for RTL2GDS using TritonRoute and OpenSTA**

Done Clock Routing, then proceed to Signal Routing.
* Implement the interconnect using the available metal layers as defined by PDK (there is 6 routing layers in sky130 PDK).
* Metal is tracks from a routing grid.
* Routing grid is huge, so required to divide and conquer. Global Routing - generates routing guides. Detailed Routing - use routing guides to implement the actual wiring.

Then will proceed to resolve DRC Violation and working on Power Distribution Net.

## Routing and Design Rule Check (DRC)

### Introduction to Maze Routing Lee’s Algorithm

Routing Stage process

**Maze Routing-Lee’s Algorithm [Lee 1961]** - Algorithm to find the shortest path between two nodes in a grid. **Routing** - The process of creating the physical wire connections within the design in which it helps in determining the best way of routing that can be done between two endpoints, the source, and the target, with the shortest distance as well as the least number of zig-zag turns. However, the algorithm needs to be aware of any blockages set that hinders any routing to be done in the particular area.

![note1](https://user-images.githubusercontent.com/118954022/221599783-d6300fc5-eb61-4edc-ae5a-5d3bbdb9b33a.jpg)

Steps in Lee's Algorithm

1) Create the routing grid behind the floorplan.
2) The two points were created which are the source and target. Algorithm will look for the best route to connect the two points with the help of the routing grid.
3) The tool will label the grid ground (adjacent of horizontal and vertical grid). However, it will not label the grid under the blockage and at the boundary.

![note2](https://user-images.githubusercontent.com/118954022/221600598-5d2de574-fa67-41c8-85e2-df7dbed5f115.jpg)

### Lee’s Algorithm Conclusion

It is preferable to choose the LHS instead of RHS of the figure below. It is because the chosen route in the LHS figure got the best route which is less bending (L-shaped) rather than the RHS figure. Therefore, LHS figure will proceed to do the global routing. Performing the routing for 1 route will be fairly simple, but when we have millions of start and endpoints to route between, this method will consume a lot of time and memory. Maze routing consumes more time and memory if the design is huge. There are some algorithms that can help to reduce the time and memory consumption such as line-search algorithm, stanner-tree algorithm.

![note3](https://user-images.githubusercontent.com/118954022/221601484-03a2cf7b-3c88-4206-8203-e842e7bf80eb.jpg)

### Design Rule Check (DRC)

Design Rule Check (DRC): the rules that should be followed whenever the routing of the design is performed. One of the rules may be the minimal **Wire Width**, where the width of the wire should be no less than a specified amount based on the limitations of the fabrication process. Another rule that is based on the fabrication process of lithography is the **Wire Pitch**, where the centre-to-centre distance between 2 wires should be no smaller than a certain distance. Another rule includes **Wire Spacing** rule, where distance between 2 wires should be no smaller than a certain distance. These are many rules that the tool needs to take into account when performing the routing of the design.

Can refer this website for more example and solution on DRC: https://www.design-reuse.com/articles/41504/design-rule-checks-drc-a-practical-view-for-28nm-technology.html

![note4](https://user-images.githubusercontent.com/118954022/221603495-9c35a166-ba37-4e1a-ab69-f9ee7b83e96e.jpg)

One type of DRC violation is a **Signal Short**, where two wires that are not intended to be connected becomes in contact on the same layer. This could lead to **functional failure**, so this needs to be taken care of. To fix this, we need to simply moving one of the wires onto a different metal layer. However, please keep in mind that there are new drc rules that need to be taken into account.

![note5](https://user-images.githubusercontent.com/118954022/221604716-7b67f225-ff51-409c-98e9-5d1727cfb39a.jpg)

New drc rules after fixing

**Via width** where the width of the via should be no less than a certain value. **Via spacing** where the distance between 2 vias cannot be less than a specific distance. Most of these DRC rules come from the lithographic process and the limitations that come with the technology.

![note6](https://user-images.githubusercontent.com/118954022/221605412-f9b539e0-fe86-4d1b-b349-aa8b2aa3dd6a.jpg)

Performing parasitic extraction, where the resistances and capacitances of the wires are extracted and will be used for further processes.

![note7](https://user-images.githubusercontent.com/118954022/221605519-0cfe915d-b6bc-4a68-a860-5c5eb2ce8e44.jpg)


## TritonRoute Features

### TritonRoute Feature 1 - Honors Pre-processed Route Guides

OpenLane routing stage consists of two stages:
  * **Global Routing** - Form routing guides that can route all the nets. The tool used is FastRoute.
  * **Detailed Routing** - Uses the global routing's guide to connect the pins with the least amount of wire and bends. The tool used is TritonRoute.
  
**Triton Route**

In fast routing, a rough routing draft is created. Fast routing is the engine which is used for global routing. During global routing, the region is divided into grid cells, which acts as a route guide for the TritonRoute to be used for the detail routing, where an algorithm is used to find the best connectivity between the points. It honours the preprocessed route guides (obtained after fast routes), wherein the tool attempts as much as possible to route within route guides. The tool assumes route guides for each net satisfies inter-guide connectivity. Triton route works on proposed MILP (Mixed integer liner programming) based panel routing scheme with intra-layer parallel and inter-layer sequential routing framework, to finds the best way to perform the routing. Intra-layer refers to the routing within a layer, while inter-layer routing refers to routing between layers, through the uses of vias.

![note8](https://user-images.githubusercontent.com/118954022/221608927-955fb102-73d7-4d93-8e2f-788f41197552.jpg)

### TritonRoute Feature 2 & 3 - Inter-guide Connectivity and Intra- & Inter-layer Routing
	
Preprocessed guides should have unit width and must be in the preferred direction of the layer. Global route is done by fast route, and the output would be the routing guide. The initial route guides are transformed into the preprocessed guides through splitting, merging, and bridging. Whenever the tool detected the route guide with non-preferred direction, it divides the route guide into unit widths, and then the route with preferred direction is merged, while the non-preferred direction route is bridged to be a route on another layer, which is the preferred direction for routing. This way, parallel routing with higher layers are avoided, as well as avoiding parallel plate capacitance.

Each layer or panel will have its own preferred routing direction assigned to it, in which the routes should be formed. Routing in higher layers will begin only once the routing the bottom layers have been completed. Two guides are connected if they are on the same metal layer with touching edges, or if they are on neighbouring metal layers with a non-zero vertically overlapped area.

![note9](https://user-images.githubusercontent.com/118954022/221609784-632b3dfd-61ca-40bb-a396-00deebfb6b3e.jpg)

Each unconnected terminal i.e. pin of a standard cell instance, should have its pin shape overlapped by a route guide. The purple box in the RHS figure below would be the routing guide on the metal 1 layer that would overlap with the unconnected terminal. 
  
### TritonRoute Method to Handle Connectivity

**Inputs** file needed for TritonRoute are the LEF file, DEF file, and the Preprocessed route guides. **Outputs** from the TritonRoute would be a detailed routing solution with optimized wire-length and via count. **Constraints** needed in TritonRoute are the route guide honouring, connectivity constraints and design rules.

TritonRoute handles connectivity through 2 ways:
* **Access Point (AP)** - On-grid point on the metal layer of the route guide, and is used to connect to lower-layer segments, upper-layer segments, pins or IO ports.
* **Access Point Cluster (APC)** - A union of all Access Points derived from the same lower-layer segment, upper-layer guide, a pin or an IO port.

Access point refers to the point where the via can be placed to allow connectivity between layers. The objective of the Mixed Integer Liner Programming (MILP) is to connect one access point to another optimally. Choose one of the access points where the via should be dropped. Then, determine how the first access point will be connected to the next access point.

Handling connectivity:
* Connect one access oint to another access point optimally.
* There is multiple access point, so need to pick the right one.
* Need to connect layer by layer.

![note10](https://user-images.githubusercontent.com/118954022/221612552-35868f5d-638d-445f-9e09-474a9fd3cbab.jpg)

Algorithm use for optimizing routing :
* Need to find the cost among two APC.
* Then need to find minial and optimal for APC.

![note11](https://user-images.githubusercontent.com/118954022/221612635-066ba5c9-90bb-458b-9110-9d7690f387f2.jpg)


------------------------------------------------------------------------------------------------

## LABS


## Power Distribution Network and Routing

### Lab Steps to Build Power Distribution Network
  
If already from openLane, then do this, >> cd work/tools/openlane_working_dir/openlane ; make mount ; pwd ; ls -ltr ; ./flow.tcl -interactive ; package require openlane 0.9 ; prep -design picorv32a -tag 13-01_14-09 ;. If we want to retain the configurations from the last openlane job, we need to use '**prep -design -tag**'. If we want to create a fresh run with new configurations but without changing the tag name, we need to use '**prep -design -tag -overwrite**'.
  
In OpenLane, >> echo $::env(CURRENT_DEF)  (to ensure current_def is on the CTS stage and we will know we have done until which stage); gen_pdn  (to generate power distribution network);. Error encountered during “**gen_pdn**” in which the stage cannot perform routing as current_def has not changed to floorplan.pdn and it is due to incomplete proc in file. 
  
![lab1 0](https://user-images.githubusercontent.com/118954022/220697601-c347e49a-06e8-44a2-9b4e-9422364f740d.jpg)

![lab1 1](https://user-images.githubusercontent.com/118954022/220699417-f4a7aee7-f144-4e82-bf40-f8009c2b5e12.jpg)
  
### Lab Steps from Power Straps to std Cell Power
  
This is a review on PDN. If the power and ground rails has a pitch of 2.72, thus the customized inverter cell will have a height of 2.72 or else the power and ground rails will not be able to power up the cell. As shown below, power and ground flows from power/ground pads --> power/ground ring --> power/ground straps --> power/ground rails. 
  
Refernce : https://github.com/AngeloJacobo/OpenLANE-Sky130-Physical-Design-Workshop#timing-analysis-with-real-clocks
  
![lab2 0](https://user-images.githubusercontent.com/118954022/220705648-c741191f-684b-42aa-a91a-ea305bf3da6c.jpg)

BLUE is GND pad, RED is Power VDD pad, having 4 corners pads. Power and ground connect to ring and connect to chip through straps. Then connect to standard cells and macro cells through rails. The power and ground signals first go into the pads, into the power rings, then through the straps, and lastly, through the rails. 
  
### Basics of Global and Detail Routing and Configure TritonRoute
  
There will be a variable, ROUTING_STRATEGY in routing stage. The routing strategy specifies the optimization mode to be use in TritonRoute. There are 5 routing strategies. In this training we will proceed with default valu = 0, routing will not be optimal, but this option time saving and low memory consumption.
  
>> echo $::env(CURRENT_DEF)  (to ensure the .def file of pdn has been created) ; echo $::env(ROUTING_STRATEGY) ; run_routing ;. Then, >> cd ~/Desktop/work/tools/openlane_working_dir/openlane/configuration ; vim README.md ;. Assuming power distribution network has been successfully generated without being encountered by any error.

![lab3 0](https://user-images.githubusercontent.com/118954022/220722477-924dff25-88db-456e-89cb-1cedf86f73b0.jpg)
  

## TritonRoute Features

### Routing Topology Algorithm and Final Files List Post-route
  
Optimization algorithm for routing topology. 
  
For each APC, the algorithm needs to find the cost associated with the distance between 2 APCs which are the minimum spanning tree, MST, between the APCs and the costs. The objective of the algorithm is to find the minimal and most optimal point between the 2 APCs.
  
There are 3 violations. TritonRoute strategy = 0 is chosen right now. If TritonRoute strategy = 14 is chosen, there might be more violations due to high memory consume and it might take some time to finish the running. Therefore, we need to fix the violations manually. 
  
![lab4 0](https://user-images.githubusercontent.com/118954022/220725761-c49fba52-82a6-41e6-a5dc-444cba56a092.jpg)
  
Open file and review 3 violations which on li1 layer that needs to fix manually. The file is generated from global route. The file contains coordinate of each nets. When perform detail route, it will make sure its follow this routing guide. 
  
![lab4 1](https://user-images.githubusercontent.com/118954022/220728043-65bf786d-82db-42eb-85b7-b35562e29b60.jpg)

Creating a new spef file that requires merged.lef and picorv32a.def. Need to extract parasitic, need specific def and lef.Then generate out .spef file.

![lab4 2](https://user-images.githubusercontent.com/118954022/220729001-59393338-95de-40e3-ac8d-ccb359cdaabe.jpg)

Floorplan and placement has no change to netlist, so no .v files. CTS stage has insert buffer. Before routing has add in diode, the 3rd one also before routing. Post-STA will consume in the last one and will introduce another command read_spef.
  
![lab4 3](https://user-images.githubusercontent.com/118954022/220730023-453bcf19-7ab4-41fd-807a-e6648187d926.jpg)
  
  
------------------------------------------------------------------------------------------------

# #Day_20

**Floorplanning and Power Planning Labs**
  
## Lecture
  
Physical Design Flow :
  
<img width="643" alt="onenote1" src="https://user-images.githubusercontent.com/118954022/217070555-6e28efad-23f1-4250-8700-c6320c5fcd75.png">

References : 
  1) https://github.com/manili/VSDBabySoC/tree/main/src/lef
  2) Collaterals : https://github.com/kunalg123/icc2_workshop_collaterals
  3) https://www.vlsifacts.com/asic-physical-design-flow/
  4) https://asic-soc.blogspot.com/2007/10/physical-design-flow.html
  
------------------------------------------------------------------------------------------------

## LABS

Your Tasks 
  
* Step 1: 
Refer the repo for the skywater 130nm PDK files: bharath19- 
gs/synopsys ICC2flow 130nm: This repo is for synopsvs icc2 flow for skywater 
130nm PDK (github.com) 
  
* Step 2: 
Using the 130nm PDK reproduce the same as you have done using OpenSource 
tools in Synopsys tools, Refer the repo for ICC2 Flow/commands: 
Devipriya1921/VSDBabySoC ICC2 (github.com) 


------------------------------------------------------------------------------------------------

# #Day_21
  
**Placement and CTS Labs**

## Lecture

### Placement 
  
* Pre-Placement Sanity Checks Floating Pins in Netlist, Unconstrained Pins, Timing, Pin direction mismatch, etc. 
* What is Placement? 
  * Standard Cell 
  * Placement Stages ( Global Placement, Legalization, Detailed Placement )

* Placement Objectives/Quality Checks 
  * Congestion 
  * Performance 
  * Timing 
  * Routability 
  * Runtime

### Clock Tree Analysis (CTS)
  
* Inputs of CTS 
  * Placement DB 
  * CTS Spec File
  
* CTS steps 
  * Clustering 
  * DRV Fixing 
  * Insertion Delay Reduction 
  * Power Reduction 
  * Balancing 
  * Post-Conditioning 
  
* CTS Quality Checks 
1) Skew 
2) Pulse Width 
3) Duty cycle 
4) Latency 
5) Clock tree power 
6) Signal Integrity and Crosstalk (wait till Day27, until we do post-routing step) 

* Timing Analysis and Fixing 

CTS Free Course :
* https://www.udemy.com/course/vlsi-academy-clock-tree-synthesis/
* https://www.udemy.com/course/vlsi-academy-clock-tree-synthesis-part2/![image](https://user-images.githubusercontent.com/118954022/217073271-bfc88457-7ae3-49d3-8a9d-0f4e25c98fcb.png)
  
Reference :
* https://ivlsi.com/placement-vlsi-physical-design/
* https://ivlsi.com/clock-tree-synthesis-cts-vlsi-physical-design/#Clock_Tree_Synthesis
  
CTS Free Course 
 1) https://www.udemy.com/course/vlsi-academy-clock-tree-synthesis/
 2) https://www.udemy.com/course/vlsi-academy-clock-tree-synthesis-part2/


------------------------------------------------------------------------------------------------

## LABS

### Task 1 (Implement the same as previous sessions lab for Placement 
and CTS stages) 
  
* Step 1: 
Refer the repo for the skywater 130nm PDK files: bharath19-gs/svnopsvs ICC2flow 130nm: This repo is for synopsvs icc2 flow for skywater 130nm PDK (github.com) 
  
* Step 2: 
Using the 130nm PDK reproduce the same as you have done using OpenSource tools in Synopsys tools, Refer the repo for ICC2 Flow/commands: Devipriya1921/VSDBabySoC ICC2 (github.com) 
  
### Task 2 
  
Complete the CTS part 1 and part 2 courses that is been provided to you and try to implement the same for SKY 130 labs using ICC2.


------------------------------------------------------------------------------------------------


# #Day_22

**CTS Analysis Labs**

## Lecture

<img width="655" alt="onenote1" src="https://user-images.githubusercontent.com/118954022/217330214-1cdae9de-bfa7-4c47-9462-6e788cf3d217.png">

![note2](https://user-images.githubusercontent.com/118954022/217330715-a120b107-3789-4277-9b02-f32a122a5b46.jpg)

![note3](https://user-images.githubusercontent.com/118954022/217330780-e7ec990d-628c-4498-b9aa-9b314f90aabb.jpg)

Various CTS checks  
1. Skew check 
2. Pulse width check 
3. Duty cycle check 
4. Latency check 
5. Power check 
6. Crosstalk Quality check 
7. Delta Delay Quality check 
8. Glitch Quality check 
  
What does 'check clock tree' (our first go to command after placement) do ??
  
This command checks and reports issues that can lead to bad QoR such as on clock tree structure, constraints and clock tree exceptions.

How do we know if the placement done input is perfect ?? 
  
We use this command - 'check _ legality'. If it is legal — well and good, else use legalize_placement. Now, there are some default constraints. 
  
![note4](https://user-images.githubusercontent.com/118954022/217332784-06bb38bb-5710-40c5-adfd-615fddd4cb62.jpg)

We can edit those default constraints using - 'set_clock_tree_options'. '-max_capacitance', '-max_transition' are some examples (becareful keeping 
min and max values in sight).
  
![note5](https://user-images.githubusercontent.com/118954022/217333879-7986961d-c3b1-46c8-9725-ea890008347e.jpg)

IC Compiler uses the clock tree synthesis design rule constraints for all optimization phases, as well as for clock tree synthesis. For information about setting 
the clock tree synthesis design rule constraint, we can use ICC2 with debug mode. By using '-set cts_use_debug_mode true'. The main command we need to do is '-compile_clock_tree'.
  
![note6](https://user-images.githubusercontent.com/118954022/217334782-e65d8466-807f-4d92-a792-94ac97270cb0.jpg)

### CTS Results Analysis
  
![note7](https://user-images.githubusercontent.com/118954022/217336448-d0ecf536-0a66-47da-a408-8c65212d5bc9.jpg)

Now, after observing the reports, if we see the clock tree could be better, 'clock_opt' command, which performs clock tree synthesis and incremental physical 
optimization. This process results in a timing optimized design with fully implemented clock trees. The clock_opt command does the following: 
1. Performs clock tree power optimization 
2. Synthesizes(Re-Synthesizes) the clock trees
3. Optimizes the clock trees
4. Adjusts the I/O timing
5. Performs RC extraction of the clock nets and computes accurate clock arrival times
6. Performs placement and timing optimization

Sometimes there will be some unrouted clock trees, so to remove them, we use the command 'remove_clock_tree'.
  
### After CTS we do Synthesis 
  
Before we synthesize the clock trees, use the check_clock_tree command to verify that the clock trees are properly defined. 
  
' icc2_shell> check_clock_tree -clocks my_clk '

To understand CTS more, we can try do : 
1. Minimize skew only
2. Minimize skew and insertion delay 
3. Minimize skew and maximize insertion delay
4. Minimize skew and meet minimum insertion delay target

![note8](https://user-images.githubusercontent.com/118954022/217338385-65ce5cca-29b9-4804-b1ec-15b1838cfa23.jpg)
  
References :
* Udemy course - CTS1
* https://ivlsi.com/clock-tree-synthesis-cts-vlsi-physical-design/
* Full ICC2 Flow - https://prezi.com/-jmhi72feify/ic-compiler/ 
  
------------------------------------------------------------------------------------------------

## LABS

### LAB 1 - 

------------------------------------------------------------------------------------------------


# #Day_23
  
**Clock Gating Technique**

![note1](https://user-images.githubusercontent.com/118954022/220735135-08445f35-ff4d-4420-9e1f-042f449350b4.jpg)

Advanced H-Tree for Million Flop Clock End-points randomly Placed

Assume there is a digital circuit with a lot of clocks, now just imagine designing 
clock tree, which will be so huge, with so many buffers etc.  Now, the whole chip is sectioned into smaller versions and then each section will have its own clock tree, and then finally a complete routed tree.

![note2](https://user-images.githubusercontent.com/118954022/220736343-c1665f8b-f918-4776-ada9-802979e1e372.jpg)

Half/quarter Million of Buffers ?? 

Isn't that too much power? We have been worrying about clock tree only with respect to Area, Timing and etc. We forgot about another important factor - "Power". Now, we need to do CTS keeping power in mind - power "aware" CTS.

Clock Gating Technique using AND, OR Universal NAND Gate 

This is where we introduce Clock gating(CG). It has been found that 50% of the **dynamic power** originates from clock-related circuits. - source: low power vlsi design, AJIT PAL (this answers why CC?). So, what is CG? -> **Clock Gating(CG)** is one of the techniques used to save the dynamic power of clock elements in the design. Principle behind clock gating: The principle behind clock gating is to stop the clock of those sequential elements whose data is not toggling. RTL level code talks only about data transfer.

![note3](https://user-images.githubusercontent.com/118954022/220737533-975fd9ff-751e-4895-b960-d133630581c7.jpg)

Where/When is Clock Gating done ?? 

Inserted synthesis stage and optimized in the implementation stage(Physical Design stage). There are mainly three types of CG: 
* CG = AND gate 
* CG = OR gate 
* CG = Universal NAND gate

Following the Physical Design Flow, the last step is Routing. Making physical connections between signal pins using metal layers are called **Routing**. There is mainly 3 types of routing:
* P/G Routing 
* Clock Routing 
* Signal Routing 
  * Global Routing 
  * Detailed Routing 

Basic flow of Routing

![note4](https://user-images.githubusercontent.com/118954022/220739738-274d04e6-0e85-4f5a-bdc5-41c9ed669ed2.jpg)

------------------------------------------------------------------------------------------------

## LABS

Finish the udemy course for CTS-part 1 : https://www.udemy.com/course/vlsi-academy-clock-tree-synthesis/

------------------------------------------------------------------------------------------------

# #Day_24
  
**Timing Violations and ECO**

**Engineering Change Order** or **ECO** is how we incorporate last minute changes in 
our design. So typically we do ECO on the gate level netlist. Designer need to edit the gate-level netlist, make the same changes in RTL. Then pass all verifications before it is passed on to layout. Make sure the ECO pass formal and functional verification before you start editing your layout. In this stage all the violations are fixed and seal all the sign-off checks that weren't done during the PD flow.

ECO strategies in a nutshell. ECO has has the following steps : 
* Investigate the problem using the recent database .
* ECO generation to address the problem .
* ECO implementation with the recent database .
* After implementing and fixing the problem, save it in the database for future. 

ECO strategies :
* Margin based fixing 
  * Design rule violations(DRV) - max_cap and max_tran 
  * Setup and hold violations
* Selective endpoint biased fixing 
  * With and without margin 
  * With and without slack range 
* Slack based fixing 
  * Setup and hold target slack 
  * Max slack 
* Fix 'n' number paths 
  * Number of paths per group (max_paths) 
  * Number of paths per endpoint (nworst) 
* GBA(group based) and PBA(path-based)fixing 
* Full chip vs reg2reg fixing 
* Leakage fixing using HVT 
* Hierarchical ECO 
  * Top level only 
  * Individual 
  * Replicated hierarchies only 
  * All of the above 
* Physical aware ECO 
  * Routing congestion aware 
  * Cell legalization aware 
  * Buffer on route
  
References:
1. VSD-Clock Tree Synthesis - Part 2
2. Low power vlsi design, ajit pal

------------------------------------------------------------------------------------------------

## LABS

### Violations and Methods to fix

1. Finish the udemy course for CTS-part 2, and violations and ECO webinar. ( https://www.udemy.com/course/vlsi-academy-clock-tree-synthesis-part2/ )
2. There is slack violations in the design, try to fix it. 
	a. Latency needs to commented 
	b. Initial density (core utilization - initialize_fioorplan(under pre-floorplanning)) --> 40% 
	c. Clock needs to be propagated post-CTS , and for timing analysis post-placement clock should be ideal - (should have ideal in brackets) 
	d. Yishen's post layout timing reports 
The analysis column in report timing. Expectation - cells shown in the analysis column should be in the main column in post-layout timing reports.


------------------------------------------------------------------------------------------------


# #Day_25
  and 
**RISC-V Core RTL2GDS Flow**

## RTL2GDS Flow

Covered in Previous training on Day15 : https://github.com/Parvin16/sd_training#day_15 and lab notes on Day20 : https://github.com/Parvin16/sd_training#Day_20

------------------------------------------------------------------------------------------------

# #Day_26
  
**Introduction to Mixed-signal Flow**

## Lecture

Reference : VLSI Physical Design Flow(http://www.vlsisystemdesign.com)

What is **Mixed Signal Design**??

Electronic signal is  a message encoded by changing the voltage of an electric current. There are 2 types of electronic signals, Analog and Digital signals. Analog signals most available in the nature. Digital signals - basically I 's and 0's does microcontroller/ microprocessors understands or speak. Since the microprocessor/controllers speak in digital form, we use ADC's and DAC's  to get or take in analog signals.

Mixed-signal chips are those that at least partially deal with input signals whose precise values matter.This broad class includes RF, Analog, Analog-to-Digital and Digital-to-Analog conversion. More recently, a large number of Mixed-Signal chips where at least part of the chip design needs to measure signals with high precision. These chips have very different Design and Process Technology demands than normal Digital circuits.

**AMS** - analog and mixed signal(digital and analog). AMS Design Flow :

![note1](https://user-images.githubusercontent.com/118954022/221268599-e5933e2d-ec63-4800-94f0-efa2705c3a0e.jpg)

Block diagram representation for Mixed Signal Design :

![note2](https://user-images.githubusercontent.com/118954022/221268897-ed044486-dc2b-40e1-9c89-5e7fd1db770b.jpg)

Let us explore with the example of VSDBabySoC
* RVMYTH processor - digital block.
* PLL - analog block.
* DAC - analog block(for digital to analog conversion).

Introduction to Various Files

1) LEF file - Library Exchange Format file : Physical properties such as width, height etc regarding the standard cells.
   * Tf(technology file) or Tlef(technology lef) -contain same information.
   * Cell tf.

2) LIBerty file - contains the timing information of the cells.

3) gdsII and OASIS file. - GDSII is a file format similar to JPEG, DOCX, XLSX etc to enable a layout design to be transferred from one place to another(IP owner handoff to PD team, PD team to foundry for fabrication), to be viewed/used for verifications like Physical verification checks by EDA tools.

![note3](https://user-images.githubusercontent.com/118954022/221269609-b9da26d5-7235-45b5-8027-879118e16400.jpg)

Where to get the information in WHAT and WHY TO DO? This is where we need the following files:
* LEF file.
* LIB file.
* Tf files(tlu+ file).

![note4](https://user-images.githubusercontent.com/118954022/221270068-18a0dae7-d541-4d81-86f8-70960cdd3ff8.jpg)

Sources of various files

![note5](https://user-images.githubusercontent.com/118954022/221270299-04fe4c91-5abc-4886-b028-aa6fe4402408.jpg)

What are IP cores?

An **IP core** consists of a block of logic or data that is used in a semiconductor chip. It is usually the intellectual property of a particular person or company. IP cores are used when making a field programmable gate array (FPGA) or application-specific integrated circuit (ASIC).
IP cores are created throughout the design process and can be turned into components for reuse. There are different categories for IP cores including hard IP cores and soft IP cores. The soft IP core , can be customized during the physical design phase and mapped to any process technology. A hard IP core is one that has the logic implementation and the physical implementation. In other words, the physical layout of a hard macro-IP is finished and fixed in a particular process technology.

Just a diagram how it actually works in the semiconductor industry:

![note6](https://user-images.githubusercontent.com/118954022/221270660-973c1d42-e02c-46e4-bdab-9274c59765df.jpg)

References : 
1. https://www.ques10.com/p/27715/draw-and-explain-ams-design-flow-1/
2. https://www.cdeep.iitb.ac.in/slides/S15/EE719/EE719-L1.pdf
3. https://www.slideshare.net/vlsisyst/vlsi-physical-design-flow

------------------------------------------------------------------------------------------------

# #Day_27
  
**Introduction to Crosstalk - Glitch and Delta Delay**

## Lecture

Synopys trainings : https://solvnetplus.synopsys.com/s/

VSD - Signal Integrity udemy freee course : https://www.udemy.com/course/vlsi-academy-crosstalk/?couponCode=9C9DA98C9CDC80B3F70D

What is **Signal Integrity** and **Crosstalk**?
* Signal Integrity & Crosstalk are the Quality checks of the clock routes.
* Signal integrity is the ability of an electrical signal to carry information reliably and resist the effects of high-frequency electromagnetic interference from nearby signals.
* Crosstalk is the undesirable electrical interaction between two or more physically adjacent nets due to capacitive cross-coupling.
* Crosstalk is a type of noise signal that corrupts the actual signal while transmission through the communication medium.
* Reasons for Crosstalk and Fixes for Crosstalk.

Aggressor and Victim Nets
* A net that receives undesirable cross-coupling effects from a nearby net is called a victim net.
* A net that causes these effects in a victim net is called an aggressor net.

**Crosstalk-Glitch**
* When one net is switching, and another net is constant then switching signal may cause spikes on other net because of which coupling capacitance (Cc) occurs between two nets, this is called as crosstalk noise.
* Types of Glitches -> Rise, Fall, Overshoot, Undershoot.

![note1](https://user-images.githubusercontent.com/118954022/221271721-8fb5ebb0-7803-4f99-83a7-7e0445bd1b7c.jpg)

Performing Crosstalk Delay Analysis
1. Enable PrimeTime SI -> **set_app_var si_enable_analysis true**
2. Back-annotate the design with cross-coupling capacitance information in a SPEF or GPD file -> **read_parasitics - keep_capacitive_coupling file_name.spf**

Using check_timing
* Types to checking specific to crosstalk analysis:
  * no_driving_cell
  * ideal_clocks
  * partial_input_delay
  * unexpandable_clocks

Timing Reports
* report_timing
* -crosstalk_delta
* report_si_bottleneck
* report_delay_calculation –crosstalk
* report_si_double_switching
* report_noise
* **Viewing the Crosstalk Analysis Report** -> report_timing - transition_time -crosstalk_delta \ -input_pins -significant_digits 4

Bottleneck Reports
* report_si_bottleneck
* report_bottleneck
* delta_delay
* delta_delay_ratio
* total_victim_delay_bump
* delay_bump_per_aggressor
* To get a list of all the victim nets with a delay violation or within 2.0 time units of a violation, listed in order of delta delay -> report_si_bottleneck -cost_type delta_delay \ -slack_lesser_than 2.0

Bottleneck Reports
* report_delay_calculation –crosstalk
* size_cell
* set_coupling_separation
* -include_clock_nets
* minimum_active_aggressor
* In the following example command, the bottleneck command reports nets where three or more active aggressors are affecting the net -> report_si_bottleneck -cost_type delta_delay \ - minimum_active_aggressors 3

Crosstalk Net Delay Calculation
* report_delay_calculation -crosstalk \ -from [get_pins g1/Z] -to [get_pins g2/A]

Reporting Crosstalk Settings
* To check your crosstalk settings:
  * report_si_delay_analysis
  * report_si_noise_analysis
  * report_si_aggressor_exclusion
  
References : 
1) Overview of Signal Integrity and Crosstalk (synopsys.com)
2) CTS (PART-II) (crosstalk and useful skew) - VLSI- Physical Design For Freshers (physicaldesign4u.com)

------------------------------------------------------------------------------------------------

## LABS

### Glitch and Delta Delay 

------------------------------------------------------------------------------------------------

# #Day_28
  
**Introduction to DRC/LVS**

## Lecture

![note1](https://user-images.githubusercontent.com/118954022/221273496-4fe6518a-e499-4690-bc78-eb059badb072.jpg)

Physical Verification
* **DRC** (Design Rule Check): DRC checks determine if the layout satisfies a set of rules required for manufacturing.
* **LVS** (Layout vs Schematic): It is another major check in the physical verification stage. Here you are verifying that the layout you have created is functionally the same as the schematic/netlist of the design.
* **ARC** (Antenna Rule Checking): Process antenna effect or “plasma induced gate oxide damage” is a manufacturing effect.
* **ERC** (Electrical rule check): Involves checking a design for all electrical connections that are considered dangerous.
	
## Introduction to SkyWater SKY130
## DRC/LVS Theory
## Introduction to DRC Rules

------------------------------------------------------------------------------------------------

## LABS

### TASK

Step 1: Physical-Verification-using-SKY130/README.md at main · Emad-H/Physical-Verification-using-SKY130 (github.com) -> Go through the Repo, as a reference to do Step 2.

Step 2: https://www.vsdiat.com/dashboard -> Go to Physical Verification using Skywater 130nm technology Workshop.
	
## Check Tool Installations
## Creating Sky130 Device Layout In Magic
## Creating Simple Schematic In Xschem
## Creating Symbol And Exporting Schematic In Xschem
## Importing Schematic To Layout And Inverter Layout Steps
## Final DRC/LVS Checks And Post Layout Simulations
## GDS Reads
## Port
## Abstract Views
## Basic Extraction
## Setup for DRC
## Setup for LVS
## Setup for XOR
## Width Rule And Spacing Rule
## Via Size, Multiple Vias, Via Overlap and Autogenerate Vias
## Minumum Area Rule And Minimum Hole Rule
## Wells And Deep N-Well
## Derived Layers
## Paramterized And PDK Devices
## Angle Error And Overlap Rule
## Unimplemented Rules
## Latch-up And Antenna Rules
## Lab For Density Rules

------------------------------------------------------------------------------------------------

# #Day_29
  
**DRC/LVS Labs**

## Lecture

Reference Github : https://github.com/Devipriya1921/Physical-Verification-using-synopsys-40nm
	
**IC Validator**

Is a comprehensive and high-performance signoff solution that improves productivity for customers at all process nodes, from mature to advanced. It is a physical verification tool architected for massive and efficient distributed processing. ICV can run Design Rule Checks (DRC) which ensure the design meets manufacturing requirements and will not result in a chip failure. ICV can also run Layout Versus Schematic (LVS) which checking compares the extracted netlist from the layout to the original schematic netlist to determine if they match.

------------------------------------------------------------------------------------------------


-----**THE END**-----
