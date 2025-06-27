# 🧠 RISC-VIM 64-bit Processor

A custom-designed **RISC-VIM 64-bit pipelined processor**, developed to explore the functionality of RISC-V architecture using **Verilog/SystemVerilog**, with simulation and visualization tools.

---

## 📸 Project Overview

![Processor Block Diagram](images/block_diagram.png)

This project simulates a 64-bit RISC-V processor with:

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

- Used **RARS** to write and verify **RISC-V64 assembly**
- Used **Ripes** to understand pipeline behavior visually before RTL design
- Ran simulations on **Cadence tools** for waveform-level analysis

---

## 📦 Getting Started

```bash
# Clone repository
git clone https://github.com/yourname/riscvim-64bit.git
cd riscvim-64bit

# Run Simulation (example using
