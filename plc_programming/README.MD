# PLC Programming (Sysmac Studio)

This folder contains the control logic for the **Omron NX1P2 PLC**.

## Logic Structure
The program is organized into functional tasks using **Grafcet (SFC)** for sequential control and **Ladder Diagram (LD)** for safety interlocks and I/O mapping.

### Main Control Loops:
* **Initial Sorting:** Logic to differentiate between Raw Material (Green, Blue, Metal) and LIDs.
* **CNC Management:** Handles the handshake between the conveyor and the CNC Machining Center.
* **Assembly (Integration):** Controls the Pick-and-Place sequence to merge bases and lids.
* **Warehouse & Expedition:** Manages the stacker crane (transloelevador) and retrieves parts based on HMI requests.

> **Software Requirement:** Sysmac Studio v1.40 or higher.
