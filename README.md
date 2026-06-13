# FPGA LED Blink

Board: Sipeed Tang Nano 20K (GW2AR-18C)

My first FPGA project.

## Description

This design increments a 24-bit counter on every clock cycle and drives the onboard LED using bit 23 of the counter.

```verilog
assign led = counter[23];
```

As the counter increases, the LED toggles at a visible rate, producing a blinking effect.

## Files

- `led_blink.v` – Verilog source
- `fpga_project.cst` – pin constraints

## Demo

(Video/GIF here)

## What I Learned

- Verilog modules
- Registers and wires
- Continuous assignments (`assign`)
- FPGA synthesis
- Place and Route
- Pin constraints (`.cst`)
- Programming a Gowin FPGA
