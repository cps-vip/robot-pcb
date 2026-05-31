# Robot PCB
Welcome, brave soul. These are the working files for the robot's entire PCB. Almost everything is made from scratch, including buck regulators (DCDC switching) and motor drivers. See the to-do list below, and keep it up to date as you make changes. Footprints and symbols are kept here and imported to KiCAD as needed.

The associated CAD model is created in Onshape and the View link is here: https://cad.onshape.com/documents/2f51a332a8a74cbfb94f20e6/w/6173c2876300e7cd1fbb1689/e/74bdbf041e164ee37f124c87?renderMode=0&uiState=6a1c43214f1164212180f01c

You can copy, export, and modify the CAD as needed from Onshape. If this link ever goes out of date, you can use the STEP files I have in another repository called `robot-cad`. 

The STM32 CubeMX files are also in this repository and shall be used as a reference for available pins on the board. Keep the assignments up to date as you change the schematic, and you should avoid unexpectedly running out of timers. 

## Install footprints and symbols
1. In KiCAD, go to Preferences > Manage Symbol Libraries > [Folder Icon/Browse] > [Select the footprint file from `kicad_libraries`]

## To-Do
- [ ] Expansion GPIO ports: add female headers or similar (locking JST?) that expose more GPIO pins for debugging and added features
- [ ] Assign footprints, probably 0603 or 0402 to not go insane. For LEDs, use *emerald* green not yellow-green for the status indicator
- [ ] Lay out PCB (not trivial -- focus especially on the DCDC regulators' layout for efficiency; there are good youtube videos on this)
