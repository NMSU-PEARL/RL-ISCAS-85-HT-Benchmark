# RL-ISCAS-85-HT-Benchmark
Hardware Trojan Benchmark created by a Reinforcement Learning Agent

The zip files are password-protected. To gain access, please email badawy@nmsu.edu

Readme:
*******************
General Information
*******************
1- This zip file contains a subset of ISCAS-85 benchmarks in which hardware Trojans (HTs) have been inserted.
2- The benchmarks were generated by a Reinforcement Learning (RL) toolset where an agent explores the environment (in this case, a Verilog circuit) and inserts HTs.
3- The HT circuits are built from anded trigger nets and an XOR gate for payload.
4- For the details of our HT insertion criteria, please refer to our paper "Hardware Trojan Insertion Using Reinforcement Learning" (https://dl.acm.org/doi/abs/10.1145/3526241.3530379).
5- If you use this benchmark in your research, we kindly request you to cite our paper "Hardware Trojan Insertion Using Reinforcement Learning" (https://dl.acm.org/doi/abs/10.1145/3526241.3530379).


*******************
Benchmark Details
*******************
1- The dataset includes 6 benchmarks namely: c432, c880, c1355, c1908, c3540, c6288
2- Each Benchmark contains 2-input, 3-input, 4-input, and 5-input HTs.
3- The benchmarks name format is verilog_XX.v 
4- Commented at the top of each .v file, you can see the HT trigger nets.
5- At the bottom of each .v file, you see these trigger nets anded, followed by an XOR gate where it is the payload.
6- Each Verilog file has its own log file, and the format is log_verilog_XX_YY.txt. XX is the same as the Verilog HT name, and YY is the ICP (Input Coverage Percentage). It is 0<YY=<1.
7- ICP states what percentage of the circuit total inputs were involved during the activation of that particular HT. This information can also be found inside each of the log files.
8- The input combination to activate the particular is included in the log files for sanity check. It is called the input stack.



