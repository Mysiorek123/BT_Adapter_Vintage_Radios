# Bluetooth Adapter for Vintage Radios

This project presents the design and implementation of a specialized Bluetooth adapter aimed at modernizing vintage radio receivers, such as the Polish Unitra Zodiak, while preserving their unique acoustic character. The hardware features a multi-stage power supply and signal isolation architecture, utilizing a bridge rectifier, high-capacity filtering, and a PS2561 optoisolator to eliminate hum and ground loops. 


# I/O Pinouts Description

- ~AC - AC Input Voltage (6,3V)
- J1 - Separated 1,2V DC Input
- J2 - Separated 1,2V Ground
- J3 - Bluetooth Power Supply (VCC)
- J4 - Bluetooth Ground (GND)

# Schematic Diagram
<img width="1587" height="1119" alt="BT_Adapter Vintage Radios (2)" src="https://github.com/user-attachments/assets/6d8ca497-26d1-4c93-9097-23b49716d3ea" />

# PCB View

The physical implementation employs a double-sided PCB designed for a vertical "sandwich" stack configuration, ensuring full mechanical compatibility and efficient heat dissipation. 

<img width="715" height="704" alt="image (2)" src="https://github.com/user-attachments/assets/89832f5a-14a3-4b97-810d-935945937fe4" />
<img width="465" height="532" alt="image (3)" src="https://github.com/user-attachments/assets/7de62821-b84e-417f-9dbd-fb38a88adcd0" />

# Components()
| Reference  | Footprint | Qty | Value / Description|
| :--- | :--- | :-: | :--- |
| **1** | J2 | SolderWire-0.1sqmm_1x01_D0.4mm_OD1mm | 1 | BT_VCC | |
| **2** | J1 | SolderWire-0.1sqmm_1x01_D0.4mm_OD1mm | 1 | 1V2_SEPARATED | |
| **3** | J3 | SolderWire-0.1sqmm_1x01_D0.4mm_OD1mm | 1 | BT_GND | |
| **4** | B1 | Diode_Bridge_19.0x3.5x10.0mm_P5.0mm | 1 | B40C2300-1500A | |
| **5** | C2, C4 | C_Axial_L3.8mm_D2.6mm_P7.50mm_Horizontal | 2 | 100nF | |
| **6** | U2 | TO-220-3_Vertical | 1 | LM7805 | |
| **7** | R2 | R_Axial_DIN0207_L6.3mm_D2.5mm_P7.62mm_Horizontal | 1 | 10k | |
| **8** | C3 | CP_Radial_D6.3mm_P2.50mm | 1 | 220uF | |
| **9** | I1 | SolderWire-0.1sqmm_1x02_P3.6mm_D0.4mm_OD1mm | 1 | AC | |
| **10** | R1 | R_Axial_DIN0207_L6.3mm_D2.5mm_P7.62mm_Horizontal | 1 | 220 | |
| **11** | Q1 | TO-220-3_Vertical | 1 | IRF620N | |
| **12** | C1 | CP_Radial_D10.0mm_P5.00mm | 1 | 2200uF | |
| **13** | U1 | DIP-4_W7.62mm | 1 | PS2561 | |
