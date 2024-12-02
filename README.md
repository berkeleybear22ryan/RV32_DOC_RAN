# RV32 Instruction Set Documentation

Welcome to the RV32 Instruction Set Documentation, created by **Ryan Allyn Nader**. This repository contains a detailed breakdown of RV32 instructions, complete with formats, examples, and explanations.

## Table of Contents

- [Introduction](#introduction)
- [Instruction Categories](#instruction-categories)
- [Pseudo Instructions](#pseudo-instructions)
- [Arithmetic Core](#arithmetic-core)
- [Directives](#directives)
- [Usage Example](#usage-example)

---

## Introduction

This documentation serves as a comprehensive guide to the RV32 instruction set. It is tailored for students, developers, and enthusiasts looking to understand the fundamentals of RISC-V assembly programming. Each instruction includes:

1. **Format**: The encoding type (R, I, S, U, SB, UJ).
2. **Description**: A detailed explanation of the operation.
3. **Example**: Sample usage with code snippets.
4. **Shorthand**: Simplified logical expression or equivalence (if applicable).

---

## Instruction Categories

### RV32I Base Instructions

The base integer instruction set for RV32 includes essential operations:
- **Arithmetic**: `add`, `addi`, `sub`, `mul`, etc.
- **Logical**: `and`, `or`, `xor`, `sll`, `srl`, etc.
- **Memory**: `lw`, `lb`, `sw`, `sb`, etc.
- **Branching**: `beq`, `bne`, `blt`, `bge`, etc.
- **Control Flow**: `jal`, `jalr`, `ecall`, `ebreak`.

### RV32I Pseudo Instructions

Pseudo-instructions simplify common operations:
- `li` (load immediate)
- `mv` (move)
- `neg` (negate)
- `j` (jump)
- `nop` (no operation)

### RV32M Multiply Extension

Advanced arithmetic operations:
- `mul` (multiply)
- `div` (divide)
- `rem` (remainder)
- Unsigned counterparts: `divu`, `remu`.

---

## Directives

Directives provide metadata and organizational instructions:
- `.globl` - Declare global symbols.
- `.data` - Define data sections.
- `.text` - Define text (code) sections.
- `.align` - Align data or instructions.

---

## Usage Example

### Sample Instruction: `add`

**Format**: R-Type  
**Description**: Adds values from `rs1` and `rs2`, storing the result in `rd`.  
**Example**:

```assembly
li t0, 8      # Load 8 into register t0
li t1, 10     # Load 10 into register t1
add t2, t0, t1 # t2 = t0 + t1 -> t2 = 18
```

**Explanation**:  
This code initializes registers `t0` and `t1` with values 8 and 10, respectively. The `add` instruction adds these two registers and stores the result (18) in `t2`.

---

For more details on each instruction, please refer to the full HTML documentation. This README complements the structured content, guiding users to the specific areas of interest.