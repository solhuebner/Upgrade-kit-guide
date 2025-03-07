[E4_STARTGCODE]: https://github.com/ZONESTAR3D/Slicing-Guide/blob/master/PrusaSlicer/Custom_Gcode.md#start-g-code
[M4_MIXMULTICOLORPRINT]: https://github.com/ZONESTAR3D/Slicing-Guide/blob/master/PrusaSlicer/PrusaSlicerGuide_M4.md#how-to-print-more-than-4-colors-using-m4-hot-end
[E4_TOOLCHANGE]: https://github.com/ZONESTAR3D/Slicing-Guide/blob/master/PrusaSlicer/Custom_Gcode.md#tool-change-g-code
[FW_Z9V5]: https://github.com/ZONESTAR3D/Firmware/tree/master/Z9/Z9V5/bin
[FW_Z9M4]: https://github.com/ZONESTAR3D/Firmware/tree/master/Z9/Z9M4
[FW_Z8P]: https://github.com/ZONESTAR3D/Firmware/tree/master/Z8/Z8P

----
## <a id="choose-language">:globe_with_meridians: Choose language </a>
[![](../lanpic/EN.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/FAQ_M4E4.md)
[![](../lanpic/ES.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/FAQ_M4E4-es.md)
[![](../lanpic/PT.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/FAQ_M4E4-pt.md)
[![](../lanpic/FR.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/FAQ_M4E4-fr.md)
[![](../lanpic/DE.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/FAQ_M4E4-de.md)
[![](../lanpic/IT.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/FAQ_M4E4-it.md)
[![](../lanpic/RU.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/FAQ_M4E4-ru.md)
[![](../lanpic/JP.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/FAQ_M4E4-jp.md)
[![](../lanpic/KR.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/FAQ_M4E4-kr.md)
<!-- [![](../lanpic/SA.png)](https://github.com/ZONESTAR3D/Upgrade-kit-guide/tree/main/HOTEND/FAQ_M4E4-ar.md) -->

----
# FAQ for E4 and M4 hotend
- [**What's the different between E4 and M4 hotend?**](#a1)
- [**Which type of hotend should I choose?**](#a2)
- [**How to load filaments into the hotend correctly?**](#a3)
- [**What is the difference in slicing settings between M4 and E4 hotends**](#a4)
- [**How to switch between M4 and E4 hotend?**](#a5)


-----
## <a id="a1">What's different between E4 and M4 hotend?</a>
![](./M4V6vsE4.jpg)   
- **M4 hotend** can mix different colored filaments to produce new colored filaments. **E4 hotend** does not have this ability.  
- **E4 hotend** is good at printing one color or multi color 3d object (up to 4 color).
- **M4 hotend** is good at printing gradient color 3d object, it can print more than 4 colos 3d object too (by mixing the filaments).
### Working principle of E4 hotend
![](./E4/User_guide/E4_principle.gif)
### Working principle of M4 hotend
[](https://github.com/ZONESTAR3D/Document-and-User-Guide/assets/29502731/2b9f4d75-b6fd-486f-aaa7-7a1163383316)

### Advantages of E4 hotend
1. Smaller "extruder switch prime tower" while printing multi color 3d object.
2. Better quality when printing one color 3d object.
3. Support to print different type of filament on the same 3d object.
### Advantages of M4 hotend
1. Support mixing different color filaments to new colors.
2. Support gradient color printing.
3. Support higher flow rate.
![](M4VSE4.jpg)

-----
## <a id="a2"> Which hotend should I choose, M4 or E4?</a>
- If you **do not need** to print gradient color 3d model, we suggest you choose **E4 hotend**, it can get better quality on printing single color and multi colors 3d prints.
- If you want to print **gradient color** 3d model, or you want to **mix different color filaments to another color**, choose M4 hotend.

-----
## <a id="a3"> How to load/unload filaments correctly</a>
M4 hot end and E4 hot end have different requirements for loading filament. 
- **Requirements of quantity for loading filaments:**
  - The M4 hot end requires four filaments to be loaded at the same time, regardless of whether printing single color or multi-color; 
  - The E4 hot end can choose the number of filaments to load according to the colors printed.   
- **Requirements of position for loading filaments:**
  - The M4 hot end requires the filament to be installed at the bottom of the hot end; 
  - The E4 hot end requires the filament to be installed above the funnel mouth of the hot end (extending the PTFE tube by about 20mm).
### For M4 Hotend
#### Steps to load filaments into the M4 hotend:
##### [![](https://img.youtube.com/vi/-47yB95uIxI/0.jpg)](https://www.youtube.com/watch?v=-47yB95uIxI)
When loading the filaments into the M4 hotend, regardless of how many extruders you need to use during printing, ***all four filaments must be loaded into the hotend***, and it is important to  ***ensure that all filaments are loaded into the bottom of the hotend*** before starting printing.     
:warning: ***Whether printing in single color or multi-color, you need to load all four filaments into the M4V6 hotend.***     
1. Cut the front of the filament with diagonal pliers before loading it to the extruder and hotend.
2. Load 4 filaments to all extruders one by one and then rotate the gear of the extruders until the filament enter to the inner PTFE tube of hotend, rotate more 4 ~ 5 turn and then stop.     

#### Steps to unload filament from the M4 hotend:
1. Heating the nozzle (200℃ for PLA / 230℃ for PETG/ABS) and wait for the temperature to reach. ***Menu: Prepare>>Filament>>Preheat: 200/230***
2. Feed filaments at least 10mm on all 4 channels simultaneously. ***Menu: Prepare>>Filament>>Extruder: All; Prepare>>Filament>>Slowly Load***
3. Unload filaments from the hotend. ***Menu: Prepare>>Filament>>Slowly unload***    

### For E4 Hotend
#### <a id = "PRELOAD_FILAMENT">Steps to load filaments into the E4 hotend:</a>
##### [![](https://img.youtube.com/vi/FyHrAMytlT8/0.jpg)](https://www.youtube.com/watch?v=FyHrAMytlT8)
If you understand the working principle of the E4 hotend, you should already know that when printing multi-color, the machine first needs to unload the previously loaded filament from the hotend and then load the next filament. However, usually ***the machine does not have the ability to recognize the distance between the front end of the filament and the nozzle before starting printing***. Therefore, we need to set up a process called <u>***"pre-load filaments"***</u>, which aims to allow the machine to move the fine threads to a suitable position known to the machine before printing the object.      
:warning: ***Only the filaments on the extruder that need to be used in the gcode file need to be loaded into the E4 hotend.***      

### Steps to unload filament from the E4 hotend:
1. Heating the nozzle (200℃ for PLA / 230℃ for PETG/ABS). ***Menu: Prepare>>Filament>>Preheat: 200/230***
2. Feed filament at least 10mm on the used extruder. ***Menu: Prepare>>Filament>>Extruder: 1/2/3/4; Prepare>>Filament>>Slowly Load***
3. Unload filament from the hotend. ***Menu: Prepare>>Filament>>Slowly unload***

-----
## <a id = "a4">What is the difference in slicing settings between M4 and E4 hotend:</a>
:pushpin: These settings have been set in the profiles of the PrusaSlicer software we provide. You only need to choose the correct **printer preset** according to your machine and hotend type.
### Slice settings for multi-color printing    
For printing multi-color, the slicing settings for the E4 hotend and M4 hotend mainly differ as follows:
- **start gcode**
  - **For the E4 hotend**, it requires "pre-load filaments" before starting printing([**Know Why**](#PRELOAD_FILAMENT)), for details, please refer to [**start gcode of the E4 hotend**][E4_STARTGCODE].     
  - **For the M4 hotend**, When printing no more than 4 colors, there is no need to make special changes to the start gcode. But **if you need to print more than 4 colors** (mixing different colored filaments into multiple colors), you can set the color mixing ratio in the start gcode. For details, please refer to [**How to print more than 4 colors by using M4 hot end**][M4_MIXMULTICOLORPRINT].
- **Retraction settings of the Extruders**
  - **For the E4 hotend**, the recommended **Retraction length** is 6 ~ 8mm (must be less than 10mm).
  - **For the M4 hotend**, the recommended **Retraction length** is 8 ~ 15mm.
- **Wipe Tower (Prime Tower)**     
:pushpin: The slicing software that supports multiple extruder printers has an **"Wipe Tower(Prime Tower)"** option. Because when the printer switches from one extruder to another, it often needs to first clean the fine threads of the previous color in the hot end. After turning on the erase tower option, the slicing software can generate an "additional" print in the gcode file to clean up any remaining filaments in the hot end.
  - **For the E4 hotend**, the required volume of the wire tower is relatively small.
  - **For the M4 hotend**, the required volume of the wire tower is relatively big.
- **Tool change G-code**
  - **For the E4 hotend**, when switching the extruder, it is necessary to pull out the previous color filament from the hotend and then load the next color filament to the hotend. Therefore, Tool Change Gcode needs to be set to achieve this operation. For deltails, please refer to [**Tool change G-code for E4 hotend**][E4_TOOLCHANGE].
  - **For the M4 hotend**, it doesn't need **Tool change G-code**.

-----
## <a id="a5"> How to switch between M4 hotend and E4 hotend</a>
### 1. Loosen the three screws on the hotend housing and remove the old hotend from the machine (x pulley). Then install the new hotend on the machine (x pulley) and lock the screws.
![](./E4/User_guide/E4-4.jpg)
### 2. Connect the wires of the new hotend to the machine.
![](./E4/User_guide/wiring1.jpg) ![](./E4/User_guide/wiring2.jpg)
### 3. Set the hotend type on the LCD menu: *Control>>Configure>>Hotend Type*
![](./E4/User_guide/hotendtype-mix.jpg)![](./E4/User_guide/hotendtype-nonmix.jpg)
#### :pushpin: The connectors of the Z9V5 print head are hidden inside the machine, you need to remove the rubber ring and pull out the connectors.
![](./Z9V5HotendWire.jpg)
### :warning: NOTE 1: If you can't find the "hotend type" menu on LCD screen, please upload the newest firmware to your printer. 
[**:point_right: Firmware for Z9V5**][FW_Z9V5] / [**:point_right: Firmware for Z8P**][FW_Z8P] / [**:point_right: Firmware for Z9M4**][FW_Z9M4] 
### :warning: NOTE 2: The mix color Hotend and non-mix color hotend must use different slice settings, please pay attention to distinguish. Using the wrong slice setting may block the hotend.

-----