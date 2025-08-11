# 🧠 RISC-VIM 32-bit Processor

A custom-designed **RISC-VIM 32-bit pipelined processor**, developed to explore the functionality of RISC-V architecture using **Verilog/SystemVerilog**, with simulation and visualization tools.

---

## 📸 Project Overview

![Processor Block Diagram](images/https://private-user-images.githubusercontent.com/53592110/237593769-4caaeee5-e804-42ae-b0f0-264a62f2d385.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTQ5MjY2ODMsIm5iZiI6MTc1NDkyNjM4MywicGF0aCI6Ii81MzU5MjExMC8yMzc1OTM3NjktNGNhYWVlZTUtZTgwNC00MmFlLWIwZjAtMjY0YTYyZjJkMzg1LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA4MTElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwODExVDE1MzMwM1omWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTJhYWViYjdlZTQ3MTQyMzdjMTZiNDZlNWI0OTA5NjI5YTA5Mjc0NTQ2ZTg0NWU4OWUyZWI3M2RiYmZlZjM3ZDEmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.kKVqd8LFVJ-KBhpV3gHz8R55_VYYLcC_XvzFl2xifP8)

This project simulates a 32-bit RISC-V processor with:

- ✅ 5-Stage Pipeline (IF, ID, EX, MEM, WB)
- ✅ ALU for arithmetic/logical operations
- ✅ Forwarding Unit & Hazard Detection
- ✅ Modular Verilog design
- ✅ RV64I Instruction support

---

## 🧩 Core Modules

| Module Name        | Description                                   |
|--------------------|-----------------------------------------------|
| `IF_Stage`         | Instruction Fetch                             |
| `ID_Stage`         | Instruction Decode & Register Fetch           |
| `EX_Stage`         | ALU Execution and Branch Decision             |
| `MEM_Stage`        | Memory Read/Write                             |
| `WB_Stage`         | Write Back to Register File                   |
| `Hazard_Unit`      | Detects and handles data/control hazards      |
| `Forwarding_Unit`  | Enables data forwarding to avoid stalls       |

---

## 🛠️ Tools & Software Used

- **Verilog/SystemVerilog** – Core hardware design  
- **Cadence Xcelium / Virtuoso** – Simulation & Schematic design  
- **QuestaSim** – RTL Simulation  
- **RARS** – Assembly code writing & ISA testing  
- **Ripes** – Visual pipeline simulation and instruction walkthrough  
- **GTKWave** – View waveform outputs  
- **RISC-V GNU Toolchain** – Assembler and Hex generation  

---

## 📐 Architecture Visualization

![Pipeline GIF](images/pipeline.gif)

---

## 💡 Learning Support

- Used **RARS** to write and verify **RISC-V32 assembly**
- Used **Ripes** to understand pipeline behavior visually before RTL design
- Ran simulations on **Cadence tools** for waveform-level analysis

---

## 📦 Getting Started

```bash
# Clone repository
git clone https://github.com/yourname/riscvim-64bit.git
cd riscvim-64bit

# Run Simulation (example using
