# Multicycle-RISC-processor-Design

This project implements a simple 16-bit multi-cycle RISC processor designed in Verilog. It was developed for educational purposes to demonstrate instruction processing using a multi-cycle architecture.

## Features

- **Architecture:** 16-bit instruction and data width with byte-addressable memory  
- **Registers:** 8 General-Purpose Registers (R0–R7), with R0 hardwired to zero  
- **Execution:** Multi-cycle instruction execution (Fetch, Decode, Execute, Memory, Write-back)  
- **Instruction Set:** Supports R-Type, I-Type, J-Type, and S-Type instructions  
- **ALU:** Performs arithmetic, logic, and comparison operations (with condition flags)  
- **Memory:** Separate Instruction and Data memory (Little Endian format)  
- **Simulation:** Built and tested using [EDA Playground](https://www.edaplayground.com/)  

## Instruction Set

- **R-Type:** `AND`, `ADD`, `SUB`  
- **I-Type:** `ADDI`, `ANDI`, `LW`, `SW`, Branch instructions (`BGT`, `BEQ`, etc.)  
- **J-Type:** `JMP`, `CALL`, `RET`  
- **S-Type:** Store-type instructions  

## Design Summary

- **Multi-Cycle Design:**  
  Each instruction is executed over several clock cycles, broken down into:
  - Instruction Fetch
  - Instruction Decode
  - Execution
  - Memory Access
  - Write-back

- **Control Path:**  
  Control signals are dynamically generated per cycle to guide instruction flow.

- **Testing:**  
  Individual components were verified before full system integration. Sample programs were executed to validate functionality and branching logic.

## Tools Used

- **Language:** Verilog  
- **Simulation Platform:** EDA Playground   

## Conclusion

This processor was successfully built and verified using a custom instruction set. It demonstrates the fundamentals of instruction decoding, memory operations, and ALU logic in a multi-cycle RISC architecture. The design is modular and extensible, serving as a foundation for further architectural exploration or pipelining enhancements.



