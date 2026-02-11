# 01 — LED Blink

## Aim

My first FPGA project: get an LED blinking on the Basys3 board.

This was mainly about getting used to Vivado and the overall FPGA workflow.

## What I learned

* The Basys3 has a 100 MHz clock
* That clock is far too fast to see directly
* A counter (clock divider) is needed to slow it down
* How to generate a bitstream and programme the board

## How it works

A counter counts clock cycles and toggles an LED once it reaches a set value.
This effectively slows the 100 MHz clock down to a visible blink.

## Files

* `blink.v` — Verilog design
* `basys3.xdc` — pin constraints

