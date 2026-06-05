# AC to DC Converter – KiCad Project

## Overview
This project demonstrates a **basic AC‑to‑DC conversion circuit** designed and simulated using **KiCad**. It converts alternating current (AC) input into a stable direct current (DC) output using a full‑wave bridge rectifier and a smoothing capacitor. The design is ideal for educational purposes, prototyping low‑power supply modules, or as a foundation for regulated power supply development.

## Circuit Description
The circuit employs four **1N4007 diodes** configured as a **bridge rectifier**, which converts the AC input into pulsating DC. A **1000 µF electrolytic capacitor** smooths the output by filtering ripple voltage. A **10 kΩ resistor** provides discharge path stability, while a **2.2 kΩ resistor and LED** serve as a visual indicator for DC output availability.

### Key Components
| Component | Description | Function |
|------------|--------------|-----------|
| D1–D4 | 1N4007 Diodes | Bridge rectifier for AC‑to‑DC conversion |
| C1 | 1000 µF Capacitor | Filters ripple to produce smoother DC |
| R1 | 10 kΩ Resistor | Provides discharge path for C1 |
| R2 | 2.2 kΩ Resistor | Current limiter for LED indicator |
| D5 | LED | Indicates DC output presence |
| J1, J2 | Screw Terminals | AC input and DC output connections |

## Working Principle
1. **AC Input:** The circuit receives AC voltage through terminal J1.  
2. **Rectification:** Diodes D1–D4 conduct alternately during positive and negative half‑cycles, producing full‑wave rectified DC.  
3. **Filtering:** Capacitor C1 charges during peaks and discharges during troughs, reducing ripple.  
4. **Indication:** The LED (D5) glows when DC output is available, confirming successful conversion.

## Expected Output
- **Input:** 12 V AC (example)
- **Output:** ≈ 10.8 V DC (after diode drops)
- **Ripple:** < 1 V (depending on load and capacitor value)

## Applications
- Educational demonstration of rectification principles  
- Pre‑regulator stage for DC power supplies  
- Embedded or IoT prototypes requiring low‑voltage DC input  

## Repository Structure
