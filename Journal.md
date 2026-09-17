## Time Spent

| Journal | Work | Time Spent |
|---|---|---:|
| Journal 1 | Planning and Designing | 1 hour |
| Journal 2 | Creating the Schematic in KiCad | 2.5 hours |
| Journal 3 | PCB Component Placement and Layout | 2.5 hours |
| Journal 4 | PCB Routing and Finalizing the Board | 3 hours |
| Journal 5 | Designing the Case and CAD Assembly | 3 hours |
| Journal 6 | Writing Firmware and Finishing the Project | 2 hours |
| **Total** | **Complete Coolio Pad Project** | **14 hours** |





# Coolio Pad :  Build Journal

## Journal 1 – Planning and Designing the Coolio Pad ( ## 11 SEP 2026 )

Today I started planning my hackpad project, which I decided to call Coolio Pad
I wanted to make something small and useful that I could keep next to my main keyboard.

My idea was to make a 15 key macropad with a rotary encoder.... 
The keys can be used for shortcuts like opening apps, copy andpaste, media controls, and other commands.
I also wanted the rotary encoder mainly for volume control.

For the controller, 
I decided to use the XIAO RP2040 because it is small and has enough pins for this project. 

I roughly planned the key layout first and tried to keep everything compact and clean.

After deciding the main components and layout, I was ready to start working on the schematic in KiCad.

**Time spent: 1 hour**

---

## Journal 2 – Creating the Schematic in KiCad  ( ## 12 SEP 2026 )

Today I started making the schematic for Coolio Pad in KiCad
I added the XIAO RP2040, 15 MX switches, diodes, the rotary encoder, and the other connections needed for the board.

The main thing I worked on was connecting the switches properly in a matrix. 
I used diodes with the switches so that multiple key presses can be detected correctly without unwanted inputs.

I also connected the rotary encoder to the controller and checked the power and ground connections. 
At first the schematic looked a little messy, so I rearranged the symbols and labels to make it easier to understand.

After checking the connections again, I assigned the required footprints and got the schematic ready for PCB design.

**Time spent: 2.5 hours**

---

## Journal 3 – PCB Component Placement and Layout ( ## 13 SEP 2026 )

Today I moved from the schematic to the PCB editor in KiCad. 
The first job was placing all 15 switch footprints in a clean grid so the macropad would feel organized and easy to use.

I placed the rotary encoder near the top of the board where it would be easy to reach.
Then I positioned the XIAO RP2040 and the diodes while trying to keep enough space between all the components.

A lot of the time went into moving things by small amounts and checking the spacing. 
I also thought about where the USB port would be so that the case would not block the cable.

Once the main layout looked right, I adjusted the board outline and prepared everything for routing.

**Time spent: 2.5 hours**

---

## Journal 4 – PCB Routing and Finalizing the Board ( ## 14 SEP 2026 )

Today I worked on routing the Coolio Pad PCB.
This part took more time because every switch, diode, encoder pin, and controller pin had to be connected without making the board too messy.

I routed the traces between the key matrix and the XIAO RP2040 first.
Some traces crossed each other... so I had to move components and use both PCB layers to make the routing cleaner.

After finishing the main connections... I checked the board for unconnected nets and spacing problems.
I also cleaned up some traces that had awkward turns and made the board easier to manufacture.

Finally, I checked the board outline and generated the final PCB files so the board would be ready for fabrication.

**Time spent: 3 hours**

---

## Journal 5 – Designing the Case and CAD Assembly ( ## 15 SEP 2026 )

Today I started working on the case for Coolio Pad. 
I wanted the case to be simple and compact... 
while still giving enough room for the PCB, switches, controller, rotary encoder, and USB cable.

I designed a top and bottom part for the case and added the required openings for the keys and encoder.
I also added screw holes so both parts could be fixed together properly.

After that.. I imported the PCB model into the CAD assembly and checked whether everything lined up. 
I had to make a few small changes to the dimensions and clearances 

so that the PCB would fit without touching the walls.

Once the fit looked good, I exported the final STEP files for the top, bottom, PCB, and full assembly.

**Time spent: 3 hours** ( ## 16 SEP 2026

---

## Journal 6 – Writing the Firmware and Finishing the Project ( ## 16 SEP 2026  )

Today I worked on the firmware for Coolio Pad using **KMK**. I set up the key matrix pins and assigned shortcuts to the 15 keys so each key can perform a useful action on the computer.

I also added support for the rotary encoder so it can be used for controls like increasing and decreasing volume. After setting up the basic controls, I went through the code and checked that the pin assignments matched the PCB schematic.

Once the firmware was ready, I organized the project files into separate folders for the PCB, CAD, and firmware. I also finished the BOM and README so the project would be easier for someone else to understand and build.

This was the final stage of Coolio Pad, and at this point the design, PCB, case, and firmware were all ready.

**Time spent: 2 hours**
