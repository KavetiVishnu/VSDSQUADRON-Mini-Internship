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
$ git clone https://github.com/KavetiVishnu/VSDSQUADRON-Mini-Internship.git
$ cd VSDSQUADRON-Mini-Internship
```
The design code: iiitb_rv32i.v
The testbench code: iiitb_rv32i_tb.v  

## 3. Running and Simulating the Verilog Code
Use Icarus Verilog (iverilog) to compile and simulate the design:
```
$ iverilog -o VSDSQUADRON-Mini-Internship iiitb_rv32i.v iiitb_rv32i_tb.v
$ vvp VSDSQUADRON-Mini-Internship
```
## 4. Viewing the Simulation Waveform in GTKWave     

To visualize the waveform, GTKWave is used
```
$ gtkwave iiitb_rv32i.vcd
```
This setup allowed to successfully simulate the RISC-V processor and analyze the waveforms. 

   ![image](https://github.com/user-attachments/assets/29b88f5f-d17f-481e-bc87-73a5cae7dd63)
