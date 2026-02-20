# LED Matrix Moving Display (Digital Logic — NI Multisim)

A phased digital-logic implementation of a **moving LED matrix display** in **NI Multisim**, using **shift-register style sequencing** and **multiplexer-controlled datapaths** to load and shift predefined patterns (character/number/shape) **left ↔ right**.

---

## Quick Snapshot

- **Platform:** NI Multisim (`.ms14`)
- **Outcome:** Animated LED-matrix pattern movement with direction control
- **Method:** Modular (phase-based) build-up → final integrated design
- **Artifacts:** Circuit files + report + phase diagrams (screenshots)

---

## Architecture & Design Rationale

This project models a classic synchronous display pipeline:

1. **Pattern definition / storage** (binary vector representing a symbol/shape)
2. **Clocked shifting** to create animation across the LED matrix
3. **Control logic** (e.g., direction selection) that selects the next-state path using multiplexers
4. **Output mapping** to LED rows/columns (depending on your matrix wiring)

---

## Project Phases (with Diagrams)

### Phase 1 — Core storage / initial movement logic
![Phase 1 Diagram](./first%20phase.PNG)

### Phase 2 — Expanded logic / scaling toward full display
![Phase 2 Diagram](./second%20phase.PNG)

### Phase 3 (Final) — Integrated LED matrix moving display
![Final Phase Diagram](./third%20phase%28final%20phase%29.PNG)

---

## Files Included

### Final integrated project
- `LED Matrix.ms14` — Final NI Multisim circuit (complete design)
- `LED Matrix.pdf` — Documentation/report

### Phase implementations
- `first phase.ms14` — Phase 1 circuit
- `second phase.ms14` — Phase 2 circuit

### Diagrams (screenshots)
- `first phase.PNG`
- `second phase.PNG`
- `third phase(final phase).PNG`

---

## How to Run (NI Multisim)

1. Open `LED Matrix.ms14` in **NI Multisim**.
2. Start simulation: **Simulate → Run**.
3. If motion is too fast/slow, adjust the **clock frequency** in the circuit.
4. Use the control inputs (direction/select lines) to switch between **Shift Left** and **Shift Right**.
5. Observe the LED matrix output: the pattern should move smoothly across the display.

---

## How to Demo (30–60 seconds)

A clean demo video typically shows:

1. **Load** a pattern (show the initial static pattern on LEDs)
2. Run **Shift Right** for a few seconds
3. Switch to **Shift Left** and show reversal
4. Optionally show **Reset/Clear** (if available)
5. Zoom briefly on the clock/control part to prove it’s synchronous logic

---

## Notes

- This repository stores the project in a **phase-based** structure to match development and evaluation.
- File naming is preserved to align diagrams, Multisim circuits, and the PDF report.
- GitHub can preview `.PNG` files directly; the `.ms14` files require NI Multisim.

