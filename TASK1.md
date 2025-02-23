#  TASK1 - COMPILING C PROGRAMME USING RISCV COMPILER
```
gedit sum.c
```

<img width="959" alt="image" src="https://github.com/user-attachments/assets/df65174d-a3c6-4080-9b62-e1428a524f74" />      

```
gcc sum.c
./a.out
```
  
<img width="959" alt="image" src="https://github.com/user-attachments/assets/f7d8e9fd-4a63-4c9f-bd59-d2b1be3310d7" />        

```
cat sum.c
```


<img width="959" alt="image" src="https://github.com/user-attachments/assets/f5c10dbf-6bbd-4931-a34d-0ffdd8ed2d8f" />          

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





 






