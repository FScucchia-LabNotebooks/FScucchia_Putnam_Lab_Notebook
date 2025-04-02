---
layout: post
title: Symbiont cell count protocol - GUAVA
date: '2025-03-15'
category: [ Physiology ]
tags: [ Coral, Chlorophyll]
---

#### Measuring concentration of Symbiodiniaceae cells using the GUAVA instrument

**Instrument details**

This protocol refers to the Millipore Guava easyCyte HT Flow Cytometer located at the URI Coastal Institute Building (Bay Campus).

![GUAVA.png](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/GUAVA.png?raw=true)

**Equipment for GUAVA**

All specific equipment for use can be found in the GUAVA manual. 
- 96 well plates with round bottoms
- 1.5mL tubes
- ICF solution 
- Bleach (sodium hypochlorite solution) 
- GUAVA easyCheck Kit (contains Guava easyCheck Bead Reagent and Guava Check Diluent)

**Sample Preparation**  

1. Thaw coral homogenate aliquot (650uL) and vortex sample for 15 seconds.
2. To separate host and algae, centrifuge the 1.5 tube for 4 minutes at 5000rpm at 4°C. 
3. Remove the supernatant (host tissue) work with pellet (algae).
4. Resuspend the algae with 650uL 1XPBS and homogenize.
5. Centrifuge for 5 minutes at 5000rpm at 4°C.
6. Remove the supernatant. 
7. Resuspend the algae with 650uL PBS and homogenize.
8. Centrifuge for 5 minutes at 5000rpm at 4°C.
9. Remove the supernatant thoroughly
10. Resuspend the algae with 650uL PBS and homogenize. Freeze and store. 

_Note_: You want to make sure that the samples is free of host remainings and dirt, which may clog the GUAVA.

**Measuring symbiont cell density**
#### System Start-up
1. Turn on the laptop computer.
2. When the computer is finished booting up, turn on the guava easyCyte HT System. The power switch is located half-way up on the right side at the back of the instrument.
3. Start guavaSoft Software by double-clicking the guavaSoft application icon on the desktop.

#### System prime
1. Prime the system by performing a complete cleaning procedure.
<img align="right" src="https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/wells.png?raw=true">
2. Click on the “Essential Tools” option and open the “Cleaning” module. Click on “Start clean”: the tray will eject. 
3. The tubes from the previous procedures will be on the tray
4. If tubes are one day old-refill the tubes with MilliQ water or ICF in the proper locations. If more than one day old, replace tubes that appear to be contaminated or dirty. 
5. Run the “Clean” procedure to prime/wash the system TWICE (it lasts for 15mins each). Do this at least once if not enough time or Guava is in regular use. Do at least TWICE after weekends, or long period of not in use.
6. Select the CS tube (position 9) as the “Capillary shutdown” tube, as system won’t be in use immediately.

#### Capillary Shutdown

1. The “Capillary Shutdown” procedure is automatically done at the end of the “Clean” procedure.
2. The capillary is placed into a tube of water and can stay like this until acquisition without any risk of drying particles on the capillary glass wall.

#### Backflushig the Fluid System

1. If the fluid system is suspected as being blocked, click “Backflush” on the easyCheck screen, or any Guava assay screen. A message should appear on the screen with a prompt to select the well/tube to be used for backflushing – the default position is w1, conaining 100ul of bleach 
2. Leave the default position for Backflushing as w1 and click “OK” (w1 must be containing 100ul bleach solution before clicking “OK”).  
3. Once the Backflush procedure is complete, click “Quick Clean” to rinse any bleach from the capillary.
4. If a run has been paused in order to perform the the Backflush procedure, click “Resume”.

#### System preparation 
1. Open the “InCyte” module. Open the tray by clicking on the EJECT button. 	
2. Remove the old tubes corresponding to the “Cleaning & shutting down” procedure & replace them with new ones.
3. Place the “acquisition” cleaning tubes on the tray.
<img align="right" src="https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/wells2.png?raw=true">
S 	Spin/dry empty (use regular 1.5mL tubes) 
W 	Mixer wash 1400µL water in 1.5mL tubes
Q 	Quick clean 1400µL water in 1.5mL tubes
B 	Backflush - empty 1.5mL tubes
C 	Clean/Rinse 750µL ICF – short 500uL free standing tube for this to save on ICF.
CS 	Capillary Shutdown 1400µL water in 1.5mL tubes

4. Before doing a Guava easyCheck with beads- perform one “Clean & Rinse” or “Quick clean” in InCyte to clean the system. The system is now ready for sample acquisition.

