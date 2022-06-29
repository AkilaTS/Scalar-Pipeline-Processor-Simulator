# Scalar-Pipeline-Processor-Simulator
C++ program to simulate the execution of machine code in a 5 stage scalar pipeline processor (RISC processor) with operand forwarding through the Register file.

The processor has a 256B instruction cache (ICache.txt) and a 256B data cache (DCache.txt), both having a read port and a write port each. Both are direct-mapped caches with block size of 4B.

Both the instruction cache and data cache are assumed to be perfect, so there won’t be any cache misses. The processor has a register file (RF) with sixteen, 8-bit registers, named R0, R1,..., R15. R0 always stores the value “0”. Negative numbers are stored in 2’s complement form.

The machine code is read from the Instruction cache (ICache.txt), data is accessed from the Data Cache (DCache.txt) and the contents of the Register File are read from RF.txt. The changes to the Register File and Data Cache will be made in the RF.txt and DCache.txt files itself.

The simulator also displays various statistics such as no. of instructions processed, no. of cycles taken to execute the code, no. of instructions of each type, no. of data and control stalls, CPI etc in the file "Output.txt".
