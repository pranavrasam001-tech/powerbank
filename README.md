# Mini Power Bank PCB Design

## About the project

i worked on this mini power bank pcb project using kicad to understand how a power bank circuit is designed and how its different parts work together

the board uses a TP4056 charging circuit, a DW01A battery protection circuit and a MIC2290 boost converter to provide a 5v output

the main idea was to build a simple charging and power supply circuit without using a microcontroller. during this project i worked on the circuit diagram, component selection, footprint assignment, pcb layout and routing. i also prepared the files needed for pcb manufacturing

## features

- usb type-c charging input
- support for a single-cell lithium-ion battery
- battery overcharge and over-discharge protection
- overcurrent protection
- 5v output through a boost converter
- separate charging and protection circuits
- compact pcb design
- no microcontroller required for basic operation
- designed using kicad

## tools and components used

### software

- kicad
- pcb fabrication tools for generating gerber and drill files
- autodesk fusion 360
  
### components

- TP4056 battery charging IC
- DW01A battery protection IC
- MIC2290 boost converter
- MOSFETs for battery protection
- usb type-c connector
- inductor
- resistors
- capacitors
- led
- battery connector

## what i worked on

- researched the components needed for a basic power bank circuit
- understood how the charging protection and voltage conversion sections work
- created the circuit diagram in kicad
- connected the TP4056 charging section to the battery
- added the DW01A protection circuit with external MOSFETs
- worked on the MIC2290 boost converter section
- assigned footprints to the components
- moved the components into the pcb editor
- arranged the components within the board outline
- started connecting the tracks between the components
- checked the component positions spacing and direction
- prepared the gerber drill and component placement files for manufacturing

## pcb design preview

### 1. circuit schematic


<img width="940" height="572" alt="circuit schematic" src="https://github.com/user-attachments/assets/22f606a3-df45-4cf5-be37-f27162d1e1dc" />

### 2. pcb layout


<img width="914" height="890" alt="pcb layout" src="https://github.com/user-attachments/assets/35912bad-8e66-4fab-8d97-bbe148f618d3" />

### 3. 3d pcb view


<img width="540" height="712" alt="3d pcb view" src="https://github.com/user-attachments/assets/f4a4ba90-cd7e-4703-b46b-48228823704b" />

## where this design can be used

this project helped me explore a few areas of electronics such as

- portable power supply circuits
- lithium-ion battery charging
- battery protection
- voltage conversion
- usb-powered devices
- power management
- pcb design and prototyping

## Bill of materials

the following table contains the components used in the pcb design along with their footprints and part details

| Designator | Value | Footprint | LCSC Part # | Type | Manufacturer | MPN | Order Qty (5 pcs) | Price (USD) |
|---|---|---|---|---|---|---|---:|---:|
| BT1 | Battery_Cell | BatteryHolder_Keystone_3000_1x12mm | C238097 | Extended | Keystone | 3000 | 5 | 1.709 |
| C3 | 100nF | C_0603_1608Metric | C14663 | Basic | YAGEO | CC0603KRX7R9BB104 | 5 | 0.042 |
| D1 | LED | LED_0603_1608Metric | C99290 | Extended | Lite-On | LTST-C191TBKT | 20 | 0.426 |
| J1 | USB_C_Receptacle_PowerOnly_6P | USB_C_Receptacle_HRO_TYPE-C-31-M-12 | C165948 | Extended | Korean Hroparts Elec | TYPE-C-31-M-12 | 5 | 0.934 |
| L1 | 10µH | L_Bourns_SRR1260 | C3221699 | Extended | BOURNS | SRR1260-100M | 5 | 4.6695 |
| Q1 | Q_NMOS_GSD | SOT-23-6 | C908265 | Extended | FUXINSEMI | FS8205A | 14 | 1.0038 |
| Q2 | Q_NMOS_GSD | SOT-23-6 | C908265 | Extended | FUXINSEMI | FS8205A |  |  |
| R1 | 5.1k | R_0603_1608Metric | C23186 | Basic | UNI-ROYAL | 0603WAF5101T5E | 10 | 0.015 |
| R2 | 5.1k | R_0603_1608Metric | C23186 | Basic | UNI-ROYAL | 0603WAF5101T5E |  |  |
| R3 | 2.2k | R_0603_1608Metric | C4190 | Basic | UNI-ROYAL | 0603WAF2201T5E | 5 | 0.009 |
| R4 | 1.2kΩ | R_0603_1608Metric | C22765 | Basic | UNI-ROYAL | 0603WAF1201T5E | 5 | 0.017 |
| R5 | 15k | R_0603_1608Metric | C22809 | Basic | UNI-ROYAL | 0603WAF1502T5E | 5 | 0.0145 |
| R6 | 4.99k | R_0603_1608Metric | C23046 | Basic | UNI-ROYAL | 0603WAF4991T5E | 5 | 0.0105 |
| R7 | 100Ω | R_0603_1608Metric | C22775 | Basic | UNI-ROYAL | 0603WAF1000T5E | 5 | 0.0115 |
| U1 | TP4056-42-ESOP8 | SOIC-8-1EP | C16581 | Extended | TOPPOWER | TP4056-42-ESOP8 | 5 | 0.9265 |
| U2 | DW01A | SOT-23-6 | C351410 | Extended | PUOLOP | DW01A | 9 | 0.4788 |
| U3 | MIC2290 | MLF-8-1EP | C144214 | Extended | Microchip Tech | MIC2290YML-TR | 5 | 8.455 |
| C1 | 2.2µF | C_0603_1608Metric | C9900011780 | Extended | JLCPCB Assembly | cap,2.2uF,+/-10%,25V,X5R,C0603 | 20 | 0.014 |
| C2 | 22µF | C_0805_2012Metric | C9900276340 | Extended | JLCPCB Assembly | 22uF 10V C-0805 | 9 | 0.3582 |

