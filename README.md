# PulseChord: Wearable Haptic/Vibrational Audio System
**OSHWA Certified Open Source Hardware | [UID Pending]**

![PulseChord Logo](PC%20LOGO.png)

## Project Overview
PulseChord is a purely analog haptic feedback belt that converts live audio into tactile vibrations through voice coil actuators positioned around the torso/waist. Designed to create an immersive sensory experience, it delivers real-time feedback corresponding to musical rhythm and dynamics.

This project bridges the gap between digital audio and physical sensation, utilizing an industrial manufacturing substrate to create an accessible, wearable haptic interface.

## Technical Research
The academic theory and signal-conditioning research behind this project can be found on SSRN:
* **SSRN Research Paper:** [PulseChord: Wearable Haptic Systems](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5532803)

## Technical Specifications
* **Architecture:** Purely Analog Signal Processing (No Software/Microcontroller)
* **Haptic Drivers:** 6x Full-range vibrational voice coil actuators (4Ω, 5W)
* **Amplification:** Dual TPA3110 (XHA232) Class D Stereo Amplifiers
* **Wiring Configuration:** Drivers are wired in **series pairs** (8Ω per pair) as shown in `Schematic 2.png`.
* **Conditioning:** TL074-based low-noise quad op-amp stage
* **Power:** 11.1V 3S LiPo Battery (2200mAh)
* **Chassis:** 50mm High-durability Nylon webbing with 3D-printed modular mounts
* **Fasteners:** M2 x 30mm Stainless Steel hardware

## Repository Structure
* `/Hardware`: Eagle Schematic (`.sch`) and Board (`.brd`) files
* `/Mechanical`: 3D source files (`.stl`, `.FCStd`) for speaker holders
* `BOM.txt`: Formatted Bill of Materials with manufacturer specifications
* `LICENSE.txt`: Hardware (CERN-OHL-P-2.0) and Documentation (CC-BY-SA-4.0) licenses
* `GerberFiles.zip`: Production-ready files for PCB fabrication

## Assembly Quick-Start
1. **PCB:** Fabricate the Gerber files using a standard 2-layer FR4 process.
2. **Printing:** Print 6x `Holder Design-Body.stl` in PLA (20% infill).
3. **Mechanical Assembly:** * First, mount the vibrational actuators into the 3D-printed holders using M2 x 30mm screws and nuts. 
    * Once secured, thread the 50mm nylon strap through the integrated slots in the holders.
4. **Wiring:** Wire the speakers in series pairs as detailed in **Schematic 2.png**. Connect each 8Ω load to the amplifier output channels.

## Licensing
* **Hardware:** [CERN-OHL-P-2.0](https://spdx.org/licenses/CERN-OHL-P-2.0.html)
* **Documentation:** [CC-BY-SA-4.0](https://creativecommons.org/licenses/by-sa/4.0/)

---

### Parental Consent & Attestation
I, **Muhammad Omar Farooq**, hereby attest to the authenticity and independent development of the PulseChord project by my son. I support the Open Source Hardware Association (OSHWA) certification of this hardware and provide parental consent for the publication of these technical materials and research on GitHub and SSRN.

**Signed:** Muhammad Omar Farooq  
**Date:** December 2025

---
**Developer:** Hariz Zoran Farooq  
**Contact:** harizzoranfarooq@gmail.com  
*Certified through the Open Source Hardware Association.*
