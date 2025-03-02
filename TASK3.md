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
_**Format:**_

| funct7 (7 bits) | rs2 (5 bits) | rs1 (5 bits) | funct3 (3 bits) | rd (5 bits) | opcode (7 bits) |   

_**Example:**_

add x5, x1, x2  # x5 = x1 + x2
