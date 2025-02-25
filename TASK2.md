# TASK2 - Comparing -O1 vs -Ofast in SPIKE Simulation   

The SPIKE simulator is an emulation tool for the RISC-V Instruction Set Architecture (ISA) that enables testing and verification of programs compiled for RISC-V. In this project, a basic C program was compiled using the RISC-V GCC toolchain and executed on SPIKE. The program’s behavior was examined under two compiler optimization settings:

* _**-O1:** This optimization level applies moderate improvements to boost performance and reduce code size while maintaining compatibility with language standards. It offers a balanced trade-off between execution speed and reliability, making it ideal for general-purpose applications._

* _**-Ofast:** This level activates all -O3 optimizations along with extra aggressive enhancements that maximize performance, even if it means bending some language standards. It is best used in scenarios where achieving the highest possible speed is more critical than strict standard adherence._

```
gedit ha.c
```

<img width="1120" alt="image" src="https://github.com/user-attachments/assets/8d56fc3f-b33b-44eb-9088-9deafd606235" />     

```
gcc ha.c
./a.out
```

<img width="1120" alt="image" src="https://github.com/user-attachments/assets/a5fb48f5-04f8-459f-865f-9fe81645b12e" />       

```   
cat ha.c
```   

<img width="1118" alt="image" src="https://github.com/user-attachments/assets/e168ba15-2ad4-429c-a427-28f9c111c815" />      

```
$ riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c
$ riscv64-unknown-elf-objdump -d sum1ton.o | less
$ spike pk sum1ton.o
$ spike -d pk sum1ton.o
```


<img width="1118" alt="image" src="https://github.com/user-attachments/assets/0b0d65fb-3d60-4723-98b7-81387df5aacc" />    

<img width="1120" alt="image" src="https://github.com/user-attachments/assets/f3cf1d74-a338-4603-b7b0-3e4d57c43a00" />

<img width="1120" alt="image" src="https://github.com/user-attachments/assets/ae09a731-ce9a-43eb-b821-7f22aba9754d" />    

<img width="1120" alt="image" src="https://github.com/user-attachments/assets/e97228c1-e56c-4d73-971c-037aecabe5cd" />






