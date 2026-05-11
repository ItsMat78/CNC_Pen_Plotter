# CNC Pen Plotter (NEMA17 · Fusion 360 · UGS)
<img width="1156" height="1542" alt="image" src="https://github.com/user-attachments/assets/a3766ec6-50b2-4197-9584-66d594cedb4e" />

A custom-built **CNC Pen Plotter** designed for **NEMA17 stepper motors**, with all mechanical parts modeled in **Fusion 360** and fabricated using 3D printing. The machine operates using standard **G-code** and is controlled via **Universal G-code Sender (UGS)**.

This project focuses on simplicity, modularity, and hackability—no proprietary nonsense, just clean mechanics and open tooling.

**Warning:** The files have problems with friction in sliding parts

---

## 🛠 Features

- Custom mechanical design optimized for **NEMA17 stepper motors**
- Fully parametric **Fusion 360** CAD models
- 3D-printable **STL files** included
- Standard **G-code** workflow
- Compatible with **Universal G-code Sender (UGS)**
- Supports pen plotting, sketches, and basic 2D drawings
- Modular design for easy upgrades (laser, different tool heads, etc.)

---

## ⚙️ Hardware Overview

- **Stepper Motors:** NEMA17  
- **Controller:** GRBL-compatible controller (Arduino-based or equivalent)
- **Motor Drivers:** A4988 / DRV8825 (or compatible)
- **Frame:** 3D printed parts + standard fasteners
- **Tool Head:** Pen holder (custom design)
- **Power Supply:** As per controller and motor requirements

> Note: Exact wiring and driver configuration may vary depending on the controller used.

---

## 🧩 Mechanical Design

All mechanical components were **designed from scratch in Fusion 360**.  
The repository includes:

- Editable **Fusion 360 design files**
- Exported **STL files** ready for 3D printing
- Designs tailored specifically for NEMA17 motor mounting and alignment

Directory structure example:
/cad -> Fusion 360 files
/stl -> Exported STL files

---

## 💻 Software & Control

- **Firmware:** GRBL (or compatible)
- **G-code Sender:** Universal G-code Sender (UGS)

### Workflow
1. Create or import vector designs (SVG, DXF, etc.)
2. Convert to G-code using your preferred CAM tool
3. Send G-code to the plotter using **UGS**
4. Plot responsibly

---

## 🚀 Getting Started

1. Assemble the mechanical structure using the provided STL files
2. Mount NEMA17 motors and wire them to the controller
3. Upload GRBL firmware to your controller
4. Configure motor steps/mm and limits in GRBL
5. Connect via **Universal G-code Sender**
6. Run a test plot

---

## 📁 Repository Structure

├── cad/ # Fusion 360 source files
├── stl/ # 3D printable STL files
├── gcode/ # Sample G-code files (optional)
├── docs/ # Additional documentation or images
└── README.md

---

## 🧠 Notes & Limitations

- Designed primarily for **2D plotting**, not high-force CNC operations
- Accuracy depends heavily on belt tension, frame rigidity, and calibration
- Not intended for high-speed or industrial use (your pen will revolt)

---

## 🔧 Future Improvements

- Limit switches and homing
- Improved pen lift mechanism
- Better cable management
- Optional laser or engraving attachment
- Cleaner enclosure design

---

## 📜 License

MIT

---

## 🙌 Acknowledgements

- GRBL project
- Universal G-code Sender
- The eternal patience required for stepper motor calibration
