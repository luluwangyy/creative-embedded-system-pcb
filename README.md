# 🦆 The Duck 555 Timer Pendant

**A custom PCB pendant featuring a flashing LED integrated into a stylized duck form factor.**

![Final Board View](assets/final-outcome.gif)

Blog: https://www.notion.so/PCB-Design-and-Fabrication-3053158f0df780498474fec68f859eae?source=copy_link

## Project Overview
This project explores PCB fabrication as an artistic medium. The circuit is a standard astable multivibrator using a **TL555 timer chip**, designed to flash a red LED located at the duck's mouth/bill. The board is powered by a 3.7V coin cell battery.

The physical outline of the board is milled to resemble the side profile of a duck, experimenting with the idea of "playfulness" in hardware.


## Technical Specifications
* **Chip:** TL555 (Low power CMOS 555 timer)
* **Power Source:** 3V - 3.7V Coin Cell (CR2032 or similar)
* **Visual Output:** 1x Red LED (5mm)
* **Fabrication:** CNC Milled Copper Clad Board

## Bill of Materials (BOM)

| Component | Value/Type | Qty | Notes |
| :--- | :--- | :--- | :--- |
| U1 | TL555 | 1 | 8-pin DIP or SOIC |
| LED1 | Red LED | 1 | Placed at mouth coordinates |
| R1, R2 | 1kΩ - 100kΩ | 2 | Adjust for flash rate |
| C1 | 10µF | 1 | Electrolytic or Ceramic |
| Battery Holder | CR2032 SMT | 1 | Rear mount |

## Schematic & Design
The design files are located in the `assets/fabrication-files/` directory of this repository. 

**Reproduction Steps:**
1.  **Mill:** Use the provided Gerber files to mill the board outline and traces.
2.  **Solder:** Surface mount the battery holder on the back first.
3.  **Populate:** Solder the resistors and capacitor.
4.  **Finish:** Solder the TL555 and the LED. Ensure the LED polarity matches the "mouth" placement constraints.

---
*Created for [Course Name] - Spring 2026*