### estimated manufacturing cost

the following costs are from the manufacturing order details included in the original project file

| Description | Cost (USD) |
|---|---:|
| Components for 5 boards | 19.0943 |
| PCB fabrication for 5 boards | 4.00 |
| PCBA setup fee | 8.24 |
| PCBA stencil | 1.55 |
| PCBA components | 10.41 |
| Extended components fee | 9.27 |
| SMT assembly | 0.45 |
| Nitrogen reflow soldering | 0.91 |
| PCBA subtotal | 30.83 |
| PCB and PCBA total | 34.83 |
| Shipping | 9.83 |
| Coupon | -10.00 |
| **Order total** | **34.66** |

## safety considerations

since this project uses a lithium-ion battery it is important to check the circuit carefully before connecting the battery or applying power

things to check before testing

- make sure the battery polarity is correct
- check the battery voltage and charging limits
- verify the TP4056 charging connections
- check the DW01A protection circuit and MOSFET connections
- confirm the battery and output connections are correct
- check the MIC2290 component values and layout
- inspect the pcb for short circuits and incorrect connections
- test the charging and output sections carefully under controlled conditions

## cad design using autodesk fusion 360

along with the pcb design i also worked on creating an enclosure for the mini power bank using autodesk fusion 360

the idea was to make a small case that could hold the battery and pcb properly while leaving enough space for the charging port and led indicator

### what i designed

- **main enclosure:** created the main box with a base and side walls to hold the internal parts. i also added rounded edges to give it a cleaner look
- **internal base:** worked on the inside layout and added a small block to represent the battery position along with supports for the other components
- **component placement:** checked the available space to see how the battery and other parts would fit inside the enclosure
- **usb type-c opening:** added an opening on the side so the charging cable could be connected easily
- **led indicator opening:** created a small hole on the top so the led could be seen from outside
- **top cover:** designed a separate cover and checked how it fits with the main body

### software used

- autodesk fusion 360

### design progress

the basic enclosure and its main parts have been modelled. this includes the internal space battery placement component supports charging port opening led indicator hole and top cover

the imo note here was the base adn the lid are not attached and spearateld designed , i have uploaded the images related to this 
<img width="1117" height="778" alt="image" src="https://github.com/user-attachments/assets/dc7d2f56-db0b-43fb-8c8f-8a062ee0c3cd" />

### cad design preview

the following images show different parts of the enclosure designed in autodesk fusion 360

**1. main enclosure design**

**2. internal base and component placement**

**3. usb type-c charging port**

**4. led indicator opening**

**5. top cover and final assembly**

<img width="753" height="398" alt="main enclosure design" src="https://github.com/user-attachments/assets/0f5211ea-7811-46f0-9362-6e580edd5cb7" />

<img width="686" height="460" alt="enclosure design" src="https://github.com/user-attachments/assets/996aa8af-0c61-40c2-a029-b436873837e4" />
