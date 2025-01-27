
# 32-bit MIPS Processor Implementation
This project implements a 32-bit MIPS processor in Verilog HDL targeting the Xilinx Zynq Zybo FPGA board.

## Architecture

![MIPS CPU Architecture](https://github.com/mo-faruque/MIPS_Processor/blob/main/docs/cpu_block.png)

- 32-bit pipelined processor
- Separate 32-bit instruction and 16-bit data memories (Harvard architecture) 
- 32 x 16-bit general purpose registers
- 32-bit program counter

## Instruction Set 

- R-type (Register-Register)
- I-type (Register-Immediate) 
- Arithmetic, logical, load/store, control
- 32-bit fixed length instructions

## Pipeline Stages

The processor has the following 5 pipeline stages:

- Fetch instruction (IF)
- Decode and execute instruction (ID/EX)
- Access memory (MEM) 
- Write back (WB)
- Update PC for next instruction (PC)

## Components

- Control Unit (Finite State Machine)
- Registers 
- ALU
- Instruction Memory
- Data Memory


## Simulation

The processor was simulated using testbenches to verify the functionality.
![Simulation Waveform](https://github.com/mo-faruque/MIPS_Processor/blob/main/docs/functional-verification/waveform_view.png)

## Synthesis

The processor RTL code was synthesized targeting the Xilinx Zynq Zybo FPGA board.
![RTL Schematic](https://github.com/mo-faruque/MIPS_Processor/blob/main/syn/RTL_Schematic.png)

## Repository Structure

- `rtl/` - Contains Verilog code for the processor 
- `tb/` - Testbenches for simulation
- `syn/` - Synthesis scripts 
- `docs/` - Documentation (architecture, verification plan etc.)


## Documentation

- [Spec document](https://github.com/mo-faruque/MIPS_Processor/blob/main/docs/MIPS_Project_Description.pdf) - Architecture and implementation details
- [Verification plan](https://github.com/mo-faruque/MIPS_Processor/blob/main/docs/functional-verification/mips_functional_verification.pdf) - Testcases and results
- [FPGA Resources](https://github.com/mo-faruque/MIPS_Processor/blob/main/syn/Detailed%20RTL%20Component%20Info.pdf) - Testcases and results

<!--
## Author

John Doe

[github.com/john-doe](https://github.com/john-doe)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


-->


 


