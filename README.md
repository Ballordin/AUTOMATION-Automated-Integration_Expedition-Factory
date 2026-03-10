# Integrated Production, Assembly & Expedition Factory 🏭

## 📖 Project Overview

This project focuses on the design and implementation of an automated flexible manufacturing system (FMS). It simulates a complete industrial cycle: from raw material sorting and CNC machining to part assembly (bases and lids) and final warehouse expedition.

The system was developed using a Digital Twin approach, where the control logic was tested in a 3D simulated environment (Factory I/O) before being interfaced with physical industrial hardware.

## 🛠️ Tech Stack

PLC: Omron NX1P2 (Programmed via Sysmac Studio).

HMI: Omron NB7W-TW01B (Designed via NB Designer).

Simulation: Factory I/O (Real-time 3D Industrial Simulator).

Communication: Ethernet/IP protocol.

Control Logic: Grafcet (SFC) for sequential flow and Ladder Logic for safety/interlocking.

## ⚙️ Functional Stages

The factory is divided into several automated cells:

Sorting & CNC: The system identifies raw materials (Green, Blue, or Metal) and feeds them into a CNC Machining Center.

Part Assembly (Integration): The machined "bases" are paired with the correct "lids" using automated Pick-and-Place grippers.

Warehousing: Finished parts are moved to a high-bay warehouse via a stacker crane (transloelevador).

Expedition: Through the HMI, an operator can request specific parts from the warehouse to be delivered to the expedition bay.

## 🖥️ HMI Interface

The HMI provides the operator with:

Real-time Monitoring: Status of every sensor and actuator.

System Control: Start, Stop and Reset.

Order Management: A dedicated screen to select which part color/type to expedite from the warehouse.

## 📂 Repository Structure

/plc_programming: Sysmac Studio project files (.smc2).

/hmi_design: NB Designer project files for the Omron HMI.

/simulation: Factory I/O scene file.

/docs: Contains the Pre-Project Report (initial planning) and the Final Technical Report.

/media: Video demonstrations and screenshots of the HMI/Logic.

## 👥 Author
Tiago Oliveira

## How to use these files:
Logic: Open the ProjetoFinal.smc2 in Sysmac Studio to view the Ladder and Grafcet logic.

HMI: Open the .nbp file in NB Designer to view or edit the interface.

Simulation: Open the .factoryio file. Ensure the driver is set to "OPC UA" or "Omron Ethernet/IP" to connect with the PLC.
