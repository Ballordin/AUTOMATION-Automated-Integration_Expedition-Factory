# Digital Twin Simulation (Factory I/O)

The entire production line was modeled and simulated in **Factory I/O** to validate the PLC logic.

## Features
* **Industrial Sensors:** Uses diffuse, retro-reflective, and vision sensors for part detection.
* **Actuators:** Includes 3-axis Pick-and-Place robots, heavy-duty conveyors, and a CNC unit.
* **Communication:** Connected to Sysmac Studio via **Ethernet/IP**.

### How to Run:
1. Open the `.factoryio` file.
2. Go to `File > Drivers`.
3. Select the **Omron Ethernet/IP** driver and ensure the IP matches your Sysmac configuration.
