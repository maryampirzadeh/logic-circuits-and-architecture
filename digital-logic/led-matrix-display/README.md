# LED Matrix Moving Display (Digital Logic Project — NI Multisim)

Design and simulation of a **moving LED matrix display** implemented in **NI Multisim**, based on **shift-register / flip-flop sequencing** and **multiplexer-based control**.  
The project is implemented in **phases** (incremental development), ending with a complete LED-matrix animation that can move **left ↔ right**.

---

## Overview

This project builds a digital logic system that can display **characters/numbers/shapes** on an LED matrix and animate them as a **moving pattern**.  
Key idea: store an initial pattern, then repeatedly **shift** it with a clock to create motion across the LED array.

---

## What it Demonstrates (Learning Outcomes)

- D Flip-Flop–based storage and sequencing (Shift Register concept)
- Control of data-path using **Multiplexers** (mode selection)
- Clock-driven synchronous update (timing / animation speed control)
- Modular construction (scaling from small register → larger display)
- Practical simulation workflow in **NI Multisim** (circuit + report + diagrams)

---

## Core Features

- **Predefined pattern loading** (initial bits representing a shape/character)
- **Shift Right / Shift Left** motion modes (direction control)
- **Hold / Static display** mode (keep pattern unchanged)
- **Reset/Clear capability** (depending on the phase design)
- **Scalable architecture** (phased growth toward the final display)

---

## Repository Structure (This Folder)

**Main circuit and report**
- `LED Matrix.ms14` — Final integrated Multisim project (complete design)
- `LED Matrix.pdf` — Project report/documentation

**Phased implementation (incremental builds)**
- `first phase.ms14` — Phase 1 implementation
- `second phase.ms14` — Phase 2 implementation

**Diagrams / Screenshots**
- `first phase.PNG`
- `second phase.PNG`
- `third phase(final phase).PNG`

> Tip: GitHub renders `.PNG` directly in the browser, so these act as visual documentation.

---

## How to Run (NI Multisim)

1. Install **NI Multisim** (version compatible with `.ms14` files).
2. Open the main circuit:
   - `LED Matrix.ms14`
3. Start simulation:
   - **Simulate → Run**
4. Adjust animation speed (if needed):
   - Change the **clock frequency** used in the design.
5. Observe output:
   - LED states should animate according to the selected motion mode (left/right).

---

## How to Review the Design Quickly

If you want a fast understanding without opening Multisim:

1. Read `LED Matrix.pdf` (explains logic and phases)
2. Inspect diagrams:
   - `first phase.PNG` → initial register / core mechanism
   - `second phase.PNG` → expanded logic / scaling step
   - `third phase(final phase).PNG` → final integrated display

---

## Notes

- The project is fully **simulation-based** (Multisim).
- File naming is kept close to the original phase structure to match the report and diagrams.
- If you need cleaner naming later, you can rename files (GitHub keeps history).

---

## License

This repository includes a `LICENSE` file at the root level.  
If you reuse parts of the project, keep attribution consistent with the license terms.
