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

Final 32-bit Instruction (I-type):11111111111100000010000000100011
In hexadecimal:0xFF5FF06B
```





























