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
## AUIPC Instruction
## Instruction: auipc gp, 0x13
> This instruction belongs to the U-type instruction set as it involves an immediate value for upper-immediate loading.
> 
 * Type: U-Type (Upper Immediate)
 * Label: None (it's a direct instruction without a label)
 * Details:
   * Opcode for AUIPC: 0110111
   * rd (gp): 3 (Register number for gp)
   * imm: 0x13 (20-bit immediate value)
32-bit Instruction Encoding:
 * Binary Representation:
   * 0110111 00000000 00000000 00000000 00010011
## ADDIW Instruction
## Instruction: addiw a5, a5, -1
> This instruction adds the immediate value (-1) to the 32-bit value in register a5 and stores the 32-bit result in register a5.
> 
 * Type: I-Type (Immediate)
 * Label: None (it's a direct instruction without a label)
 * Details:
   * Opcode for ADDIW: 0011011
   * funct3: 000 (for addiw)
   * rd (a5): 15 (Register number for a5)
   * rs1 (a5): 15 (Register number for a5)
   * imm: -1 (Immediate value, which is a 12-bit signed integer)
32-bit Instruction Encoding:
 * Binary Representation:
   0011011 000 15 15 1111111111111111
## JR Instruction
## Instruction: jr zero
> This instruction unconditionally jumps to the address stored in register zero.
> 
 * Type: R-Type (Register)
 * Label: None (it's a direct instruction without a label)
 * Details:
   * Opcode for JR: 0000000
   * rs1 (zero): 0 (Register number for zero)
   * rs2: 0 (Not used)
   * rd: 0 (Not used)
   * funct3: 000 (Not used)
   * funct7: 0010000 (for jr)
32-bit Instruction Encoding:
 * Binary Representation:
   0000000 00000 00000 00000 0010000
## JALR Instruction
## instruction: jalr a5 
> The jalr instruction belongs to the I-type instruction set in RISC-V architecture.
> 
 * Type: I-Type (Immediate)
 * Label: (Optional - can be assigned as needed)
 * Details:
   * Opcode: 1100111
   * rd: 00000 (No destination register specified)
   * funct3: 000
   * rs1 (a5): 00101 (Register number for a5)
   * rs2: 00000 (No second source register)
   * imm[11:0]: 000000000000 (Immediate field is not used)
32-bit Instruction Encoding:
 * Binary Representation:
   1100111 00000 000 00101 00000 000000000000
## BGEU Instruction
## Instruction: bgeu t1, a2, 10334
> This instruction belongs to the B-type instruction set as it's a branch instruction with an immediate offset.
> 
 * Type: B-Type (Branch)
 * Label: 10334 (This is the target address of the branch)
 * Breakpoint: Can be set at this instruction to pause program execution before the branch condition is evaluated.
 * Details:
   * Opcode for BGEU: 1100011
   * funct3: 111 (for bgeu)
   * rs1 (t1): 5 (Register number for t1)
   * rs2 (a2): 1 (Register number for a2)
   * imm: 10334 (13-bit signed immediate value representing the branch offset)
32-bit Instruction Encoding:
 * Binary Representation:
   * 1100011 00101000 00000001 111
##ADDI Instruction
### Instruction: addi a5, a5, -176
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
## SLLI Instruction
### Instruction: slli a3, a3, 0x20
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
  ## SB Instruction
### Instruction: sb a1, 14(a4)
> This instruction stores the byte from register a1 to the memory address calculated by adding the immediate value (14) to the value in register a4.
> 
 * Type: S-Type (Store)
 * Label: None (it's a direct instruction without a label)
 * Details:
   * Opcode for SB: 0100011
   * funct3: 000 (for sb)
   * rs1 (a4): 10 (Register number for a4)
   * rs2 (a1): 5 (Register number for a1)
   * imm[11:5]: 0000111 (Upper 7 bits of the immediate value, 14)
   * imm[4:0]: 00110 (Lower 5 bits of the immediate value, 14)
32-bit Instruction Encoding:
 * Binary Representation:
   0100011 000 10 5 0000111 00110
  ### ADD Instruction
### Instruction: add a3, a3, t0
> This instruction adds the values in registers a3 and t0 and stores the result in register a3.
> 
 * Type: R-Type (Register)
 * Label: None (it's a direct instruction without a label)
 * Details:
   * Opcode for ADD: 0000000
   * funct3: 000 (for add)
   * rd (a3): 9 (Register number for a3)
   * rs1 (a3): 9 (Register number for a3)
   * rs2 (t0): 5 (Register number for t0)
   * funct7: 0000000 (for add)
32-bit Instruction Encoding:
 * Binary Representation:
   0000000 9 000 9 5 0000000
### SUB Instruction
### Instruction: sub a3, t1, a2
> This instruction subtracts the value in register a2 from the value in register t1 and stores the result in register a3.
> 
 * Type: R-Type (Register)
 * Label: None (it's a direct instruction without a label)
 * Details:
   * Opcode for SUB: 0000000
   * funct3: 000 (for sub)
   * rd (a3): 9 (Register number for a3)
   * rs1 (t1): 5 (Register number for t1)
   * rs2 (a2): 6 (Register number for a2)
   * funct7: 0100000 (for sub)
32-bit Instruction Encoding:
 * Binary Representation:
   0000000 9 000 5 6 0100000
##   BNEZ Instruction
## Instruction: bnez a1, 10388
> This instruction branches to the specified offset (10388) if the value in register a1 is not equal to zero.
> 
 * Type: I-Type (Immediate)
 * Label: None (it's a direct instruction without a label)
 * Details:
   * Opcode for BNEZ: 0000011
   * rs1 (a1): 5 (Register number for a1)
   * imm: 10388 (Immediate value, which is a 12-bit signed integer)
32-bit Instruction Encoding:
 * Binary Representation:
   0000011 000 5 0000000 0011111111111111
   ## BLTU Instruction
## Instruction: bltu a4, a3, 1031c
> This instruction branches to the specified offset (1031c) if the unsigned value in register a4 is less than the unsigned value in register a3.
> 
 * Type: I-Type (Immediate)
 * Label: None (it's a direct instruction without a label)
 * Details:
   * Opcode for BLTU: 0001011
   * rs1 (a4): 10 (Register number for a4)
   * rs2 (a3): 9 (Register number for a3)
   * imm: 1031c (Immediate value, which is a 12-bit signed integer)
32-bit Instruction Encoding:
 * Binary Representation:
   0001011 000 10 9 1111111111111111
  ## MV Instruction
## Instruction: mv a4, a0
> This instruction moves the value from register a0 to register a4. It's essentially a simplified form of the add instruction where the second source register is the same as the destination register.
> 
 * Type: R-Type (Register)
 * Label: None (it's a direct instruction without a label)
 * Details:
   * Opcode for ADD: 0000000
   * funct3: 000 (for add)
   * rd (a4): 10 (Register number for a4)
   * rs1 (a0): 0 (Register number for a0)
   * rs2 (a0): 0 (Register number for a0)
   * funct7: 0000000 (for add)
32-bit Instruction Encoding:
 * Binary Representation:
   0000000 10 000 0 0 0000000
