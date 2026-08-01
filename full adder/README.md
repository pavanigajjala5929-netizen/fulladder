# 1-Bit Full Adder in Verilog

## Overview

This project implements a 1-bit Full Adder using Verilog HDL.

A Full Adder adds three 1-bit binary inputs:

- A
- B
- Cin (Carry Input)

It produces two outputs:

- Sum
- Cout (Carry Output)

## Logic Equations

Sum = A XOR B XOR Cin

Cout = (A AND B) OR (B AND Cin) OR (A AND Cin)

## Truth Table

| A | B | Cin | Sum | Cout |
|---|---|-----|-----|------|
| 0 | 0 | 0 | 0 | 0 |
| 0 | 0 | 1 | 1 | 0 |
| 0 | 1 | 0 | 1 | 0 |
| 0 | 1 | 1 | 0 | 1 |
| 1 | 0 | 0 | 1 | 0 |
| 1 | 0 | 1 | 0 | 1 |
| 1 | 1 | 0 | 0 | 1 |
| 1 | 1 | 1 | 1 | 1 |

## Project Structure

```text
verilog-full-adder/
├── README.md
├── src/
│   └── full_adder.v
├── tb/
│   └── full_adder_tb.v
├── simulation/
│   └── waveform.png
└── docs/
    └── truth_table.png