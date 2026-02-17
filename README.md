# Decoder-Reduction-Approximation-Scheme-for-Booth-Multipliers
 # Project Overview
This project presents a Decoder Reduction Approximation (DRA) based Booth Multiplier implemented in Verilog HDL for FPGA platforms. The design focuses on improving multiplier efficiency by simplifying the Booth decoding stage, which is a major contributor to area, delay, and power consumption in conventional multipliers.
Instead of utilizing all Booth decoders, the proposed architecture selectively processes only the most significant encodes. This approximation reduces hardware complexity and switching activity while preserving acceptable output accuracy.
The design is suitable for error-tolerant and energy-aware applications such as DSP systems, multimedia processing, and AI inference accelerators, where minor computational inaccuracies are tolerable.

# Implementation Summary (Xilinx Flow)
1.	Designed using Verilog HDL following a modular RTL methodology for clarity and scalability
2.	Implemented on Xilinx FPGA design tools (ISE/Vivado) using a standard synthesis–simulation workflow
3.	Architecture divided into key modules: Booth Encoder, Partial Product Generator, and Accumulation Unit
4.	DRA technique applied by reducing the number of active Booth decoders to lower logic utilization
5.	Partial products generated using radix-4 Booth encoding principles
6.	Accumulation performed using shift-and-add operations for efficient hardware mapping
7.	Functional verification carried out through a dedicated Verilog testbench with multiple input cases
8.	Post-synthesis analysis used to observe logic usage and timing behavior
9.	Design structured to allow future extension to higher bit-width multipliers

 #Research Contribution
•	Demonstrates decoder-level approximation in arithmetic unit design
•	Highlights trade-offs between accuracy and hardware efficiency
•	Provides a practical reference for FPGA-based approximate computing
•	Offers a scalable approach for low-power multiplier architectures
