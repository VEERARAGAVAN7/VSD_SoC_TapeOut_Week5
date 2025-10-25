# ⚡ Floorplanning & Placement — Week 5

<div align="center">

![RISC-V](https://img.shields.io/badge/RISC--V-SoC%20Tapeout-blue?style=for-the-badge&logo=riscv)
![VSD](https://img.shields.io/badge/VSD-Program-orange?style=for-the-badge)
![India](https://img.shields.io/badge/Made%20in-India-saffron?style=for-the-badge)

</div>

<div align="center">

🧩 RTL & Synthesis → 🏗️ Floorplanning → 📌 Placement → 🧪 DRC & LVS → 🎯 Tapeout Ready

</div>

---

## 📅 Week 5 — Floorplanning & Placement

This week focused on **physical design steps** of the RISC-V SoC, specifically **floorplanning** and **placement**.  
The tasks involved setting up the **config.mk**, analyzing the **floorplan errors**, optimizing **macro placement**, and observing **placement results** in GUI.  
All operations were performed using **OpenROAD**, **Magic**, and associated standard cell libraries.

---

### 🧪 Day 1 — RTL2GDS Flow: Initial Steps

#### 📘 Objective
To set up the **design environment** and prepare the project for **synthesis, floorplanning, and placement**.

#### ⚙️ Key Topics
- Understanding **config.mk** variables.
- Directory and **file structure after setup**.
- Initial **RTL2GDS flow preparation**.

#### 🧰 Steps Performed
1. Created project directory and added RTL source files.
2. Configured `config.mk` with target library and clock constraints.
3. Verified **project structure** and script paths.

#### 📈 Observations
- Proper setup prevents errors in **floorplan and placement stages**.
- Ensures **consistent netlist synthesis** and tool execution.

---

### 🧪 Day 2 — Run Synthesis

#### 📘 Objective
To synthesize the RTL to a **gate-level netlist** ready for floorplanning.

#### ⚙️ Key Topics
- **Netlist generation**
- Synthesis logs and statistics
- Verifying **synthesized design against RTL**

#### 🧰 Steps Performed
1. Run synthesis using **Yosys** with Sky130 libraries.
2. Generated **synthesized netlist (`.v`)**.
3. Checked **synthesis report** for area, timing, and power.

#### 📈 Observations
- Gate-level netlist matches RTL behavior.
- Timing slack and cell utilization were within acceptable range.

---

### 🧪 Day 3 — Run Floorplan

#### 📘 Objective
To define **chip area, macro placement, and IO pins** for the SoC.

#### ⚙️ Key Topics
- Defining **core area** and **utilization targets**.
- Macro placement strategies.
- Handling **floorplan errors**.

#### 🧰 Steps Performed
1. Set floorplan parameters in **OpenROAD scripts**.
2. Observed errors such as **[ERROR MPL-0045] unbalanced partitioning**.
3. Fixed errors by adjusting **target utilization** and **macro placements**.

#### 📈 Observations
- Correct floorplanning prevents later congestion during placement.
- Proper **macro alignment** ensures better routing and timing.

---

### 🧪 Day 4 — Run Placement

#### 📘 Objective
To place all standard cells and macros within the floorplan **optimally**.

#### ⚙️ Key Topics
- Standard cell placement
- Legalization and spreading
- Placement optimization to reduce wirelength and congestion

#### 🧰 Steps Performed
1. Ran **OpenROAD placement scripts**.
2. Verified placement in **GUI** for overlaps and spacing.
3. Generated **placement reports** for area utilization.

#### 📈 Observations
- Cells were placed without overlap and obeyed design rules.
- Placement quality impacts **timing closure** and overall PPA (Power, Performance, Area).

---

### ✅ Key Learnings from Week 5

- Understood **floorplanning parameters** and constraints in OpenROAD.
- Learned to debug **floorplan errors** and optimize macro placement.
- Performed standard cell **placement**, ensuring legality and efficiency.
- Observed how **floorplan and placement quality** directly affects **timing and routing**.

---

## 🙏 **Acknowledgment**

<div align="center">

### 🏆 **Program Leadership & Support**

I sincerely thank [**Kunal Ghosh**](https://github.com/kunalg123) and Team **[VLSI System Design (VSD)](https://vsdiat.vlsisystemdesign.com/)** for their guidance and mentorship throughout **Week 5 — Floorplanning & Placement** of the **RISC-V SoC Tapeout Program**.

</div>

---

## 📈 **Weekly Progress Tracker**

![Week 1](https://img.shields.io/badge/Week%201-RTL%20Foundations-success?style=flat-square)
![Week 2](https://img.shields.io/badge/Week%202-SoC_Design%20Flow-success?style=flat-square)
![Week 3](https://img.shields.io/badge/Week%203-STA-success?style=flat-square)
![Week 4](https://img.shields.io/badge/Week%204-CMOS%20Design-success?style=flat-square)
![Week 5](https://img.shields.io/badge/Week%205-Floorplanning%20%26%20Placement-brightgreen?style=flat-square)

### 🚀 **Journey Continues...**

In the upcoming weeks, I will explore **clock tree synthesis**, **routing**, **timing closure**, and finally prepare the **RISC-V SoC for tapeout readiness** 🚀

---

**🔗 Program Links:**

[![VSD Website](https://img.shields.io/badge/VSD-Official%20Website-blue?style=flat-square)](https://vsdiat.vlsisystemdesign.com/)  
[![RISC-V](https://img.shields.io/badge/RISC--V-International-green?style=flat-square)](https://riscv.org/)  
[![Efabless](https://img.shields.io/badge/Efabless-Platform-orange?style=flat-square)](https://efabless.com/)

**👨‍💻 Participant:** [VEERARAGAVAN7](https://github.com/VEERARAGAVAN7)
