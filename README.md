# Mini Power Bank PCB Design

## About the Project

I designed this Mini Power Bank PCB using KiCad to understand how a lithium-ion battery charging and power management circuit is designed from scratch. The board combines a TP4056 charging circuit, a DW01A battery protection circuit, and a MIC2290 boost converter to provide a nominal 5V output.

The design focuses on battery charging, protection, and voltage conversion without using a microcontroller. I worked on the schematic, component footprint assignment, PCB placement, routing, and preparation of manufacturing files.

## Features

* USB Type-C charging input
* Single-cell lithium-ion battery charging
* Battery overcharge and over-discharge protection
* Overcurrent protection through the battery protection circuit
* 5V output using a DC-DC boost converter
* Dedicated battery charging and protection ICs
* Compact PCB layout
* No microcontroller or firmware required for basic operation
* Designed using KiCad

## Tools and Components Used

**Software:**

* KiCad
* PCB fabrication tools for generating Gerber and drill files

**Components:**

* TP4056 lithium-ion battery charger
* DW01A battery protection IC
* MIC2290 boost converter
* MOSFETs for battery protection
* USB Type-C connector
* Inductor
* Resistors
* Capacitors
* LED
* Battery connector

## What I Did

* Researched the components required for a basic power bank circuit.
* Studied the functions of the battery charging, protection, and boost converter sections.
* Created the circuit schematic in KiCad.
* Connected the TP4056 charging circuit to the battery interface.
* Designed the DW01A battery protection section with external MOSFETs.
* Added the MIC2290 boost converter and its associated components.
* Assigned footprints to the schematic components.
* Transferred the components into PCB Editor.
* Arranged the components within the board outline.
* Started routing the PCB connections.
* Reviewed component placement, spacing, and orientation.
* Generated Gerber, drill, and component placement files for manufacturing.

## PCB Design Preview

### 1. Circuit Schematic

The schematic illustrates the battery charging circuit, protection network, and boost converter, along with their associated components and connections.

<img width="940" height="572" alt="image" src="https://github.com/user-attachments/assets/22f606a3-df45-4cf5-be37-f27162d1e1dc" />


### 2. PCB Layout

The PCB layout shows the component placement, copper tracks, and board arrangement.

<img width="914" height="890" alt="image" src="https://github.com/user-attachments/assets/35912bad-8e66-4fab-8d97-bbe148f618d3" />


### 3. 3D PCB View

The 3D view provides a visual representation of the board and helps review component orientation, spacing, connector placement, and mechanical arrangement.

<img width="540" height="712" alt="image" src="https://github.com/user-attachments/assets/f4a4ba90-cd7e-4703-b46b-48228823704b" />


## Applications

This design can serve as a starting point for learning and experimenting with:

* Portable power supply circuits
* Lithium-ion battery charging
* Battery protection systems
* DC-DC boost converters
* USB-powered electronic devices
* Power management circuit design
* PCB design and electronics prototyping

**Note:** The design must be electrically verified and the assembled board tested before it can be considered a working power bank. Actual output current and performance depend on the selected components, battery, thermal conditions, and PCB layout.

## What I Learned

Working on this project helped me understand how different power management circuits operate together.

I learned how to:

* Design a battery charging schematic.
* Understand lithium-ion battery protection using a dedicated protection IC and MOSFETs.
* Work with a DC-DC boost converter.
* Verify MOSFET gate, source, and drain connections.
* Check component pinouts and footprints against datasheets.
* Assign footprints and arrange components in KiCad.
* Route PCB tracks and review board connectivity.
* Use ERC and DRC to identify design issues.
* Generate manufacturing files for PCB fabrication.

## Bill of Materials (BOM)

