Welcome! This project is about building a 4-bit ALU (Arithmetic Logic Unit) using Verilog HDL.
It’s a perfect starter project for those learning digital design, Verilog, and VLSI basics.

**Project Overview**
In this project, we design and test a 4-bit ALU that can perform:
1. Arithmetic operations like Add and Subtract
2. Logic operations like AND, OR, XOR, NOT
3. Shift operations like Left Shift and Right Shift
All written in Verilog and simulated using Vivado or any Verilog simulator.

**What is an ALU?**
An ALU (Arithmetic Logic Unit) is the "brain" of every computer processor.It takes numbers (called operands) and performs math and logic operations based on a control signal called opcode.

**Supported Operations**
Opcode (3-bit)	Operation	Description
000	ADD	Adds A and B
001	SUB	Subtracts B from A
010	AND	Bitwise AND of A and B
011	OR	Bitwise OR of A and B
100	XOR	Bitwise XOR of A and B
101	NOT	Bitwise NOT of A only
110	LSHIFT	Left shift A by 1 bit
111	RSHIFT	Right shift A by 1 bit

**Registers & Data Flow Explained**
Inputs: 
A (4-bit register): Stores the first number. 
B (4-bit register): Stores the second number.
opcode (3-bit register): Selects the operation.
Output:
result (4-bit register): Stores the output of the ALU operation.

**How data flows:**
You give values to A and B.
Select an operation using the opcode.
ALU processes A and B based on the opcode.
Result is stored in the result register.

Example:
If A = 0101 (5), B = 0011 (3), and opcode = 000 (Add), The ALU will calculate 5 + 3 = 8 and store 1000 in result.

**How to Simulate**
*Option 1:* Using Vivado
step1: Open Vivado and create a new project.
step2: Add alu.v and tb_alu.v files.
step3: Click on Run Simulation → Run Behavioral Simulation.
step4:See the waveforms and verify the outputs.

*Option 2:* Using Online Simulator
step1: Go to EDA Playground
step2: Select SystemVerilog + Icarus Verilog.
step3: Paste alu.v and tb_alu.v code.
step4: Click Run and see the output.

Happy Learning!
