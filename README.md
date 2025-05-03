# HE60

HE60 is a 60% Hall-effect keyboard PCB with a split spacebar, and a Tsangan layout.

## Features

- Support for GH60 tray mount cases e.g., KBDfans Tofu60 Redux, and KBDfans Holy60.
- Support for gummy O-ring mount cases **if the USB-C port is not soldered** e.g., Bakeneko60, and SingaKBD Unikorn (required 10mm JST cable).
- [libhmk](https://github.com/peppapighs/libhmk) firmware.
- [hmkconf](https://hmk.prasertsuk.com) web-based configurator.

## Disclaimer

- At the moment, only the gummy O-ring version with 1.2mm PCB thickness has been tested. Please proceed with caution if you are using the tray mount version.
- The PCB requires standoffs to be mounted to the switch plate. The mounting points are **not compatible** with other available plates e.g., GEON Venom60 7U plate.

## Supported Layouts

![Layouts](/doc/layout.png)

## Fabrication

The following files are required:

- BOM (Bill of Materials): Contains the list of components required to build the PCB.
- Pick and Place: Contains the placement of the components on the PCB.
- Gerber: Contains the PCB design files for fabrication.

Note that the components in the BOM are all mounted on the bottom side of the PCB, and are based on the available components in JLCPCB at the time of writing. You may need to adjust the components based on your preference or availability. For the JST connector (labeled `JST_SH`), I used WAFER-SH1.0-4PWB offered by JLCPCB. **Make sure to deselect the USB-C port when choosing the components to solder if you are using the gummy O-ring version.**

The fabrication files above are available [here](https://github.com/peppapighs/HE60/releases).

## Build Guide

The following items are required to build the PCB:

- PCB
- Switch plate (DXF file available [here](/plate.dxf). You may need to use less flexible materials such as aluminum or FR4 to prevent the switch at the top right corner from popping out if you use the alternative backspace layout.)
- Magnetic switches (e.g., GEON Raw HE, Gateron Magnetic Jade, Duhuk Core HE, etc.)
- Stabilizers (**Clip-in is required for the gummy O-ring version**)
- M2 3.5mm standoffs x8 (available at [KBDfans](https://kbdfans.com/collections/other-accessories/products/kbdfans-m2-3-countersunk-flat-head-screw-kit), and [Taobao](https://item.taobao.com/item.htm?_u=d20ikgunaje547))
- M2 3mm flat head screws x16

1. Attach the standoffs to the PCB using the M2 screws. **Warning: The position of the standoff above the spacebar in v1.0 will interfere with the 7U stabilizer. Consider removing it if you are using the 7U layout.**

![Standoff](/doc/1-standoff.jpg)

2. Install the stabilizers to the PCB.

![Stabilizers](/doc/2-stabilizers.jpg)

3. Install the switches to the plate.

![Plate with switches](/doc/3-plate-with-switches.jpg)

4. Assemble the plate and PCB together. Press the PCB against the plate to make sure the switches are seated properly.

![Assembled side](/doc/4-assembled-side.jpg)

5. Screw the standoffs to the plate using the rest of the M2 screws.

![Assembled](/doc/5-assembled.jpg)

6. Install the PCB into the case.

![Case](/doc/6-case.jpg)
![Case with keycaps](/doc/7-case-with-keycaps.jpg/)

## Firmware

Refer to the [libhmk](https://github.com/peppapighs/libhmk) documentation for the firmware installation instructions.

## Acknowledgements

- Xelus from AEBoards for reviewing the PCB design and providing feedback.
- Keyboard Atelier community for supporting the project.
