# RISC-V Processor Implementation in Verilog

## Overview
This project implements a **RISC-V processor** in Verilog, supporting both **sequential and pipelined** execution. It includes full **hazard detection and handling**, ensuring correct instruction execution through techniques like **data forwarding and pipeline stalls**.

## Features
- **Sequential and Pipelined Implementations**: Compare and analyze performance differences.
- **Hazard Handling**: Implements data hazards, control hazards, and structural hazard mitigation.
- **RISC-V Instruction Set**: Supports essential RISC-V instructions.
- **Optimized Performance**: Efficient pipeline execution with hazard resolution.

## Implementation Details
- **Sequential Processor**: Executes one instruction at a time.
- **Pipelined Processor**: Implements classic RISC-V pipeline stages:
  - Instruction Fetch (IF)
  - Instruction Decode (ID)
  - Execute (EX)
  - Memory Access (MEM)
  - Write Back (WB)
- **Hazard Handling**:
  - **Data Forwarding**: Reduces stalls caused by data dependencies.
  - **Pipeline Stalls**: Introduced where forwarding is insufficient.
  - **Branch Prediction**: Optimized control hazard resolution.

## Setup & Simulation
### Prerequisites:
- Verilog Simulation Tool (e.g., ModelSim, Vivado, Icarus Verilog)
- RISC-V Assembly/Test Programs

### Running the Simulation:
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/riscv-processor.git
   cd riscv-processor
