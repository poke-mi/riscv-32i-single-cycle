# riscv-32i-single-cycle
## Overview
A hardware implementation of a 32-bit single-cycle processor core based on the RISC-V RV32I base integer instruction set architecture (ISA). Developed entirely in Verilog, this project demonstrates foundational RTL design, custom data path routing, memory interfacing, and instruction decoding for modern ASIC architectures.

## Architecture Highlights
* **Core Design:** Single-cycle execution architecture.
* **Datapath:** Custom 32-bit routing integrating the ALU, Program Counter (PC), Register File, and Control Unit.
* **Memory:** Distinct instruction and data memory interfaces (Harvard architecture).

## Supported Instruction Set (RV32I Base)
* **Arithmetic & Logical:** `ADD`, `SUB`, `AND`, `OR`, `XOR`, `SLL`, `SRL`, `SRA`, `ADDI`, `ANDI`, `ORI`, `XORI`
* **Memory Operations:** `LW` (Load Word), `SW` (Store Word)
* **Control Flow:** `BEQ`, `BNE`, `BLT`, `BGE`, `JAL`, `JALR`

## Directory Structure
* `src/` — Verilog source code for core logic (ALU, Register File, Control Unit, Top-level Datapath).
* `tb/` — Self-checking Verilog testbenches for module-level and system-level verification.
* `docs/` — Datapath schematics, block diagrams, and ISA reference materials.
* `asm/` — Sample RISC-V assembly programs and compiled hex files for simulation testing.

## Project Milestones
- [x] Design and verify the Arithmetic Logic Unit (ALU).
- [ ] Implement the 32x32-bit Register File (Sequential Logic).
- [ ] Construct the Instruction and Data Memory modules.
- [ ] Develop the Control Unit (Instruction decoding and signal generation).
- [ ] Top-level structural instantiation and data path routing.
- [ ] Full system simulation executing a custom RISC-V assembly program.

## Toolchain & Verification
**Hardware Description Language:** Verilog (IEEE 1364-2005)
**Compiler/Simulator:** Icarus Verilog (`iverilog`)
**Waveform Viewer:** GTKWave
