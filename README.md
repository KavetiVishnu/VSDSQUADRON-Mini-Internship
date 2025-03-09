 # <a href="https://github.com/KavetiVishnu/VSDSQUADRON-Mini-Internship"> VSDSQUADRON-MINI-INTERNSHIP </a>


The **VSDSquadron Mini Internship 2025** focuses on RISC-V architecture and open-source tools for VLSI chip design. Under the mentorship of **Mr. Kunal Ghosh**, I am gaining hands-on experience in designing RISC-V-based systems while working with industry-standard open-source methodologies.    

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------      

## <a href="https://github.com/KavetiVishnu/VSDSQUADRON-Mini-Internship/blob/e912ae0a2eb57db06ed19a972eeaaf69ce7fcf5f/TASK1.md">**_RISC-V Toolchain Configuration and C Code Compilation Using GCC and RISC-V Compilers._**</a>

## My Implementation Approach for <a href="https://github.com/KavetiVishnu/VSDSQUADRON-Mini-Internship/blob/e912ae0a2eb57db06ed19a972eeaaf69ce7fcf5f/TASK1.md">**TASK1**</a> :
**step-1:** _I started by setting up the RISC-V toolchain using the VDI file. Then, I wrote a C program to compute the sum of numbers from 1 to n._

**step-2:** _First, I compiled and executed the program using the standard GCC compiler to verify the output. After confirming correctness, I recompiled it using the RISC-V GCC compiler._   

**step-3:** _Finally, I examined the generated assembly instructions to compare the differences between standard GCC and RISC-V compilation._     


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------    
## <a href="https://github.com/KavetiVishnu/VSDSQUADRON-Mini-Internship/blob/8938bf862890063faa56e395011558d98dd1ae1c/TASK2.md">**_Debugging C Code Using SPIKE Simulation and Interactive Debugging Mode._**</a> 

## My Implementation Approach for <a href="https://github.com/KavetiVishnu/VSDSQUADRON-Mini-Internship/blob/8938bf862890063faa56e395011558d98dd1ae1c/TASK2.md">**TASK2**</a> :    

**step-1:** _Initially, I started by writing a C program to implement a half-adder. After completing the code, I compiled and executed it using gcc and ./a.out to verify its correctness._

**step-2:** _Next, I proceeded with optimization and simulation by compiling the program with the -O1 optimization flag using GCC. To analyze the generated machine code, I disassembled the object file using riscv64-unknown-elf-objdump -d. Then, I simulated the execution on SPIKE using spike pk ha.o and spike -d pk ha.o._

**step-3:** _After that, I performed a comparison with -Ofast optimization by recompiling the program with the -Ofast flag. I repeated the disassembly and SPIKE simulation steps to observe the performance differences between -O1 and -Ofast optimizations._

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------   
##  <a href="https://github.com/KavetiVishnu/VSDSQUADRON-Mini-Internship/blob/c50db42157cc7190ab60296c14ac2f27b4b6c632/TASK3.md">**_Identification of 15 Unique RISC-V Instructions._**</a>     

## My Implementation Approach for <a href="https://github.com/KavetiVishnu/VSDSQUADRON-Mini-Internship/blob/c50db42157cc7190ab60296c14ac2f27b4b6c632/TASK3.md">**TASK3:**</a>        

**step-1:** _In Step 1, I extensively studied the RISC-V Instruction Set Architecture (ISA) using resources from Google books and academic papers. I thoroughly learned each instruction format, analyzed examples, and grasped the underlying principles of the ISA. This deep understanding empowered me to confidently identify, interpret, and explain 15 unique RISC-V instructions, which were essential for the subsequent tasks in my implementation._     

**step-2:** _In Step 2, I analyzed the riscv-objdump output generated from the executions of Task 1 and Task 2. During this analysis, I identified and extracted 15 unique RISC-V instructions that were used in both tasks. This step helped in solidifying my understanding of the instructions and their formats as I reviewed the actual machine-level implementations._  
    
**step-3:** _In Step 3, I carefully identified and provided clear explanations for the 15 unique RISC-V instructions in Task 3. I broke down each instruction's functionality, purpose, and its impact on the overall execution of the application. This step involved ensuring that each instruction was thoroughly understood and could be explained with precision in the context of Task 3._   

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- 

##  <a href="https://github.com/KavetiVishnu/VSDSQUADRON-Mini-Internship/blob/f183fb9032f6cfb8412f1047350306445334f86a/TASK-4.md/TASK4.md">**_Conducting a Functional Simulation Experiment with RISC-V Core_**</a>         











