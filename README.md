# Memory Controller Verification using UVM

## Overview
This project implements a **UVM-based verification environment** for a
SystemVerilog **Memory Controller** supporting read and write operations.
The objective is to demonstrate a **clean UVM architecture**, proper
transaction flow, and functional checking suitable for entry-level VLSI
verification roles.

---

## Design Under Test (DUT)
- 64K × 32-bit Memory Controller
- Supports READ and WRITE commands
- Synchronous design with FSM-based control
- Written in synthesizable SystemVerilog

---

## Verification Methodology
The verification environment is developed using **Universal Verification Methodology (UVM)** and follows an industry-standard structure.

### UVM Components Implemented
- **Transaction** – Defines memory read/write transactions
- **Sequence & Sequencer** – Generates different stimulus patterns
- **Driver** – Drives transactions to the DUT via interface
- **Monitor** – Samples DUT signals and converts them to transactions
- **Agent** – Encapsulates driver, monitor, and sequencer
- **Scoreboard** – Performs functional checking of read/write data
- **Environment** – Integrates agent and scoreboard
- **Test** – Controls simulation and executes sequences

---

## Directory Structure
