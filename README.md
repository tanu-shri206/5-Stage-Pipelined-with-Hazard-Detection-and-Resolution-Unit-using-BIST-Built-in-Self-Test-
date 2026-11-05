# Design and Verification of a 5-Stage Pipelined Processor with Hazard Detection, Forwarding and Built-In Self-Test (BIST)

## 1. Project Overview

This project focuses on the design and verification of a **32-bit, 5-stage pipelined processor** using Verilog HDL.

The processor integrates a Hazard Detection Unit (HDU), a Forwarding Unit, and a Built-In Self-Test (BIST) mechanism. The objective is to improve data hazard handling, evaluate processor execution performance, and demonstrate fault detection through simulation.

The design follows a five-stage pipeline architecture: Instruction Fetch (IF), Instruction Decode (ID), Execute (EX), Memory Access (MEM), and Write Back (WB).

## 2. Processor Architecture

The processor consists of the following five pipeline stages:

| Pipeline Stage | Function |
|---|---|
| IF – Instruction Fetch | Fetches instructions from instruction memory |
| ID – Instruction Decode | Decodes instructions and reads register operands |
| EX – Execute | Performs arithmetic and logical operations |
| MEM – Memory Access | Handles data memory operations |
| WB – Write Back | Writes results back to the register file |

### Key Design Components

- **Hazard Detection Unit (HDU):** Integrated into the Instruction Decode stage to identify relevant hazard conditions.
- **Forwarding Unit:** Integrated into the Execute stage to forward data from pipeline registers and reduce data dependency delays.
- **BIST Mechanism:** Incorporated to support internal testing and fault-detection evaluation.

## 3. Key Features

- 32-bit processor datapath
- Five-stage pipelined architecture
- Hazard Detection Unit integration
- Data forwarding mechanism
- Built-In Self-Test (BIST) integration
- Modular Verilog HDL implementation
- Simulation-based functional verification
- Performance evaluation using execution cycles and CPI
- Fault-injection-based BIST evaluation

## 4. Performance Evaluation

The processor was evaluated using a test sequence containing six instructions.

| Performance Parameter | Without HDU | With HDU and Forwarding |
|---|---:|---:|
| Number of Instructions | 6 | 6 |
| Total Execution Cycles | 14 | 9 |
| CPI | 2.33 | 1.50 |

**Execution-cycle reduction: 35.71%**

The simulation results demonstrate improved execution efficiency for the evaluated instruction sequence after integrating hazard detection and forwarding.

*Note: These results correspond to the specific test sequence used in the project and should not be interpreted as a general performance improvement for every workload.*

## 5. Hazard Handling Evaluation

Three hazard conditions were considered in the reported evaluation.

| Configuration | Resolved Hazards | Unresolved Hazards |
|---|---:|---:|
| Without HDU | 0 | 3 |
| With HDU and Forwarding | 2 | 1 |

The results demonstrate improved hazard handling through the forwarding mechanism. Some hazard conditions remain unresolved in the implemented configuration.

## 6. Built-In Self-Test (BIST)

A Built-In Self-Test mechanism was integrated to evaluate the testability of the processor.

The BIST evaluation involved fault injection and simulation-based response analysis to examine whether injected errors could be detected.

The reported results show detection of all three injected errors in the evaluated test cases.

## 7. Tools and Technologies

| Category | Tools |
|---|---|
| Hardware Description Language | Verilog HDL |
| Design and Simulation | Xilinx Vivado, ModelSim |
| Waveform Analysis | GTKWave |
| Version Control | Git, GitHub |

## 8. Project Outcomes

- Designed and integrated a five-stage pipelined processor.
- Integrated hazard detection and data forwarding mechanisms.
- Evaluated processor performance using execution cycles and CPI.
- Implemented a BIST-based testing approach.
- Evaluated fault detection using simulation-based fault injection.
- Compared processor behavior under different hazard-handling configurations.

## 9. Future Scope

- Enhanced load-use hazard handling.
- Implementation of pipeline stalling and flushing.
- Improved control hazard handling.
- FPGA-based hardware implementation.
- Further processor performance optimization.

## 10. Project Status

**Completed – RTL Design, Integration and Simulation-Based Verification.**

