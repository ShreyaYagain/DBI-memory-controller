Theoretical Framework
	1	Power in Memory Interfaces
	◦	Dynamic power (capacitance × voltage² × switching frequency) dominates.
	◦	DBI reduces switching activity, lowering dynamic power use.
	2	Data Bus Inversion (DBI)
	◦	Selectively inverts data bytes to minimize bit toggling.
	◦	Requires careful timing analysis to avoid setup/hold violations.
	◦	Signal integrity must be preserved (rise/fall times, jitter, crosstalk).
	3	Enhancements
	◦	ECC (Error Correction Codes) improves reliability.
	◦	Parallel processing can boost throughput and robustness.

Problem Statement
Traditional memory interfaces waste power due to excessive bit transitions at high data rates. With the rise of IoT (25B devices by 2030) and data-driven applications, energy efficiency is becoming critical. Without innovations like DBI, scalability and sustainability of future computing systems are at risk.
TOOLS:

EDA Playground: EDA Playground allows users to write and simulate code in Verilog, SystemVerilog, etc., which are crucial for designing and testing memory interface components like the DBI block. This platform also allows users to collaborate and work on a single project which makes it very helpful in group
projects. This tool is used in the project to simulate the circuit design and also see the consumed power (unitless method).

KeilMicrovision4(explored): Keil MicroVision 4 is an integrated development environment (IDE) for programming, debugging, and simulating embedded systems, primarily for ARM and other microcontroller architectures. This tool was explored but discontinued because we didn't get the desired outputs.

Xilinx: Xilinx develops programmable logic devices, such as FPGAs and adaptive SoCs, enabling customizable hardware solutions for a wide range of applications. This tool is used in the project to get results on the power consumed in Watts by the DBI and non-DBI circuits.


Results:        ￼
	•	Switching Frequency: Simulations on EDA Playground showed reduced switching activity with DBI enabled, directly lowering dynamic power. Without DBI, transitions (and power use) were higher.
	•	Power Evaluation: Xilinx analysis confirmed 20–30% lower power consumption and up to 25% bandwidth improvement in DBI mode.
	•	Discussion: The design met its objectives, achieving both energy savings and performance gains. ECC integration improved reliability, making the approach scalable for mobile and data center applications. Despite initial tool challenges, results highlight DBI’s dual benefits for efficiency and performance.

                               ￼
From the output values received we can see where DBI is used, there is a lower percentage of switching as compared to the switching in test cases where DBI is turned off.  So we can use this formula to see that power consumed is proportional to the amount od switching. So, the power consumed is lower during DBI usage.
