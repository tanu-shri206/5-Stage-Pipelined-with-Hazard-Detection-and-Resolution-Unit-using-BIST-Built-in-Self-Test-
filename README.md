# Design and Verification of a Performance-Enhanced Hazard Detection and Resolution Unit with BIST in a Pipelined Processor

## Project Overview

This project focuses on the design and verification of a performance-enhanced Hazard Detection and Resolution Unit (HDU) integrated within a 5-stage pipelined processor architecture. The processor improves execution efficiency by reducing hazards that occur during instruction processing. 

To further improve reliability and testability, a Built-In Self-Test (BIST) mechanism is incorporated into the design. The complete system is implemented using Verilog HDL and verified using simulation tools.

---

## Processor Architecture

The processor follows a standard 5-stage pipeline:

1. Instruction Fetch (IF)
2. Instruction Decode (ID)
3. Execute (EX)
4. Memory Access (MEM)
5. Write Back (WB)

---

## Project Features

- 5-stage pipelined processor design
- Hazard Detection Unit (HDU)
- Forwarding Unit for data hazard handling
- Pipeline stall mechanism
- Control hazard handling
- Built-In Self-Test (BIST)
- LFSR-based test pattern generation
- MISR-based output signature analysis
- Modular Verilog HDL implementation
- Functional verification through testbenches

---

## Modules Implemented

### Core Processor Modules
- 32-bit ALU
- Register File
- Program Counter (PC)
- Instruction Memory
- Data Memory
- Control Unit
- Pipeline Registers

### Hazard Handling Modules
- Hazard Detection Unit
- Forwarding Unit
- Stall Logic

### BIST Modules
- LFSR (Linear Feedback Shift Register)
- MISR (Multiple Input Signature Register)
- BIST Controller

---

## Tools and Technologies Used

- Verilog HDL
- Xilinx Vivado
- ModelSim
- GTKWave 
- GitHub

---

## Verification Methodology

The design is verified using:

- Directed test cases
- Functional verification
- Simulation waveforms
- Hazard condition testing
- BIST validation

---

## Performance Parameters

The following parameters are considered for performance analysis:

- Cycles Per Instruction (CPI)
- Pipeline stall count
- Forwarding efficiency
- Branch prediction accuracy
- Hazard resolution efficiency

---

## Future Scope

- FPGA implementation
- Advanced branch prediction techniques
- Out-of-order execution
- Power optimization methods
- Superscalar architecture extension

---

## Project Status

Current Progress:

✔ ALU design  
✔ Register File design  
✔ Program Counter design  
✔ Instruction Memory design  
- Pipeline implementation in progress  
- Hazard Detection Unit integration  
- BIST integration and verification  

---

## Team members

Tanushri Lute and Team
