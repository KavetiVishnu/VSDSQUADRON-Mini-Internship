# RISC-V Architecture   
 * RISC-V is an open-standard, Reduced Instruction Set Computing (RISC) architecture designed for simplicity, modularity, and scalability.        
 * It provides a streamlined and extensible instruction set, making it highly efficient for a wide range of applications, from embedded systems to high-performance computing.     
 * Its load-store architecture, optimized instruction set, and support for various extensions (e.g., integer, floating-point, vector processing) make it a powerful choice for diverse computing needs.   
## RISC-V Instruction Formats        
The RISC-V Instruction Set Architecture (ISA) defines six standard instruction formats, each designed to support different types of operations efficiently.       
  
**1. R-Type** – Register-Register operations   
**2. I-Type** – Immediate operations  
**3. S-Type** – Store operations  
**4. B-Type** – Branch operations  
**5. U-Type** – Upper Immediate operations  
**6. J-Type** – Jump operations     

   <img width="616" alt="image" src="https://github.com/user-attachments/assets/2ae752f3-a817-41c5-b5c5-563c1771fc1b" />    

   


## _1. R-Type (Register-Register)_   
_**Functionality:**_  Used for arithmetic and logical operations that involve two source registers and one destination register.  
_**Example:**_  add x5, x1, x2 ; x5 = x1 + x2
  
## _2. I-Type (Immediate)_
_**Functionality:**_ Used for operations that require an immediate value, including arithmetic, logical, load, and control-flow instructions.   
_**Example:**_ addi x5, x1, 10  ; x5 = x1 + 10

## _3. S-Type (Store)_
_**Functionality:**_ Handles store instructions, where data from a register is written to memory.   
_**Example:**_ sw x5, 20(x1)  ; Store word from x5 to memory address (x1 + 20)   

## _4. B-Type (Branch)_
_**Functionality:**_ Used for conditional branching based on register comparisons.     
_**Example:**_ beq x1, x2, 16  ; If x1 == x2, branch to PC + 16     

## _5. U-Type (Upper Immediate)_
_**Functionality:**_ Used for loading large immediate values into registers.     
_**Example:**_ lui x5, 0x12345  ; Load upper immediate 0x12345000 into x5   

## _6. J-Type (Jump)_
_**Functionality:**_ Used for jump and link operations, commonly for function calls and control flow changes.     
_**Example:**_ jal x1, 100  ; Jump to PC + 100 and store return address in x1      


## 1. addi sp, sp, -32   
   
```
Type = I-type instruction
imm[11:0] = 1111111111110000 (2's complement of -32)
rs1 = 00010 (sp register, register 2)
funct3 = 000 (addition operation)
rd = 00010 (sp register, register 2)
opcode = 0010011 (for addi instruction)
```

#32-bit Instruction:   
![image](https://github.com/user-attachments/assets/5884e2e5-8b7c-4c95-80be-740e58d752f5)


## 2. sd ra, 24(sp)  
```
Type = I-type Format (for Store Doubleword (sd) instruction)  
imm[11:0] = 0000000000011000 (24 in binary)
rs2 = 00001 (ra register)
rs1 = 00010 (sp register)
funct3 = 011
opcode = 0100011 (for store instructions)
```
#32-bit Instruction:    
![image](https://github.com/user-attachments/assets/bea25d1c-05f5-448d-83b0-e1986f5ca0db)

## 3. sw zero, -20(s0) 
```
Type = I-type Format (for Store Word (sw) instruction)
imm[11:0] = 1111111111111100 (in two's complement for -20).
rs2 = 00000 (zero register).
rs1 = 01000 (s0 register).
funct3 = 010 (for sw).
opcode = 0100011 (store instruction opcode)
```
#32-bit Instruction:   
![image](https://github.com/user-attachments/assets/5e908fcd-3d63-45bd-a1ae-5240e91315e7)

## 4. li a5, 10 
```
The instruction li a5, 10 is a Load Immediate instruction in RISC-V, which loads the immediate value 10 into the register a5 (which is register 17 in RISC-V). Since RISC-V doesn’t have a direct li (Load Immediate) instruction, it is typically implemented using the LUI (Load Upper Immediate) and ADDI (Add Immediate) instructions to load larger immediate values. But for the immediate value 10, we can directly use the ADDI instruction.  

Instruction:
li a5, 10 can be broken down as:
addi a5, x0, 10
  
a5 = register 17 → 10001
x0 = register 0 (the zero register, which always contains 0) → 00000
Immediate = 10 → 000000000001010 (10 in binary)
funct3 = 000 (for addition operation)
opcode = 0010011 (for addi instruction)

addi a5, x0, 10:       
imm[11:0] = 000000000001010 (10 in binary)
rs1 = 00000 (x0 register)
funct3 = 000
rd = 10001 (a5 register)
opcode = 0010011 (addi instruction)
```
#32-bit Instruction:  
![image](https://github.com/user-attachments/assets/bee90f94-4a9e-400c-83dc-091a4427984e)   


## 5. lw a4, -20(s0)   
```
Type = Load Word (lw)
imm[11:0] = 1111111111111100 (in two's complement for -20).
rs1 = 01000 (s0 register).
funct3 = 010 (for lw).
rd = 01010 (a4 register).
opcode = 0000011 (for load word instruction).
```
#32-bit Instruction:    
![image](https://github.com/user-attachments/assets/12f42dbe-3647-4db2-97f3-b6dab88c2b72)

















