# samsung-riscv[WhatsApp Image 2025-01-02 at 21 17 53_4e6f2e67](https://github.com/user-attachments/assets/ca80bee8-0896-47c9-a920-24fbcb4329bf)
![image](https://github.com/user-attachments/assets/4d9f8f5d-b69a-469b-ba9d-2fdc0636d2d1)
![image](https://github.com/user-attachments/assets/60241635-8fd1-4ce8-923f-a8a88573dc23)
![image](https://github.com/user-attachments/assets/47e4a7ab-1922-4479-82ed-d72b0d9883f5)
##task2:
![Screenshot 2025-01-13 164834](https://github.com/user-attachments/assets/806db8ed-297b-4db4-88d1-3bfda808efbc)
![Screenshot 2025-01-13 164056](https://github.com/user-attachments/assets/d78491e5-bcba-4edf-814b-45708d4c8cb0)
![Screenshot 2025-01-13 163947](https://github.com/user-attachments/assets/8a60cafb-573e-44d4-80b1-dca8aa052a2c)
![Screenshot 2025-01-13 162757](https://github.com/user-attachments/assets/c59f2448-8407-431a-86ad-19c839be29aa)
![WhatsApp Image 2025-01-17 at 18 37 13_5cb638d3](https://github.com/user-attachments/assets/c68f7779-5bcb-4ee3-895b-3046a4213ab6)
![WhatsApp Image 2025-01-17 at 18 37 50_949fed92](https://github.com/user-attachments/assets/151cc39f-6d5a-4eb3-862b-cf2a5c27fbda)
![WhatsApp Image 2025-01-17 at 18 38 24_6b2319ed](https://github.com/user-attachments/assets/6ed6ac82-df3a-495c-9bb3-29fa3cf5bcb1)
## ADDI Instruction

### Instruction: `addi a5, a5, -176`

> All the arithmetic and logical operations are performed using *I-type instruction format*, hence this instruction belongs to the I-type instruction set.

- **Type:** I-Type (Immediate)
- **Label:** None (it's a direct instruction without a label)

- **Details:**
  - **Opcode for ADDI:** 0010011
  - **funct3:** 000 (for addi)
  - **rd (a5):** 15 (Register number for a5)
  - **rs1 (a5):** 15 (Register number for a5)
  - **imm:** -176 (Immediate value, which is a 12-bit signed integer)

### 32-bit Instruction Encoding:

- **Binary Representation:**1110 1000 0000 01111 000 01111 0010011
- 
---

## JAL Instruction

### Instruction: `jal ra, 10264`

> The `jal` (Jump and Link) instruction is used for control flow and belongs to the *J-type* instruction set.

- **Type:** J-Type (Jump)
- **Label:** None (it's a direct instruction without a label)

- **Details:**
- **Opcode for JAL:** 1101111
- **rd (ra):** 1 (Register number for ra)
- **imm:** 10264 (Immediate value, which is a 20-bit signed integer)

### 32-bit Instruction Encoding:

- **Binary Representation:**00000110010100000000 | 00001| 1101111
## LUI Instruction

### Instruction: `lui a0, 0×2b`

> The `lui` (Load Upper Immediate) instruction is used to load a 20-bit immediate value into the upper 20 bits of a register and belongs to the *U-type* instruction set.

- **Type:** U-Type (Upper Immediate)
- **Label:** None (it's a direct instruction without a label)

- **Details:**
  - **Opcode for LUI:** 0110111
  - **funct3:** 000 (for lui)
  - **rd (a0):** 10 (Register number for a0)
  - **imm:** 0x2b000 (Immediate value, shifted left by 12 bits to occupy the upper 20 bits)

### 32-bit Instruction Encoding:

- **Binary Representation:**101010110000 | 01010| 0110111
##  LW Instruction
### Instruction:lw a3, 12(sp)

-**Type:** I-Type (Immediate)

-**Label:** None (it's a direct instruction without a label)

**Details:**

**Opcode for LW:** 0000011 (binary for opcode 0x23)
**funct3:** 010 (for lw)
**rd (a3):** 11 (Register number for $a3)
**rs1 (sp):** 29 (Register number for $sp)
**imm:** 12 (Immediate offset, a 12-bit signed integer)

### 32-bit Instruction Encoding:
Binary Representation: 
0000011 11101 01011 010 00000 000000001100
## AUIPC instruction
### Instruction:auipc a5, 0xffff0

**Type:** U-Type (Upper Immediate)

**Label:** None (it's a direct instruction without a label)

**Details:**

**Opcode for AUIPC:** 0010111
**rd (a5):** 15 (Register number for a5 in RISC-V)
**imm:** 0xffff0 (Immediate value, which is a 20-bit unsigned integer)

### 32-bit Instruction Encoding:
Binary Representation:
0010111 00000 01111 1111111111110000
### Instruction:auipc gp, 0x13

**Type:** U-Type (Upper Immediate)

**Label:** None (it's a direct instruction without a label)

**Details:**

**Opcode for AUIPC:** 0110111
**rd (gp):** 28 (Register number for GP, which corresponds to x28)
**imm:** 0x13 (The 20-bit immediate value to be added to the PC)

32-bit Instruction Encoding:
### Binary Representation:
0000000000010011 11100 0110111
## LW Instruction
### Instruction:lw a5, 1944(gp)

**Type:** I-Type (Immediate)

**Label:** None (it's a direct instruction without a label)

**Details:**

**Opcode for LW:** 0000011
**funct3:** 010 (for lw operation)
**rd (a5):** 15 (Register number for a5)
**rs1 (gp):** 28 (Register number for gp)
**imm:** 1944 (Immediate value, which is a 12-bit signed integer)
32-bit Instruction Encoding:
### Binary Representation:
0000011111001000 11100  010  01101 0000011
### Instruction:auipc a0, 0x0

**Type:** U-Type (Upper Immediate)

**Label:** None (it's a direct instruction without a label)

**Details:**

**Opcode for AUIPC:** 0111011
**rd (a0):** 10 (Register number for a0)
**imm:** 0x0 (Immediate value, which is a 20-bit unsigned integer)

32-bit Instruction Encoding:
### Binary Representation:
00000000000000000000 01010 0111011
ADDI Instruction
Instruction: addi a5, a5, -176
> All the arithmetic and logical operations are performed using I-type instruction format, hence this instruction belongs to the I-type instruction set.
> 
 * Type: I-Type (Immediate)
 * Label: None (it's a direct instruction without a label)
 * Details:
   * Opcode for ADDI: 0010011
   * funct3: 000 (for addi)
   * rd (a5): 15 (Register number for a5)
   * rs1 (a5): 15 (Register number for a5)
   * imm: -176 (Immediate value, which is a 12-bit signed integer)
32-bit Instruction Encoding:
 * Binary Representation:
   0010011 000 15 15 10101000
SLLI Instruction
Instruction: slli a3, a3, 0x20
> This instruction performs a logical left shift on the value in register a3 and stores the result in register a3.
> 
 * Type: R-Type (Register)
 * Label: None (it's a direct instruction without a label)
 * Details:
   * Opcode for SLLI: 0000000
   * funct3: 001 (for slli)
   * rd (a3): 9 (Register number for a3)
   * rs1 (a3): 9 (Register number for a3)
   * rs2: 0 (Not used in SLLI)
   * funct7: 0000000 (for slli)
   * shamt: 0x20 (Shift amount)
32-bit Instruction Encoding:
 * Binary Representation:
   0000000 9 000 9 0000000 0x20