| Designator | Value | Footprint | LCSC Part # | Type | Manufacturer | MPN | Order Qty (5 pcs) | Price (USD) | X (mm) | Y (mm) | Rot |
|---|---|---|---|---|---|---|---|---|---|---|---|
| BT1 | Battery_Cell | BatteryHolder_Keystone_3000_1x12mm | C238097 | Extended | Keystone | 3000 | 5 | 1.709 | 152.2 | -102.8 | 0.0 |
| C3 | 100nF | C_0603_1608Metric | C14663 | Basic | YAGEO | CC0603KRX7R9BB104 | 5 | 0.042 | 147.9375 | -118.8 | 90.0 |
| D1 | LED | LED_0603_1608Metric | C99290 | Extended | Lite-On | LTST-C191TBKT | 20 | 0.426 | 126.275 | -121.0025 | 90.0 |
| J1 | USB_C_Receptacle_PowerOnly_6P | USB_C_Receptacle_HRO_TYPE-C-31-M-12 | C165948 | Extended | Korean Hroparts Elec | TYPE-C-31-M-12 | 5 | 0.934 | 134.11 | -97.2 | 180.0 |
| L1 | 10µH | L_Bourns_SRR1260 | C3221699 | Extended | BOURNS | SRR1260-100M | 5 | 4.6695 | 137.2 | -133.8 | 0.0 |
| Q1 | Q_NMOS_GSD | SOT-23-6 | C908265 | Extended | FUXINSEMI | FS8205A | 14 | 1.0038 | 157.6625 | -126.4 | 0.0 |
| Q2 | Q_NMOS_GSD | SOT-23-6 | C908265 | Extended | FUXINSEMI | FS8205A |  |  | 150.4625 | -126.4 | 0.0 |
| R1 | 5.1k | R_0603_1608Metric | C23186 | Basic | UNI-ROYAL(Uniroyal Elec) | 0603WAF5101T5E | 10 | 0.015 | 131.9 | -120.59 | 0.0 |
| R2 | 5.1k | R_0603_1608Metric | C23186 | Basic | UNI-ROYAL(Uniroyal Elec) | 0603WAF5101T5E |  |  | 131.6 | -105.4 | 0.0 |
| R3 | 2.2k | R_0603_1608Metric | C4190 | Basic | UNI-ROYAL(Uniroyal Elec) | 0603WAF2201T5E | 5 | 0.009 | 126.075 | -115.19 | 90.0 |
| R4 | 1.2kΩ | R_0603_1608Metric | C22765 | Basic | UNI-ROYAL(Uniroyal Elec) | 0603WAF1201T5E | 5 | 0.017 | 141.875 | -113.565 | 90.0 |
| R5 | 15k | R_0603_1608Metric | C22809 | Basic | UNI-ROYAL(Uniroyal Elec) | 0603WAF1502T5E | 5 | 0.0145 | 148.3 | -139.075 | 90.0 |
| R6 | 4.99k | R_0603_1608Metric | C23046 | Basic | UNI-ROYAL(Uniroyal Elec) | 0603WAF4991T5E | 5 | 0.0105 | 155.5 | -139.825 | 90.0 |
| R7 | 100Ω | R_0603_1608Metric | C22775 | Basic | UNI-ROYAL(Uniroyal Elec) | 0603WAF1000T5E | 5 | 0.0115 | 126.75 | -134.225 | 90.0 |
| U1 | TP4056-42-ESOP8 | SOIC-8-1EP_3.9x4.9mm_P1.27mm_EP2.41x3.3mm_ThermalVias | C16581 | Extended | TOPPOWER(Nanjing Extension Microelectronics) | TP4056-42-ESOP8 | 5 | 0.9265 | 134.475 | -114.765 | 0.0 |
| U2 | DW01A | SOT-23-6 | C351410 | Extended | PUOLOP | DW01A | 9 | 0.4788 | 154.5375 | -118.6 | 0.0 |
| U3 | MIC2290 | Micrel_MLF-8-1EP_2x2mm_P0.5mm_EP0.8x1.3mm_ThermalVias | C144214 | Extended | Microchip Tech | MIC2290YML-TR | 5 | 8.455 | 152.3 | -135.65 | 0.0 |
| C1 | 2.2µF | C_0603_1608Metric | C9900011780 | Extended | JLCPCB Assembly | cap,2.2uF,+/-10%,25V,X5R,C0603 | 20 | 0.014 | 128.475 | -112.215 | 90.0 |
| C2 | 22µF | C_0805_2012Metric | C9900276340 | Extended | JLCPCB Assembly | 22uF 10V C-0805 | 9 | 0.3582 | 157.0 | -134.8 | 90.0 |
| **Parts total - JLCPCB BOM match (5 boards)** | | | | | | | | **19.0943** | | | |
| **PCB (5 pcs, 2 layers, 1.6mm, HASL with lead, green)** | | | | | | | | **4.00** | | | |
| **PCBA setup fee** | | | | | | | | **8.24** | | | |
| **PCBA stencil** | | | | | | | | **1.55** | | | |
| **PCBA components (11 items)** | | | | | | | | **10.41** | | | |
| **PCBA extended components fee** | | | | | | | | **9.27** | | | |
| **PCBA SMT assembly** | | | | | | | | **0.45** | | | |
| **PCBA nitrogen reflow soldering** | | | | | | | | **0.91** | | | |
| **PCBA subtotal (economic, top side)** | | | | | | | | **30.83** | | | |
| **Merchandise total (PCB + PCBA)** | | | | | | | | **34.83** | | | |
| **Shipping** | | | | | | | | **9.83** | | | |
| **Coupon** | | | | | | | | **-10.00** | | | |
| **Order subtotal** | | | | | | | | **34.66** | | | |

## Firmware Requirements

This design does not require firmware because the TP4056, DW01A, and MIC2290 perform their functions through dedicated hardware circuitry.

A microcontroller would only be required if additional programmable features were introduced, such as a digital battery percentage display, software-based monitoring, or programmable power management.

## Project Status

The schematic and PCB design have been developed in KiCad, and manufacturing files have been generated.

Further verification is required to confirm all component connections, footprints, battery protection functions, boost converter operation, and PCB design rules before fabrication and testing.

## Safety Considerations

Lithium-ion batteries require correct charging limits, suitable protection circuitry, and proper electrical connections.

Before powering the circuit:

* Verify the battery polarity and voltage ratings.
* Check the TP4056 charging configuration.
* Verify the DW01A sensing network and MOSFET connections.
* Confirm that battery negative and protected output negative follow the intended protection topology.
* Check the MIC2290 component values and layout recommendations.
* Inspect the PCB for shorts and incorrect connections.
* Test the charging and output stages under controlled conditions.

Do not connect a battery or valuable electronic device until the circuit has been reviewed and checked for faults.


```

The folder structure is a suggested organization for the project repository. Update the filenames and folders to match the files actually included in the repository.
