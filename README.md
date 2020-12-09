# A RISC-V core micro-architecture to implement RV32I Base Instruction Set

[![](https://img.shields.io/badge/-RISC--V-red "RISC-V")](https://riscv.org/) [![](https://img.shields.io/badge/-TL--Verilog-blue "TL-Verilog")](https://tl-x.org/)
### Table of Contents  
[Introduction](#introduction)  
[Technologies](#technologies)  
[Examples of use](#examples)  
[Acknowledgements](#acknowledgements)


## Introduction
This project was developed during the RISC-V based MYTH (Microprocessor for You in Thirty Hours) [workshop](https://www.vlsisystemdesign.com/riscv-based-myth/). In order to create yourself a microarchitecture that implements RISC-V ISA (Instruction Set Architecture), one needs to understand stages required to go from ISA to physical design of the core. The workshop cover the following stages: understanding RISC-V RV64I ISA (Base Integer Instructions), understanding ABI (Application Binary Interface - like a contract between application and hardware to establish communication), concept of memory allocation, number representation (e.g., negative numbers), build tools (compiler, linker, assembler), simulator(e.g., spike), digital logic (using TL-Verilog), coding a RISC-V CPU subset, pipelining. Digital logic is covered in days 3-5 of the workshop and covers logic gates, combinational logic, sequential logic, pipelined logic and states.
## Technologies
#### VSD-IAT
The workshop uses a very nice and practical platform called [VSD-IAT(Intelligent Assessment Technology)](https://vsdiat.jnaapti.io/). As participant, you have access to videos, to follow the course at your own pace, have access to online labs, where you can practice with RISC-V tools (build tools, simulator) and also take some queries that grade your knowledge before and after following each part of the course.
#### Makerchip
Another amazing cloud based software used during the workshop (during days 3-5) is [Makerchip](http://makerchip.com/). An easy to use platform, with a lot of online resources (e.g., tutorials, examples) for learning digital design. The participants learn TL-Verilog and has a great combo of views to help them develop and debug their own design/code. There is an editor view for coding in TL-Verilog, another view to explore the generated code in SV(System Verilog) and expanded macros. There is also a Log view, where you can track if your code is compiling, if it passes simulation (based on Verilator), what are the errors , etc. To see your design at work, there are 3 more views: Diagram is showing your design (it is interactive, you can actually hoover the mouse pointer and see expressions), Waveform is showing all the signals (and can perform low level debugging) and Viz - visualization (you can actually try your code in a real life application, e.g., calculator or simulating execution of a program, see your registers, memory, program execution, etc). Check below few screenshots from Makerchip:
##### `Decoder` in Editor view
![alt text](https://github.com/RISCV-MYTH-WORKSHOP/riscv_myth_workshop_dec20-razvanionescu-77/blob/master/images/Decoder_Code_Makerchip.PNG "Decoder")
##### `NAV-TL` in Explorer view
![alt text](https://github.com/RISCV-MYTH-WORKSHOP/riscv_myth_workshop_dec20-razvanionescu-77/blob/master/images/NAV_TLV_Makerchip.PNG "Explorer")
##### `Log`
![alt text](https://github.com/RISCV-MYTH-WORKSHOP/riscv_myth_workshop_dec20-razvanionescu-77/blob/master/images/Log_Makerchip.PNG "Log")
##### `Diagram`
![alt text](https://github.com/RISCV-MYTH-WORKSHOP/riscv_myth_workshop_dec20-razvanionescu-77/blob/master/images/Diagram_Makerchip.PNG "Diagram")
##### `Waveform`
![alt text](https://github.com/RISCV-MYTH-WORKSHOP/riscv_myth_workshop_dec20-razvanionescu-77/blob/master/images/Waveform_Makerchip.PNG "Waveform")
##### `Viz`
![alt text](https://github.com/RISCV-MYTH-WORKSHOP/riscv_myth_workshop_dec20-razvanionescu-77/blob/master/images/Viz_Simulation_Makerchip.PNG "Visualization")
#### GitHub
GitHub is used for source code versioning. Each participant has is own repository where commits work for each assignment. There is public [repo](https://github.com/stevehoover/RISC-V_MYTH_Workshop) used during the workshop as reference design, also containing steps how to start development.
#### Slack
During the workshop, you can always get help from teachers/instructors online via [Slack](risc-vmythworkshop.slack.com) channels or during 1h daily call. Very nice and good interaction between participants and instructors. You can also can see the progress of other folks and ask for guidance or opinion of your design. 
## Examples of use
There were added folders for each assignments, covering days 3, 4 and 5 of the workshop. Each folder contains the tlv code with implementation for microarchitecture and a readme file. To try it, go to [Makerchip](http://makerchip.com/) website and copy-paste the code from example in online editor. From contextual menu (upper-right in editor view) choose Compile and Simulate (`Ctrl-Enter`). You will see in right side of the screen the Diagram generated and you can inspect Waveform and where applicable Viz views for more details.

The folders Day2 and Day3_5 contains the original code developed during the workshop, with many versions corresponding to each assignments.
## Acknowledgements
- [Kunal Ghosh](https://www.linkedin.com/in/kunal-ghosh-vlsisystemdesign-com-28084836/) (Founder VSD)
- [Steve Hoover](https://www.linkedin.com/in/steve-hoover-a44b607/) (Founder Redwood EDA)
- [Shivam Potdar](https://www.linkedin.com/in/shivampotdar99/)
- [Vineeth Jain](https://www.linkedin.com/in/vineet-jain-3b4a24150/)
