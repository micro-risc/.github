# Micro-RISC (μRISC)
 
μRISC is a small, load-store, RISC instruction set architecture,
built with a strict rule: every instruction decodes to exactly one micro-op.
No fused link-and-jump, no auto-increment/decrement addressing. If it can't
be one write, register or memory, it's not one instruction, with the sole
exception of atomic operations.
 
It's a flagged architecture (N/Z/C/V), with a 16-bit instruction
format for common operations and a 32-bit format for everything else
(wider immediates, 3-operand arithmetic, less common instructions).
 
This is a personal project, still early. Things will change.
 
## Repositories
 
- **[micro-risc-spec](https://github.com/micro-risc/micro-risc-spec)**
  the ISA specification.
- **[micro-risc-cores](https://github.com/micro-risc/micro-risc-cores)**
  hardware implementations, one subdirectory per core.
- **[micro-risc-toolchain](https://github.com/micro-risc/micro-risc-toolchain)**
  assembler and QBE Backend.
