# TASK-1

## RISC-V GNU Toolchain : 
 > *  _**Definition:**_ The RISC-V GNU Toolchain is a suite of development tools, including GCC, Binutils, GDB, and Newlib, used for compiling, debugging, and building software for RISC-V architectures.  
  
 > * _**Significance:**_ This toolchain is crucial for writing, compiling, and debugging code on RISC-V-based systems, enabling efficient embedded development, performance optimization, and low-level programming.   
  
Run the following command to install the GNU Toolchain:   
```
$ sudo apt-get install autoconf automake autotools-dev curl python3 python3-pip libmpc-dev libmpfr-dev libgmp-dev gawk build-essential bison flex texinfo gperf libtool patchutils bc zlib1g-dev libexpat-dev ninja-build git cmake libglib2.0-dev libslirp-dev  
$ git clone https://github.com/riscv/riscv-gnu-toolchain  
./configure --prefix=/opt/riscv
make linux
```   

## Yosys :  
 > * _**Definition:**_ Yosys is an open-source logic synthesis tool used for RTL (Register Transfer Level) design, primarily targeting FPGA and ASIC development. It supports Verilog and enables optimization, verification, and conversion of hardware designs.  
  
 > * _**Significance:**_ Yosys is crucial for synthesizing and optimizing hardware designs, enabling efficient FPGA-based development, digital circuit verification, and overall design improvement.
  
Run the following command to install Yosys:      
```   
$ git clone https://github.com/YosysHQ/yosys.git  
$ sudo apt install make   
$ cd yosys  
$ sudo apt-get install build-essential clang bison flex 
    libreadline-dev gawk tcl-dev libffi-dev git
    graphviz xdot pkg-config python3 libboost-system-dev 
    libboost-python-dev libboost-filesystem-dev zlib1g-dev  
$ make config-gcc  
$ make   
$ sudo make install  
Yosys 
```      

## GTKWave :  
 > * _**Definition:**_ GTKWave is an open-source waveform viewer used for analyzing and debugging digital signal simulations, supporting formats like VCD, LXT, and FST.
  
 > * _**Significance:**_ GTKWave aids in visualizing and debugging signal behaviors in digital designs, making it easier to verify and troubleshoot hardware simulations effectively.  
  
Run the following command to install GTKWave:     
```
$ sudo apt update  
$ sudo apt install gtkwave
```   


## Icarus Verilog (Iverilog) :   
 > * _**Definition:**_ Icarus Verilog (Iverilog) is an open-source Verilog simulation and synthesis tool used for compiling, simulating, and testing Verilog hardware descriptions.   
  
 > * _**Significance:**_ It is essential for verifying Verilog designs, enabling efficient simulation, debugging of logic errors, and ensuring correct hardware behavior before synthesis.   
  
Run the following command to install Iverilog:   
```
$ sudo apt-get install iverilog     
```   


