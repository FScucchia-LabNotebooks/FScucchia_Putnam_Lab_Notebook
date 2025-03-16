---
layout: post
title: Chlorophyll Protocol
date: '2025-03-15'
category: [ Physiology ]
tags: [ Coral, Chlorophyll]
---

#### Measuring concentration of Chl-a and Chl-c2 in Symbiodiniaceae 

**Protocols used**
- [Putnam Lab Chlorophyll Protocol](https://github.com/Putnam-Lab/Lab_Management/blob/master/Lab_Resources/Physiology_Protocols/Chlorophyll-Protocol.md)

I followed the above protocol based on [Wall et al. 2018](https://link.springer.com/content/pdf/10.1007/s00227-018-3317-z.pdf) with some adaptations by me to quantify Chl-a and Chl-c2 concentration in algale symbiont of  _Pocillopora acuta_ (Pacu), _Montipora capitata_ (Mcap) and _Porites compressa_ (Pcom) for the ENCORE Hawaii TPC project.

Coral homogenate prep can be found in my [previous post](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/Sample-Prep-Physio-Hawaii-TPC/).

# Detailed Protocol  

**Sample Preparation**  
1. Thaw coral homogenate aliquot and vortex sample for 15 seconds.
2. To separate host and algae, centrifuge the 1.5 tube for 4 minutes at 5000rpm at 4°C. 
3. Remove the supernatant (host tissue) work with pellet (algae).
4. Resuspend the algae with 1ml 1XPBS and homogenize.
5. Centrifuge for 5 minutes at 5000rpm at 4°C.
6. Remove the supernatant. 
7. Resuspend the algae with 1ml PBS and homogenize.
8. Centrifuge for 5 minutes at 5000rpm at 4°C.
9. Remove the supernatant thoroughly
10. Resuspend the algae with 1ml PBS and homogenize.
11.	Take 30ul for algae count, freeze and store. 
12.	Centrifuge the rest of the 1mL for 5 minutes at 5000rpm at 4°C.
13.	Remove the supernatant thoroughly
14. Add 1 mL of 100% acetone to the pellet in the 1.5 mL microcentrifuge tube and vortex the tubes to mix.
15. Place the tubes in a fridge in the dark at 4°C for 24 hours.  
16. The next day, vortex the tubes for 15 sec.  
17. Spin the tubes down at 13,000 rpm for 3 minutes at 4°C in the microcentrifuge to pellet any debris.  
18. Pipette 200µl of sample to triplicate wells of 96-well quartz plate.   
19. Pipette 200µl of acetone blank to duplicate wells.  
10. Cover the plate with silicone pad every 5th sample or so to reduce evaporate as samples are added.  
11. Remove silicon pad.   
12. Follow steps below to measure the extract Absorbance on the [Synergy HTX Multi-Mode Microplate Reader](https://www.biotek.com/products/detection-multi-mode-microplate-readers/synergy-htx-multi-mode-reader/) at 630, 663, and 750 nm in a 96-well quartz plate.
13. Standardize for path length in 200µl of sample in 96-well quartz plate.

**Measure the Absorbance**
    1.Open the Gen5 software on your computer.
    2.Once Gen5 opens on the computer you can select the pre-made protocol from the drop down menu.
    4.The plate loader should automatically open.Once the software is open on the computer.
    5.Place the 96 quart plate in the plate reader.
    5.To measure Absorbance, select the pre-made 'Chlorophyll Protocol' option and press the green start protocol button and allow to run through the 630,663 and 750nm.
    6.Export the raw GEN5 software data file and a CSV to the Desktop in a designated folder.

**Calculating Chlorophyll Concentration**
Chlorophyll a and c2 concentrations are calculated from the equations in [Jeffrey and Humphrey 1975](https://reader.elsevier.com/reader/sd/pii/S0015379617307783?token=0937035D38C07F29ADF00F1F2A21F20F221219B1CC11A444A4F84D16B98EC3A6AD941D191BA2135A68C98BA62A0B69FE) after substracting A750nm from all measurements.

Need to correct for differences in path length of the volume in the 96 well plate compared to the 1cm path length of a cuvette.
[Warren 2007](https://www.tandfonline.com/doi/full/10.1080/01904160802135092?casa_token=RqeUl1Ccg7AAAAAA%3A6SyNAs848qrRk1-Tf1g088xWD10z1Xngb8cmcgRvC3jYSYPugr2cL8QG9wFvrFj7xZF-pqqUozonRg)

R code for this analysis can be found at [K. Wong's Github](https://urldefense.proofpoint.com/v2/url?u=https-3A__github.com_kevinhwong1_Thermal-5FTransplant-5F2017-2D2018_blob_master_scripts_ChlorophyllA.R&d=DwMFaQ&c=dWz0sRZOjEnYSN4E4J0dug&r=hzX7Pj5Cn4ufjLQbICvWcOqlrencJyNZMIrmCT00z_o&m=Hpn_SeiBeA7gle40eXLMx3-j3YSrgRHCsOsZ3E5cSGA&s=q5PUrza32gdiEvIa0nI8pMvjeaMw9LFkIDujTh_tGPw&e=).

<a name="References"></a> **References**
 1.  [Jeffrey and Humphrey 1975](https://reader.elsevier.com/reader/sd/pii/S0015379617307783?token=0937035D38C07F29ADF00F1F2A21F20F221219B1CC11A444A4F84D16B98EC3A6AD941D191BA2135A68C98BA62A0B69FE)
    2. [Warren 2007](https://www.tandfonline.com/doi/full/10.1080/01904160802135092?casa_token=RqeUl1Ccg7AAAAAA%3A6SyNAs848qrRk1-Tf1g088xWD10z1Xngb8cmcgRvC3jYSYPugr2cL8QG9wFvrFj7xZF-pqqUozonRg)
    3. [Synergy HTX Operating Manual](https://github.com/urol-e5/protocols/blob/master/synergy_htx_manual.pdf)
    4. [Gen5 Software Manual](https://github.com/urol-e5/protocols/blob/master/Gen5_software_manual.pdf)