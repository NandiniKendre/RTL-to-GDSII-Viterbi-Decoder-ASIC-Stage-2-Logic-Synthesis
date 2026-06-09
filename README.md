# RTL-to-GDSII-Viterbi-Decoder-ASIC

## Stage 2: Logic Synthesis

### Overview

This repository documents the **Logic Synthesis** stage of the ASIC implementation flow for a **K=7 Convolutional Encoder and Viterbi Decoder**. After successful RTL behavioral verification, the design was synthesized using a TCL-driven synthesis flow to generate a technology-mapped gate-level netlist targeting a standard-cell library.

The objective of this stage is to transform the verified RTL design into an optimized gate-level representation while evaluating timing, area, and power characteristics required for downstream physical design stages.

---

## Design Specifications

* Constraint Length (K): 7
* Convolutional Code: (171,133) Octal
* Number of States: 64
* Architecture: Sequential Input / Sequential Output (SISO)
* RTL Language: Verilog HDL
* Target Flow: ASIC Implementation

---

## Synthesis Flow

The synthesis process included:

* RTL analysis and elaboration
* Constraint application using TCL scripts
* Logic optimization
* Technology mapping
* Gate-level netlist generation
* Timing analysis
* Area estimation
* Power estimation

---

## Generated Outputs

### Gate-Level Netlist

Technology-mapped netlist generated from the RTL design.

### Timing Report

Analysis of critical paths, setup timing, and overall timing performance.

### Area Report

Summary of standard-cell utilization and total synthesized area.

### Power Report

Estimation of dynamic, internal, and leakage power consumption.

---

## Repository Structure

```text
├── RTL/
├── Constraints/
│   └── synth.tcl
├── Netlist/
│   └── viterbi_k7_synth.v
├── Reports/
│   ├── timing.rpt
│   ├── area.rpt
│   └── power.rpt
└── README.md
```

---

## Deliverables

* TCL Synthesis Script
* Synthesized Gate-Level Netlist
* Timing Report
* Area Report
* Power Report

---

## Results

✅ RTL successfully synthesized

✅ Technology mapping completed

✅ Gate-level netlist generated

✅ Timing analysis completed

✅ Area analysis completed

✅ Power estimation completed

---

## ASIC Flow Progress

```text
RTL Behavioral Simulation & Functional Verification   ✅ Completed
Logic Synthesis                                       ✅ Completed
Gate-Level Simulation                                 ⏳ Next Stage
Floorplanning                                         ⏳ Pending
Placement                                             ⏳ Pending
Clock Tree Synthesis (CTS)                            ⏳ Pending
Routing                                               ⏳ Pending
Static Timing Analysis (STA)                          ⏳ Pending
DRC/LVS Verification                                  ⏳ Pending
GDSII Generation                                      ⏳ Pending
```

### Status

**Stage 2 Completed Successfully – Design Ready for Gate-Level Simulation and Physical Design Flow.**
