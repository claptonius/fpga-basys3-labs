# 02 — Switch to LED Mirror

## Goal

Connect the 16 slide switches directly to the 16 LEDs.

If a switch is on, the matching LED turns on.

## Why...

This was my first project where the FPGA reacts to real inputs.
It helped me understand how inputs, outputs and constraints work together.

## What I learned

* How to use the Basys3 switches as inputs
* How to map pins using an XDC file
* Basic combinational logic in Verilog
* Write HDL → build → program → test on hardware

## Verilog

```verilog
module top(
    input  [15:0] sw,
    output [15:0] led
);

assign led = sw;

endmodule
```

## Result

Flipping a switch instantly lights the corresponding LED.


