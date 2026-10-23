# date:21/10
# time spent:2hrs
## description:
i started by planning a small power bank that could charge through usb c and provide a stable 5v output. i researched the components needed for charging, battery protection and voltage boosting, and selected the tp4056, dw01a, mic2290 and other required components. i divided the schematic into separate sections to make the design easier to understand. at first, i found it difficult to understand how the components should be connected, especially the battery negative and protected ground connections. i also learned that checking datasheets is important to understand pin connections, component sizes and current limits before starting the circuit design.

------

# date:21/10
# time spent:2hrs
## description:
i started working on the usb c input and added 5.1k resistors to both cc1 and cc2. then i created the tp4056 charging circuit with the 5v input, battery connection, charging resistor and led indicator. i also connected the ground and exposed pad and checked the temp and standby pins. while working on this part, i learned how the charging circuit is connected and why each component is needed.
## Images
<img width="406" height="376" alt="image" src="https://github.com/user-attachments/assets/2b7fd660-f125-4aed-b8b0-0bfaa9f00324" />
<img width="290" height="190" alt="image" src="https://github.com/user-attachments/assets/19433eae-59ff-4f20-afa8-00203e7a994b" />
<img width="415" height="329" alt="image" src="https://github.com/user-attachments/assets/c43214c7-c7d4-4664-804f-32c09f8ca788" />

------

# date:21/10
# time spent:2hrs
## description:
i checked the errors in the charging circuit and used the erc tool to find the connections that needed attention. i also learned that the prog resistor controls the charging current and that the tp4056 can get hot while charging. after that, i added the mic2290 boost converter with a 10uh inductor, capacitors and resistors to get around 5v output. i also added the battery, dw01a protection ic and two mosfets for battery protection. while connecting everything, i had some confusion with the ground connections and mosfet pins, so i checked the net labels and component datasheets to understand the connections better.
## Images
<img width="613" height="390" alt="image" src="https://github.com/user-attachments/assets/84381533-af40-4f3c-bc32-4c567159be65" />
<img width="940" height="606" alt="image" src="https://github.com/user-attachments/assets/45868f35-52b7-4cac-a70c-c214271c8bcf" />

------

# date:22/10
# time spent:2hrs
## description:
the main difficulty was checking the mosfet gate source and drain connections and completing the dw01a sensing network i also had to make sure that batt minus was not directly connected to p minus i used erc to find missing connections and learned that checking the datasheets is also important because a clean erc report does not always mean the circuit is correct
## Images
<img width="940" height="291" alt="image" src="https://github.com/user-attachments/assets/3402d392-7c57-4e16-a113-31c840c2d470" />
<img width="940" height="572" alt="image" src="https://github.com/user-attachments/assets/f50349d6-8e2b-4675-8ca8-8c60ae5f84b6" />

------

# date:22/10
# time spent:1hr
## description:
after completing the schematic i started assigning footprints to the components in kicad i checked the footprints for resistors capacitors the led usb c connector charger protection ic boost converter inductor and battery connection i also checked the package sizes and moved the components into pcb editor where i started arranging them inside the board outline
## Images
<img width="940" height="892" alt="image" src="https://github.com/user-attachments/assets/e81f0e41-f352-4956-884e-439b3dc5faa3" />

------

# date:22/10
# time spent:1.5hrs
## description:
i arranged the components on the pcb by keeping the usb c connector near the charging circuit and placing the protection ic with its mosfets i also grouped the mic2290 with the inductor and capacitors then i started routing the connections and checked the 3d view to see the component positions spacing and overall board layout
## Images
<img width="689" height="820" alt="image" src="https://github.com/user-attachments/assets/c79d6a83-1a84-4372-b88e-9402ed17b462" />

------

# date:22/10
# time spent:2hrs
## description:
the pcb still needed some work because a few connections were not routed and the layout was not fully complete i planned to finish the routing check all the footprints and protection connections fix the remaining schematic and erc issues and run drc to check track widths clearances and any unconnected nets before sending the board for fabrication
## Images
<img width="914" height="890" alt="image" src="https://github.com/user-attachments/assets/9036501c-5119-4c6c-a3e3-c526ef8ddb24" />
