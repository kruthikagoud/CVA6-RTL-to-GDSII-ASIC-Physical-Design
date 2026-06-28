# 📸 Project Outputs — Screenshot Gallery

This file documents every stage of the **CVA6 RISC-V Core — Synthesis-to-GDSII** flow, captured directly from the cloud EDA environment (Design Compiler + IC Compiler II).

---


## Screenshot 1 — Initial Floorplan: Macro Placement Overview

24 SRAM macros placed across the floorplan — `gen_256x45` and `gen_256x128` instruction/data SRAM banks on the left, `as_4x128 sram_bank[0–3]` banks on the right. This macro layout is what drove every congestion and density decision later in the flow.

![Screenshot 1 - Initial Floorplan](https://github.com/user-attachments/assets/d91399bf-91c3-443f-9a0f-388c2e538811)

---

## Screenshot 2 — Full-Chip Placement View

Zoomed-out view after standard cell placement, showing the relationship between the dense central cell region and the macro columns on either side.

![Screenshot 2 - Full-Chip Placement](https://github.com/user-attachments/assets/7fcfd9dd-3b3f-4112-9c06-66203aaf84b1)

---

## Screenshot 3 — Zoomed Floorplan View: PG Mesh / Routing Grid

A close-up of the power/ground mesh and routing grid set up during floorplanning in IC Compiler II.

![Screenshot 3 - PG Mesh Zoom](https://github.com/user-attachments/assets/a661432d-bcee-490b-80d5-77321bfb1c24)

---

## Screenshot 4 — Cell Density Heatmap (Issue Identified)

The congestion map shows the routing utilization of the CVA6 design following standard cell placement. Localized congestion is observed primarily near the left-central region of the core due to higher cell density and routing demand. 

![Screenshot 4 - Cell Density Heatmap](https://github.com/user-attachments/assets/744b36cb-199e-4c85-9eba-e73df391b342)

---

## Screenshot 5 — Channel Congestion Map (After Fix)

Congestion analysis after placement optimization showing a more balanced cell distribution and a noticeable reduction in routing hotspots compared to the initial placement. The improved placement enhances routability, minimizes congestion, and provides sufficient routing resources for the CTS and routing stages.

![Screenshot 5 - Congestion Map Clean](https://github.com/user-attachments/assets/827326be-48b5-427d-bead-732902acc695)

---


## Screenshot 6 — Clock Tree Synthesis: Buffer Levels

Clock tree structure showing the buffer/inverter stages from the clock root down to the leaf sinks — built out to **25 levels** to manage skew and insertion delay across the macro-heavy block.

![Screenshot 6 - CTS Buffer Levels](https://github.com/user-attachments/assets/57b192f4-b48b-46e7-8a0d-bcbfbe1d0d14)

---

## Screenshot 7 — Post-Route Layout (Detailed View)

Fully routed view, showing the complete metal stack (M1–M9, VIA1–VIA8) and standard cell instances after routing.

![Screenshot 7 - Post-Route Detail](https://github.com/user-attachments/assets/47119dcc-4687-4c86-8c21-f59cd9a6bc66)

---

## Screenshot 8 — Sign-off Report: Cell Count Summary

Final cell count summary of the CVA6 design after physical implementation. The design consists of **216,892 leaf cells**, including **193,338 combinational cells**, **23,554 sequential cells**, **42,023 buffer/inverter cells**, **325 integrated clock-gating cells**, and **24 macros**, reflecting the overall design complexity and optimization achieved during the ASIC implementation flow.

![Screenshot 8 - Cell Count Report](https://github.com/user-attachments/assets/6b7c98e6-fb4c-49cb-8e36-7c0aeaf6b4e0)

---

## Screenshot 9 — Sign-off Report: Area Summary

Final area utilization report showing the breakdown of standard-cell area, macro area, physical-only cell area, and total net length after successful routing and sign-off.

![Screenshot 9 - Area Report](https://github.com/user-attachments/assets/eb988d6c-8131-4395-a5ce-84013c081bb7)

---
## Screenshot 10 — Global Timing Report

The final timing report after post-route optimization indicates successful timing closure for the CVA6 design. The design achieved **zero register-to-register setup violations** and **no hold violations**, confirming reliable synchronous operation. The reported **WNS = -0.00 ns** and **TNS = -0.00 ns** correspond to a negligible numerical precision margin, effectively representing a timing-clean and signoff-ready implementation.

![Screenshot 10 - Global Timing Report](https://github.com/user-attachments/assets/a99e80f6-449d-4d0f-8af2-2baf6a1f975e)

---
## Screenshot 11 — Design Rule Violation (DRV) Summary

Final design rule verification report after sign-off optimization. The design reports **zero design rule violations**, including **0 max transition**, **0 max capacitance**, **0 min capacitance**, and **0 minimum pulse width** violations, confirming compliance with all electrical design constraints.

![Screenshot 11 - Design Rule Violation Summary](https://github.com/user-attachments/assets/d4f79a66-aa8c-4ddf-b21d-0d663abd6e52)

---
## Screenshot 12 — DRC Verification Report

The final physical verification confirms that the CVA6 design successfully meets the signoff verification requirements. A total of **221,856 nets** were extracted with **0 open nets**, ensuring complete connectivity throughout the design. The implementation achieved **0 Design Rule Check (DRC) violations**, **0 antenna violations**, and **0 DRC violations on Metal-3 and below**, demonstrating a clean, manufacturable, and signoff-ready physical layout.

![Screenshot 12 - DRC Verification Report](https://github.com/user-attachments/assets/b0642f98-f206-4ac3-88f3-cc97553900f1)

---
## Screenshot 13 — LVS / Connectivity Verification Report

Post-route verification results showing **222,348 input nets**, **0 short violations**, **0 open nets**, and **0 floating route violations**, confirming successful routing completion and a clean physical implementation. The displayed warnings are informational and do not affect design correctness.

![Screenshot 13 - LVS Verification Report](https://github.com/user-attachments/assets/3a0ea548-2aa2-4ce3-a64d-f388ebc4f90a)

---
## Screenshot 14 — Placement Legality Report

Final placement legality verification showing **0 overlap violations**, **0 spacing violations**, **0 cell-on-site violations**, **0 legal orientation violations**, and **0 PG DRC violations**. The design successfully satisfies all physical placement rules, confirming a legally placed and signoff-ready implementation.

![Screenshot 14 - Placement Legality Report](https://github.com/user-attachments/assets/6404acd8-2ede-4381-881d-d85f3b9707ad)

---

