# Processor Project – Active-HDL Workspace

This repository hosts a fully functional multicycle datapath processor, implemented in Verilog to execute a subset of MIPS-style instructions across five distinct phases—fetch, decode, execute, memory access, and write-back—each coordinated by a centralized control unit. The design cleanly separates the ALU, register file, program counter, instruction memory, and data memory into modular components, making it easy to simulate and extend. Comprehensive testbenches accompany every module, ensuring cycle-accurate verification of individual units as well as the end-to-end processor. To explore the complete hierarchy, run simulations, and inspect waveforms, simply open the provided ProcessorProject.aws workspace file in Active-HDL—it will automatically load all source and testbench files into the project tree for instant access.
## Getting Started

1. **Open the workspace**  
   In Active-HDL, go to **File → Open Workspace…** and select:
   ```
   Arch2.aws
   ```

2. **Browse your files**  
   Once loaded, the workspace tree will display all design and testbench files:
   ```
   ControlUnit.v
   ControlUnitTB.v
   instructionMemory.v
   instructionMemoryTB.v
   pcModule.v
   pcModule_tb.v
   Processor.v
   ALU.v
   ALU_tb.v
   constants.v
   dataMemory.v
   dataMemory_tb.v
   registerFile.v
   registerFile_tb.v
   ClockGenerator.v
   ClockGenerator_tb.v
   ```

### Repository Structure

- **Arch2.aws**  
  The primary Active-HDL workspace file—open this in Active-HDL to load all of your Verilog modules and testbenches at once.

- **Arch2.wsw**  
  An alternative workspace file (WSW format) for compatibility with other HDL editors or legacy projects—loads the same set of files.

- **library.cfg**  
  Configuration file that maps library names to directories and sets up search paths for simulation and synthesis tools.

=
