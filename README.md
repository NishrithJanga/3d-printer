(https://cad.onshape.com/documents/6f697001031dbbe71f837ac1/w/ae4aa53d3f2619e6b3c1bbec/e/5889169bc7ef53647b7ca88b?renderMode=0&uiState=6a7bc8560968168bbb8c9fb8) that is the actual link to the cad just in case if u wanted it even though u can see it in stardance😁😉
# Custom $440 Open-Source Printer Build

This is my documentation log for a custom 3D printer build for the **Hack Club Stardance Summer Challenge**. 

## What I'm Building
I am building a high-performance 3D printer entirely from scratch out of individual loose parts. To follow the rules and make sure this counts as a true engineering project, I am completely skipping pre-made retail kits. Every single rail, screw, motor, and wire is being self-sourced piece-by-piece from various suppliers.

## How It Works (Sourcing & CAD)
* **The Blueprint:** The cad software that i used was onshape which is a free on browser cad like tinkercad.                     
* **The Frame:** Instead of custom brand-name plastic joints, I’m using standard 2040 and 2020 aluminum extrusions bolted together with flat 90-degree metal corner plates and loose screws.
* **The Brains:** The printer runs on a dual-board system. I'm using a **BIGTREETECH SKR Mini E3 V3** motherboard to control the physical motors, and hooking it up to a **Raspberry Pi 4 (2GB)** running Linux and Klipper so I can control the printer over my local network.

## Parts, Budget, and shipping+tax ($465)
My total budget comes out to about(would be exact but shipping and tax varies😒) **$465.00**. You can see the full, itemized spreadsheet tracking every single motor link, rail cost, and screw box directly inside the [`bom.csv`](./bom.csv) file in this repository.

## Za Building Plan

### Step 1: Building and Squaring the Frame
* Unbox the raw aluminum rails and clean down the steel smooth rods.
* Bolt the base together using loose T-nuts and corner brackets.
* Use a square tool and calipers to make absolutely sure the vertical frame towers are perfectly flat and perpendicular to the bed.

### Step 2: Adding Motors and Motion Parts
* Mount the four NEMA 17 stepper motors to the frame.
* Slide the linear ball bearings onto the smooth rods and bolt them to the metal gantry plates.
* Route the timing belts around the pulleys and pull them tight so there is no loose slack.
* Mount the Creality Sprite Pro toolhead extruder onto the X-axis plate.

### Step 3: Electronics and DIY Wiring
* Wire up the 24V Mean Well power supply.
* Mount the mainboard and Raspberry Pi safely inside a generic electronics case.
* Cut, route, and crimp the loose motor wires to the exact right lengths using a JST pin toolkit so everything plugs cleanly into the motherboard.

### Step 4: Software and Testing
* Flash the Klipper firmware onto the mainboard.
* Install the operating system and web controls onto the Raspberry Pi's SD card.
* Write the `printer.cfg` setup file from scratch to teach the computer how fast to move the motors and read the temperature sensors.
* Run calibration tests, heat up the bed, and get the first test prints running!
* pls accept this cause i've got this whole day of undocumented hours and im excited for building
