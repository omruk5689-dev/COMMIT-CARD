# Dev Journal — NFC GitHub Profile Card
<img width="2160" height="1236" alt="3D_PCB1_2026-08-21 (2)" src="https://github.com/user-attachments/assets/51c01c42-f1b5-4c39-bb08-468fb952f019" />

**Date:** August 21, 2026
**Time spent:** ~1.5 hours
**Project:** NFC-programmable card that opens my GitHub profile when tapped with a phone

---

## Overview

Built a small PCB-based NFC card. The idea: tap the card with a phone, and it opens my GitHub profile. Designed in EasyEDA (schematic + PCB layout).

## Parts Used

- **U1** — NT3H2111W0FHKH (NFC/EEPROM tag IC)
- **U2** — 25x45mm NFC Antenna coil
- **C1** — 220nF capacitor
- **LED1** — status LED (K1-6816B)
- **R1** — 470Ω resistor (LED current limiting)

## What I Did

1. **Schematic design**
   - Placed the NT3H2111 NFC IC (U1) as the core chip
   - Connected the 25x45mm NFC antenna coil (U2) to the LA/LB pins
   - Added a 220nF capacitor (C1) across VOUT/VCC for tuning/decoupling
   - Wired an LED + 470Ω resistor as a status indicator
   - Read through the datasheet to get pin connections right (VSS, SCL, FD, VCC, SDA)
<img width="2362" height="1672" alt="SCH_Schematic1_1-P1_2026-08-21 (1)" src="https://github.com/user-attachments/assets/21c85454-98c2-46db-8532-064f402bef94" />

2. **Moved to PCB layout**
   - Updated schematic to PCB in EasyEDA
   - Routed traces for the design
<img width="2160" height="1246" alt="PCB_PCB1_2026-08-21" src="https://github.com/user-attachments/assets/ae6292c8-3be3-496c-baa4-46c11e26a086" />

3. **Hit DRC (Design Rule Check) errors**
   - Ran into clearance errors (Line to TH Pad, Line to SMD Pad) and connection errors (disconnected SMD pads)  NFC IC pads
   - Fixed by:
     - Adjusting `copperThickness1oz` design rule clearances (Track↔SMD Pad, Track↔TH Pad)
     - Rerouting tracks around tightly packed pin clusters instead of straight through
     - Re-checking net connections on disconnected pads

4. **Polish**
   - Added graphics/silkscreen touches to make the card look better

5. **Final check**
   - Re-ran DRC after fixes — all clear
   - Reviewed the whole board once more — good to go
<img width="2160" height="1263" alt="3D_PCB1_2026-08-21 (3)" src="https://github.com/user-attachments/assets/3334b3de-b18e-48a3-95d4-9323f66263f2" />
<img width="2160" height="1236" alt="3D_PCB1_2026-08-21 (2)" src="https://github.com/user-attachments/assets/42504fe5-56cb-4ec9-9cc9-961def0e9bcb" />

## Status

 Schematic complete
 PCB routed
 DRC errors resolved
 Visual polish added
 Next: fabrication / ordering

---

*Logged for GitHub repo commit history.*
