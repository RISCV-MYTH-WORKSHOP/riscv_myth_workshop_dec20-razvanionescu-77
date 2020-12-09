## How to use it
The code is implementing a complete RISC-V core. It has now an optimized stage for decoder (Decoder is moved in a separate stage), implements jumps, register bypass and it finishes 
executing the code in 60 cycles. Look at cycle 57 when sum of numbers from 1 to 9 is ready (45) and then in cycle 58 it is copied in Data Memory. In cycle 60, result is loaded back from memory in register r17.

![alt text](https://github.com/RISCV-MYTH-WORKSHOP/riscv_myth_workshop_dec20-razvanionescu-77/blob/master/16_RV_Complete_RISC-V/RV_Complete_RISC-V_Diagram.PNG "Diagram")
![alt text](https://github.com/RISCV-MYTH-WORKSHOP/riscv_myth_workshop_dec20-razvanionescu-77/blob/master/16_RV_Complete_RISC-V/RV_Complete_RISC-V_Viz.PNG "Viz")
![alt text](https://github.com/RISCV-MYTH-WORKSHOP/riscv_myth_workshop_dec20-razvanionescu-77/blob/master/16_RV_Complete_RISC-V/RV_Complete_RISC-V_Waveform.PNG "Waveform")
