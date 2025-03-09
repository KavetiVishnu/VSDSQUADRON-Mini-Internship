# Execution of RISC-V Functional Simulation:   
## 1. Creating a New Directory
Navigate to the desktop and created a new directory named Vishnu:
```
$ cd Desktop
$ mkdir Vishnu
$ cd Vishnu
```

## 2. Cloning the GitHub Repository
Copy the design code and testbench code from the provided GitHub repository to local system:
```
$ git clone https://github.com/KeerthiPatil/VSDSQUADRON_MINI_INTERNSHIP.git
$ cd VSDSQUADRON_MINI_INTERNSHIP
```
The design code: ins_RV32EC.v
The testbench code: ins_RV32EC_tb.v  

## 3. Running and Simulating the Verilog Code
Use Icarus Verilog (iverilog) to compile and simulate the design:
```
$ iverilog -o VSDSQUADRON_MINI_INTERNSHIP ins_RV32EC.v ins_RV32EC_tb.v
$ vvp VSDSQUADRON_MINI_INTERNSHIP
```
## 4. Viewing the Simulation Waveform in GTKWave     

To visualize the waveform, GTKWave is used
```
$ gtkwave ins_RV32EC.vcd
```
This setup allowed to successfully simulate the RISC-V processor and analyze the waveforms. 

   ![image](https://github.com/user-attachments/assets/29b88f5f-d17f-481e-bc87-73a5cae7dd63)
