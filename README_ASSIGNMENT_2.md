# UNLOX-ACADEMY-ASSIGNMENT-2
# Design and Simulation of a 4-bit Arithmetic Logic Unit (ALU) using Verilog

## Description
This project presents the design and simulation of a **4-bit Arithmetic Logic Unit (ALU)** using Verilog Hardware Description Language. The ALU is a fundamental component in digital systems and processors, responsible for performing arithmetic and logical operations.

The designed ALU takes two 4-bit inputs (**A** and **B**) and a 2-bit select signal (**sel**) to determine the operation. Based on the select input, the ALU performs the following operations:

- Addition  
- Subtraction  
- Bitwise AND  
- Bitwise OR  

The design is implemented using combinational logic with a `case` statement inside an `always` block.

A testbench is created to verify the design by applying multiple input combinations. The simulation results are stored in a **VCD (Value Change Dump)** file and visualized using **GTKWave**.

---

## Objectives
- Understand the working of an ALU  
- Implement digital logic using Verilog HDL  
- Simulate and verify designs using testbenches  
- Analyze waveform outputs using GTKWave  

---

## Tools Used
- Verilog HDL  
- Icarus Verilog (`iverilog`)  
- GTKWave  

---

## Simulation Steps

```bash
# Compile
iverilog -o alu_out alu.v alu_tb.v

# Run simulation
vvp alu_out

# View waveform
gtkwave alu.vcd
