# 7-Segment Display (Hexadecimal Decoder) — Multisim

## Overview
This project implements a 4-bit to 7-segment hexadecimal decoder using combinational logic in NI Multisim.

The circuit accepts a 4-bit binary input (W, X, Y, Z) and drives segments A–G to display hexadecimal digits:

0–9, A, B, C, D, E, F

All segment equations are implemented using basic logic gates (AND, OR, NOT).

---

## Design Specifications

- Input: 4-bit binary (W X Y Z)
- Output: Seven segment control lines (A–G)
- Logic implementation: Sum-of-products (SOP)
- Supports full hexadecimal range (0–F)
- Designed and verified in NI Multisim

---

## Files

- `7 segment.ms14` — Multisim circuit file  
- `7 SEGMENT formulas.pdf` — Truth table and minimized Boolean expressions  
- `7-segment.png` — Circuit schematic screenshot  

---

## Circuit Diagram

![7-Segment Circuit](./7-segment.png)

---

## Technical Notes

- Each segment (A–G) is implemented as an independent Boolean function.
- Boolean expressions were derived from the truth table and simplified.
- Design assumes standard segment labeling convention.
- Output polarity may require inversion depending on display type (common-anode or common-cathode).

---

## Implementation Method

1. Construct full truth table for hexadecimal inputs.
2. Derive Boolean expressions for each segment.
3. Simplify expressions.
4. Implement using AND/OR/NOT gates.
5. Verify all 16 input combinations.

---

## Result

The final circuit correctly displays hexadecimal values (0–F) on a 7-segment display using pure combinational logic.
