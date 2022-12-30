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
+  [Day_11](https://github.com/Parvin16/sd_training#day_11) : ** **
   * [Lab](https://github.com/Parvin16/sd_training#labs-9)
+  [Day_12](https://github.com/Parvin16/sd_training#day_12) : ** **
   * [Lab](https://github.com/Parvin16/sd_training#labs-10)
 

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

## Optimizations Combinational Operations


## Sequential Optimizations


## Special Optimizations


## How Paths are Timed MCP ?


------------------------------------------------------------------------------------------------

## LABS

### LAB 1 - Combinational Optimizations

### LAB 2 - Resource Sharing Optimizations

### LAB 3 - Sequential Optimizations

### LAB 4 - Boundary Optimizations

### LAB 5 - Register Retiming

### LAB 6 - Isolating Output Ports

### LAB 7 - MultiCycle Path 

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

### LAB 2 - Check_timing , Check_design , Set_max_capacitance , HFN

------------------------------------------------------------------------------------------------


# #Day_11

## Lecture


------------------------------------------------------------------------------------------------

## LABS

### LAB 1 - 

### LAB 2 - 

------------------------------------------------------------------------------------------------


# #Day_12

## Lecture


------------------------------------------------------------------------------------------------

## LABS

### LAB 1 - 

### LAB 2 - 

------------------------------------------------------------------------------------------------


