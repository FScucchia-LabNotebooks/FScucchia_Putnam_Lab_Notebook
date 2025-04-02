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
<img align="right" src="https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/wells2.png?raw=true">

2. Remove the old tubes corresponding to the “Cleaning & shutting down” procedure & replace them with new ones.
3. Place the “acquisition” cleaning tubes on the tray.

S 	Spin/dry empty (use regular 1.5mL tubes) 

W 	Mixer wash 1400µL water in 1.5mL tubes

Q 	Quick clean 1400µL water in 1.5mL tubes

B 	Backflush - empty 1.5mL tubes

C 	Clean/Rinse 750µL ICF – short 500uL free standing tube for this to save on ICF.

CS 	Capillary Shutdown 1400µL water in 1.5mL tubes

4. Before doing a Guava easyCheck with beads- perform one “Clean & Rinse” or “Quick clean” in InCyte to clean the system. The system is now ready for sample acquisition.

#### easyCheck 

At the start of each day (when in use), once the system has been cleaned, run the easyCheck procedure to ensure the system is performing properly before starting sample acquisition. easyCheck averages the results from three acquisitions of a guava easyCheck Bead sample to determine if the results are within the expected range.
1. Prepare a 1:20 dilution of the guava® easyCheck bead reagent. Refer to the guava easyCheck Kit package insert for information: 10 uL beads + 190 uL diluent minimum
2. Click easyCheck from the main menu. Allow the instrument to warm up for 10 minutes before acquiring the beads (also allow bead and diluent to warm to RT).
3. Make sure the correct Bead Lot # and Bead Expiration Date (found on the guava easyCheck Bead Reagent vial label) and Expected Particles/mL are entered in the appropriate fields. Optionally, you may enter the guava® easyCheck Kit lot number and expiration date (found on the side of the guava easyCheck Kit box). The particles/mL corresponds to the concentration of beads in your prepared sample where the guava easyCheck Bead Reagent is diluted 1:20 with diluent.
4. Click Start. 
5. The sample tray opens and a dialog box appears prompting you to load DI water, and empty tubes, and select the tube/well containing the beads.
6. Load tubes filled with fresh DI water in w2, w4, and w5 (make sure they are all full).
7. Load empty tubes in w3 and w6.
8. Load a tube containing 100 μL of bleach in position w1 (for performing a backflush)
9. Load the easyCheck sample into the chosen well (make sure you mark the chosen well).
10. Click on the tube/plate map to select the tube/well with beads.
11.	Click OK. The system will run easy check
_Note_: If you are using a microplate, make sure well A1 of the plate is in the top-right corner of the tray.

#### easyCheck Results

The software displays %CVs and averages for particles/mL (bead count), FSC and SSC intensities, and GRN, YLW, RED, NIR, RED2, and NIR2 (if applicable) mean fluorescence intensity (MFI) for three replicates.
1.	If any result for Particles/mL falls outside ±10% of the expected value, the result is outside the acceptable range and appears in red. For example, if the actual particle count is 50,000, the acceptable Particles/mL range (±10%) is 45,000 to 55,000.
2. If the %CV for Particles/mL is >10%, it appears in red.
3. The %CV for FSC and SSC Intensities, and GRN/YLW/RED/NIR/RED2/NIR2 MFI for the three replicates should be <5%.
4. Refer to the information card that comes with the guava easyCheck Kit for the acceptable intensity ranges for each parameter.
5. If the Particles/mL (count) for a replicate or the average falls outside the acceptance range, or if an intensity value is outside the acceptable range, run Quick Clean or Clean & Rinse. Rerun the easyCheck Procedure with new bead dilution. If values continue to fall outside the acceptance range, refer to “easyCheck Procedure Troubleshooting” on page 2-8 of the manual, for more information.

#### SAMPLE ACQUISITION

1. Once the worklist is created, the tray will open: you can now place your plate. 
2. Make sure that the tubes Q (DI water) and C (ICF) are filled up before starting the acquisition. Check these tubes every time you put a new plate, since a cleaning procedure is automatically performed at the end of a plate acquisition.
3. Settings can only be saved after settings have been adjusted, before running the worklist.
4. For optimal acquisition, use cells at a concentration of 500 cells/µL.
5. Beware of dead volumes: round bottom w96: 50µL; flat-bottom w96: 75µL; 0.5mL Microtubes: 70µL; 1.5mL tubes: >1mL.
6. If the acquisition rate slows dramatically, and there is sufficient sample volume, the fluid pathway may be blocked. Click “Stop”, wait for the system to stop, and then click “Backflush”. Once the Backflush procedure is complete, click “Quick Clean” to rinse any bleach from the capillary.
7. Empty the waste, wash it and add bleach to the vial when more than half full.

#### Quick Clean

1.	Whenever leaving a system ON and NOT IN USE - do quick clean then Capillary Shutdown. 
2. Before beginning a sample run do a “quick clean”, automatically select quick clean after 12 sample wells in work list edit.
3. Approximately three Quick Clean cycles can be performed from a single well in a plate containing 250ul and seven Quick Cleans from a 1.5-mL tube containing 1.5 mL of fluid before well or tube runs.
dry and reach dead volume. Ensure cleaning tube is filled up during long runs (pause run, eject tray, top up cleaning tube, load tray, restart run).

#### Capillary Shutdown

1. At the end of your sample acquisition, close the “InCyte” module, open the “Cleaning” module and perform a “Capillary Shutdown” procedure, to make sure that the capillary is not getting dry. 
2. Always use the CS tube in position 9.
3. Never let the Guava stand overnight without making sure that the capillary has been cleaned and that “Capillary shutdown” procedure has been performed.

#### GUAVA SHUT DOWN 
1. Quit “InCyte” module and go to the “Cleaning” module. Click on “Start clean”: the tray will eject.
<img align="right" src="https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/wells3.png?raw=true">

2. Remove the tubes corresponding to the ‘acquisition clean’ procedure.
3. Place the cleaning tubes on the tray (prepare a new set every day). Use “short” 0.5mL, free standing Microtubes to spare reagents.

W 	Wash tubes- 1400µL water in 1.5mL tubes

B 	Backflush - empty 1.5mL tube

C 	clean/rinse 750µL ICF – short 0.5ml free standing tube for this to save on ICF.

CS 	Capillary Shutdown 1400 µL water in 1.5mL tubes

4. Run the “Clean” procedure to wash the system TWICE (lasts 15min each run), do this AT LEAST ONCE if no time.
5. Select the CS tube (position 9) as the “Capillary shutdown” tube. The “Capillary shutdown” procedure is automatically done at the end of the “Clean” procedure.
6. Once the “Clean” procedure is over, quit GuavaSoft; switch off laptop and Guava system.








