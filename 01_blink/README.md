# Basys 3 LED Blink (FPGA)

My first FPGA project using Verilog and AMD Vivado.

## Board
Digilent Basys 3 (Artix-7)

## Description
This project divides the onboard 100 MHz clock to blink LED0 at a frequency f of roughly 1 Hz.  
It serves as a simple “hello world” design to confirm the toolchain, board setup, and programming workflow.

## Concepts
1. FPGA clock signal (100 MHz on Basys3)
2. Clock division using a counter
3.Generating a bitstream in Vivado
4. Programming the FPGA board

## How to build and run
1. Open the `.xpr` project in Vivado.
2. Run synthesis, implementation, and generate the bitstream.
3. Connect the Basys 3 via USB (JTAG mode).
4. Program the FPGA using Hardware Manager.

## Notes
This repository contains only source and project files.  
Generated build artefacts are excluded via `.gitignore`.

