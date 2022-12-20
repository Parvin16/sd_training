# #MY_REPO

## Table Of Content

+  [Day_0](https://github.com/Parvin16/sd_training/blob/main/readme.md#day-0) : **System/Tool Setup Check. GitHub ID creation**
   * [Lab](https://github.com/Parvin16/sd_training#lab-result)
+  [Day_1](https://github.com/Parvin16/sd_training/blob/main/readme.md#day-1) - **Introduction to Verilog RTL Design and Synthesis**
   * [Lab](https://github.com/Parvin16/sd_training#labs)
+  [Day_2](https://github.com/Parvin16/sd_training/blob/main/readme.md#day-2) : **Timing libs(QTMs/ETMs), Hierarchical vs Flat Synthesis and Efficient Flop Coding Styles**
   * [Lab](https://github.com/Parvin16/sd_training#labs-1)
+  [Day_3](https://github.com/Parvin16/sd_training/blob/main/readme.md#day-3) - **Combinational and Sequential Optimizations**
   * [Lab](https://github.com/Parvin16/sd_training#labs-2)
+ [Day_4](https://github.com/Parvin16/sd_training/blob/main/readme.md#day-4) : **GLS, Blocking vs Non-blocking and Synthesis-Simulation mismatch**
   * [Lab](https://github.com/Parvin16/sd_training#labs-3)
+  [Day_5](https://github.com/Parvin16/sd_training#day_5) - **DFT**
+  [Day_6](https://github.com/Parvin16/sd_training#day_6) : **Introduction to Logic Synthesis**
   * [Lab](https://github.com/Parvin16/sd_training#labs-4)
+  [Day_7](https://github.com/Parvin16/sd_training#day_7) : **Basic SDC Constraints**
   * [Lab](https://github.com/Parvin16/sd_training#labs-5)
+  [Day_8](https://github.com/Parvin16/sd_training#day_8) : **Advanced SDC Constraints**
   * [Lab](https://github.com/Parvin16/sd_training#labs-6)
+  [Day_9](https://github.com/Parvin16/sd_training#day_9) : **Optimization in Synthesis**
   * [Lab](https://github.com/Parvin16/sd_training#labs-7)
+  [Day_10](https://github.com/Parvin16/sd_training#day_10) : **QOR**
   * [Lab](https://github.com/Parvin16/sd_training#labs-8)

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

**Controllability** - from DFT point of view, we intend if both '0' and '1' are able to _propagate_  to each and every node within the target patterns. A point is said to be controllable if both '0' and '1' can be propogated through scan patterns. 

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


### What are constraints ??


### Inp Trans Output Load 


------------------------------------------------------------------------------------------------

### LABS

**LAB 1 - Timing dot Libs**

We gonna go through the dot Lib and understand the informations. cd ...//DC_WORKSHOP/lib ,

**LAB 2 - Exploring dot Lib Part1**


**LAB 3 - Exploring dot Lib Part2**


--------------------------------------------------------------------------------------------------

# #Day_8

### Theory


------------------------------------------------------------------------------------------------

### LABS

**LAB 1 - **

**LAB 2 - **

**LAB 3 - **

**LAB 4 - **

**LAB 5 - **

**LAB 6 - **

**LAB 7 - **

**LAB 8 - **

--------------------------------------------------------------------------------------------------

# #Day_9

### Theory


------------------------------------------------------------------------------------------------

### LABS

**LAB 1 - **

**LAB 2 - **

**LAB 3 - **

**LAB 4 - **

**LAB 5 - **

**LAB 6 - **

**LAB 7 - **

--------------------------------------------------------------------------------------------------

# #Day_10

### Theory


------------------------------------------------------------------------------------------------

### LABS

**LAB 1 - **


**LAB 2 - **


------------------------------------------------------------------------------------------------
