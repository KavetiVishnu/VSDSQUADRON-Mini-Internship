# VSDSQUADRON-Mini-Internship  

The **VSDSquadron Mini Internship 2025** focuses on RISC-V architecture and open-source tools for VLSI chip design. Under the mentorship of **Mr. Kunal Ghosh**, I am gaining hands-on experience in designing RISC-V-based systems while working with industry-standard open-source methodologies.    

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------   

<a href="https://github.com/KavetiVishnu/VSDSQUADRON-Mini-Internship/blob/e912ae0a2eb57db06ed19a972eeaaf69ce7fcf5f/TASK1.md">**TASK1**</a> **:Set up the RISC-V toolchain using the VDI file. Write a basic C program to compute the sum of numbers from 1 to n. First, compile and run the program using the standard GCC compiler to verify the output. Then, recompile the same code using the RISC-V GCC compiler to examine the generated instructions and compare the differences.**

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------    
<a href="https://github.com/KavetiVishnu/VSDSQUADRON-Mini-Internship/blob/8938bf862890063faa56e395011558d98dd1ae1c/TASK2.md">**TASK2**</a>    
## My Implementation Approach : 
-> Initially, I started by writing a C program to implement a half-adder. After completing the code, I compiled and executed it using gcc and ./a.out to verify its correctness.

Next, I proceeded with optimization and simulation by compiling the program with the -O1 optimization flag using GCC. To analyze the generated machine code, I disassembled the object file using riscv64-unknown-elf-objdump -d. Then, I simulated the execution on SPIKE using spike pk ha.o and spike -d pk ha.o.

After that, I performed a comparison with -Ofast optimization by recompiling the program with the -Ofast flag. I repeated the disassembly and SPIKE simulation steps to observe the performance differences between -O1 and -Ofast optimizations.

