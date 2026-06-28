# 🚀 CVA6 RTL-to-GDSII ASIC Physical Design (64-bit RISC-V Processor)

> Complete RTL-to-GDSII implementation of the CVA6 64-bit RISC-V processor using Synopsys Design Compiler (DC Shell) and Synopsys IC Compiler II (ICC2).

---

# 📌 Project Overview

The **CVA6 (formerly Ariane)** is an open-source, 64-bit, 6-stage in-order RISC-V processor designed for high-performance embedded and SoC applications.

This project demonstrates the complete **ASIC Physical Design Flow** starting from RTL synthesis and ending with a signoff-ready GDSII layout. The implementation was carried out using industry-standard Synopsys EDA tools while performing timing optimization, congestion reduction, clock tree synthesis, routing, physical verification, and timing closure.

---

# 🎯 Project Objectives

- Perform RTL synthesis using Synopsys Design Compiler
- Develop and validate SDC timing constraints
- Complete the full ASIC Physical Design flow
- Achieve timing closure
- Minimize routing congestion
- Generate a DRC-clean and signoff-ready layout

---

# 🔄 ASIC Design Flow

```
RTL
   │
   ▼
Logic Synthesis
   │
   ▼
Floorplanning
   │
   ▼
Power Planning
   │
   ▼
Macro Placement
   │
   ▼
Standard Cell Placement
   │
   ▼
Clock Tree Synthesis (CTS)
   │
   ▼
Routing
   │
   ▼
Post Route Optimization
   │
   ▼
Static Timing Analysis (STA)
   │
   ▼
Physical Verification
   │
   ▼
GDSII Generation
```

---

# 🚀 Key Features

- RTL Synthesis using Synopsys Design Compiler
- QoR Analysis
- SDC Constraint Development
- Floorplanning
- Power Planning
- Macro Placement
- Standard Cell Placement
- Congestion Optimization
- Clock Tree Synthesis (CTS)
- Detailed Routing
- Post-Route ECO Optimization
- Static Timing Analysis (STA)
- Timing Closure
- Physical Verification
- GDSII Generation

---

# 🛠️ Tools & Environment

| Tool | Purpose |
|-------|----------|
| Verilog HDL | RTL Design |
| Synopsys Design Compiler | Logic Synthesis |
| Synopsys IC Compiler II | Physical Design |
| Tcl | Design Automation |
| Static Timing Analysis | Timing Verification |
| Red Hat Enterprise Linux | Development Environment |

---

# 📂 Repository Contents

| Folder | Description |
|----------|-------------|
| Images | Floorplan, CTS, Routing, Timing and Layout Screenshots |
| Reports | Timing, QoR, DRC, Area and Power Reports |
| Constraints | SDC Constraint Files |
| TCL_Scripts | Physical Design Automation Scripts |
| Layout | Final GDSII Layout |
| Documentation | Project Report |

---

# 📊 Physical Design Stages

## RTL Synthesis

- RTL synthesized using Synopsys Design Compiler
- Generated optimized gate-level netlist
- Timing constraints applied through SDC
- QoR reports analyzed for area, power, and timing

---

## Floorplanning

- Core utilization defined
- Macro placement optimized
- Placement blockages inserted
- Pin placement completed
- Power planning initialized

---

## Placement

- Standard cell placement completed
- Congestion analyzed
- Cell density optimized
- Placement legality verified

---

## Clock Tree Synthesis (CTS)

- Clock buffers inserted
- Clock skew minimized
- Clock latency balanced
- CTS optimization completed

---

## Routing

- Global routing
- Detailed routing
- Route optimization
- ECO routing
- Routing congestion minimized

---

## Static Timing Analysis

- Setup analysis
- Hold analysis
- Transition analysis
- Capacitance analysis
- Pulse width verification

---

## Physical Verification

- Design Rule Check (DRC)
- Route Verification
- Antenna Verification
- Open Net Verification
- Short Verification
- Layout Legality Check

---

# 📈 Final Results

| Parameter | Status |
|------------|---------|
| Setup Timing | ✅ Closed |
| Hold Timing | ✅ No Violations |
| DRC | ✅ 0 Violations |
| Antenna Violations | ✅ 0 |
| Open Nets | ✅ 0 |
| Short Violations | ✅ 0 |
| Floating Routes | ✅ 0 |
| Max Transition Violations | ✅ 0 |
| Max Capacitance Violations | ✅ 0 |
| Minimum Pulse Width Violations | ✅ 0 |
| Physical Legality | ✅ Passed |
| Signoff Status | ✅ Ready |

---

# 📸 Project Gallery

The repository includes screenshots of:

- Cell Density Map
- Floorplan
- Macro Placement
- Standard Cell Placement
- Clock Tree
- Routing
- Timing Reports
- DRC Reports
- Final Layout
- Physical Verification

---

# ⚠ Challenges Faced

### 1. Timing Closure

Achieving setup timing closure required detailed timing path analysis, driver upsizing, buffer insertion, and multiple post-route ECO optimization iterations while maintaining clean hold timing.

### 2. Congestion Optimization

Macro placement and routing congestion were minimized through floorplan refinement, placement optimization, CTS balancing, and routing optimization, resulting in a DRC-clean and signoff-ready layout.

---

# 📚 Skills Demonstrated

- ASIC Physical Design
- RTL-to-GDSII Flow
- RISC-V Processor Implementation
- Static Timing Analysis (STA)
- Floorplanning
- Power Planning
- Placement
- Clock Tree Synthesis
- Routing
- Timing Closure
- DRC Verification
- Physical Verification
- Tcl Scripting
- Verilog HDL
- Synopsys Design Compiler
- Synopsys IC Compiler II

---

# 👩‍💻 Author

**Bombothula Kruthika Goud**

Electronics & Communication Engineering

Aspiring ASIC Physical Design Engineer

LinkedIn: https://www.linkedin.com/in/kruthikabombothula/

GitHub: https://github.com/kruthikagoud

---

## ⭐ If you found this project interesting, consider giving it a Star!
