# 400W SiC PFC Boost Converter

## Overview
A 4-layer, 400W Continuous Conduction Mode (CCM) Power Factor Correction (PFC) boost converter designed from end-to-end in Altium Designer. This mixed-signal power electronics project is engineered to step up raw AC mains to a highly stable 400V DC output, utilizing modern Silicon Carbide (SiC) semiconductor technology for high-efficiency power conversion. 

## Engineering Highlights
* **System Architecture:** Engineered the schematic and component architecture for a 400W CCM PFC boost converter, calculating and sourcing critical power stage components—including a SiC MOSFET, AC line filters, and bulk inductors—to support a highly stable 400V DC output.
* **Power Layout Strategy:** Translated the mixed-signal schematic into a custom 4-layer PCB layout, strategically sizing and prioritizing high-current 100-mil copper paths for the AC mains input, bridge rectifier, and DC output stages to safely manage massive power transfer without thermal degradation.
* **EMI Mitigation & Signal Integrity:** Protected sensitive 5V controller logic from high-frequency switching noise by implementing a single-point star grounding topology to separate the power and analog ground planes, while deliberately routing the SiC gate drive and high-voltage feedback networks through shielded inner copper layers.
* **Manufacturing Readiness:** Executed strict Design for Manufacturability (DFM) verification against factory capabilities, auditing the board to resolve high-voltage creepage rules, trace clearances, and 3D mechanical constraints before generating fully validated Gerber, NC Drill, and Bill of Materials (BOM) files for automated assembly.

## Core Components
* **Controller:** Texas Instruments UCC28180D CCM PFC Controller[cite: 3]
* **Switching Element:** Wolfspeed C3M0120090D Silicon Carbide (SiC) MOSFET[cite: 1]
* **Boost Diode:** Wolfspeed C3D06060A Silicon Carbide (SiC) Schottky Diode[cite: 1]
* **Boost Inductor:** Bourns 470µH High-Current Inductor (2300LL-471-V-RC)[cite: 1]
