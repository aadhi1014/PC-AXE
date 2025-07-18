# PC-AXE: PCIe-Based Bitcoin Miner (12x BM1370, 14.4TH/s @ 200W)

![License: TAPR OHL-NC](https://img.shields.io/badge/License-TAPR%20OHL--NC-blue.svg)

**PC-AXE** is a compact, PCIe x4-based, open-hardware Bitcoin miner designed to plug directly into desktop computers. Inspired by [Bitaxe](https://github.com/skot/bitaxe), Bitcrane, and professional mining cards, PC-AXE uses twelve BM1370 ASIC chips and a 6-phase high-efficiency buck converter to deliver up to **14.4TH/s** of hashrate at just **200W** power draw.


**Note:** PC-AXE is a **work in progress**. Hardware files are being finalized, and firmware development is ongoing. Community contributions and testing feedback are welcome.

---

![PC-AXE Top View](./images/top.png)  
*Top side of the PC-AXE board*

![PC-AXE Bottom View](./images/bottom.png)  
*Bottom side of the PC-AXE board*

---

## Features

- **Standard PCIe x4 Form Factor**
  - Easily integrates into modern desktop systems
  - Powered via PCIe slot with external power input

- **12 × BM1370 ASIC Chips**
  - Same chips used in Antminer S21
  - Estimated hashrate of ~1.2TH/s per chip

- **6-Phase 180A Buck Converter**
  - High-efficiency power delivery at 1.1V
  - Total power consumption approximately 200W

- **Fully Open-Source Design**
  - Includes KiCad schematics, layout, and source files
  - Planned firmware compatibility with Bitaxe ecosystem

- **UART Debug Interface**
  - Communicates via USB-to-UART bridge (e.g. FT4232H)
  - Supports daisy-chained UART control for ASICs

- **Design Inspiration**
  - Derived from Bitaxe (compact solo miner)
  - Influenced by Bitcrane

---

## Getting Started

### Build Instructions

1. Open the project in KiCad 7 or newer
2. Review the schematic and PCB layout
3. Export Gerber files and order the PCB from your preferred manufacturer
4. Assemble the board using the BOM (to be published)
5. Flash control firmware (currently in development)

### UART Connection

Connect an FTDI FT4232H or equivalent USB-to-UART adapter to the debug header. A single UART channel can control all 12 ASICs.

---

## Important License Notice  
This project was relicensed under the **TAPR Open Hardware License – Non-Commercial (OHL-NC)** on **July 11, 2025**.  
All clones and forks made **after this date** are subject to **non-commercial use only**.  

**Commercial use, manufacturing, or distribution of this work is strictly prohibited without explicit written permission from the copyright holder.**  

If you cloned this repository *before July 11, 2025*, please contact the author for updated licensing terms.

---

## License

This hardware design is licensed under the TAPR Open Hardware License – Non-Commercial (OHL-NC).  
You are free to use, modify, and distribute for **non-commercial purposes**.  

**Commercial use requires explicit written permission from the copyright holder.**  
See the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

This project draws inspiration and technical insight from several open-source mining hardware efforts:

- [Bitaxe](https://github.com/skot/bitaxe) – foundational open hardware Bitcoin miner  
- [NerdAxe](https://github.com/BitMaker-hub/NerdAxe) – compact ESP32-based BM1370 miner 
- [NerdOCTAXE-Gamma](https://github.com/5toliv/NerdOCTAXE-Gamma) – 8‑ASIC miner derived from NerdQaxe 
- [NerdEKO‑Gamma](https://github.com/phil31/NerdEKO-Gamma) – ESP32-based miner reference design   
- [Bitcrane](https://bitcointalk.org/index.php?topic=951507.0) – USB antminer control board  design

We thank these creators for their contributions to the open-source mining community.
---

## Contact / Collaboration

If you are a developer, hardware enthusiast, or miner interested in contributing to this open hardware project, feel free to open issues or pull requests. Community collaboration is welcome.

