#  TASK1 - COMPILING C PROGRAMME USING RISCV COMPILER  
> * The command **`gedit sum.c`** opens (or creates if it doesn't exist) the **`sum.c`** file in the Gedit text editor, allowing to write or modify a C program before compilation.
  
```
gedit sum.c
```

<img width="959" alt="image" src="https://github.com/user-attachments/assets/df65174d-a3c6-4080-9b62-e1428a524f74" />      


> * The command **`gcc sum.c`** compiles the C program, and  **`./a.out`** executes it, producing an output of `55` as the sum of numbers from 1 to 10.   
    
```
gcc sum.c
./a.out
```
  
<img width="959" alt="image" src="https://github.com/user-attachments/assets/f7d8e9fd-4a63-4c9f-bd59-d2b1be3310d7" />         

> * The command `cat sum.c` displays the contents of the `sum.c` file in the terminal, allowing to view the C program without opening an editor.  
```
cat sum.c
```


<img width="959" alt="image" src="https://github.com/user-attachments/assets/f5c10dbf-6bbd-4931-a34d-0ffdd8ed2d8f" />               
> * The command `riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum.o sum.c` compiles `sum.c` for the RISC-V architecture with optimization level `O1`, using the LP64 ABI and RV64I architecture.    

> * The command `riscv64-unknown-elf-objdump -d sum.o` disassembles the compiled object file to inspect its assembly instructions.    

> * Using `riscv64-unknown-elf-objdump -d sum.o | less` allows for scrolling through the disassembled output, making it easier to analyze functions like `/main`.   


```
riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum.o sum.c
riscv64-unknown-elf-objdump -d sum.o
$riscv64-unknown-elf-objdump -d sum.o | less
/main
```  

<img width="959" alt="image" src="https://github.com/user-attachments/assets/60df8dff-556b-46a5-b554-18796ae65332" />     

```
$riscv64-unknown-elf-gcc -Ofast -mabi=lp64 -march=rv64i -o sum.o sum.c
$riscv64-unknown-elf-objdump -d sum.o
$riscv64-unknown-elf-objdump -d sum.o | less  
/main
```

<img width="959" alt="image" src="https://github.com/user-attachments/assets/b859eef5-3c9e-4475-9e18-26873a553d8f" />   
   
<img width="957" alt="image" src="https://github.com/user-attachments/assets/f887a418-5281-4f85-afb2-a2afde7a7220" />   

<img width="959" alt="image" src="https://github.com/user-attachments/assets/c8abcacb-19f9-4a54-ad20-288d7b5848e3" />





 






