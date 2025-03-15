---
layout: post
title: Total Protein Protocol
date: '2025-03-15'
category: [ Physiology ]
tags: [ Coral, Protein ]
---

#### Measuring concentration of total protein

**Protocols used**
- [Putnam Lab Total Protein Protocol](https://emmastrand.github.io/EmmaStrand_Notebook/Total-Protein-Protocol/)

I followed the above protocol with some adaptations by me to quantify total protein of  _Pocillopora acuta_ (Pacu), _Montipora capitata_ (Mcap) and _Porites compressa_ (Pcom) for the ENCORE Hawaii TPC project.

This protocol is adapted to determine total protein (soluble and insoluble) content using the [Pierce BCA Protein Assay Kit from Thermo Scientific](https://www.thermofisher.com/order/catalog/product/23225?SID=srch-srp-23225).  

Coral homogenate prep can be found in my [previous post](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/Sample-Prep-Physio-Hawaii-TPC/).

# Detailed Protocol  

**Adult Tissue Sample Preparation**
1. Thaw homogenate aliquot labeled with the coral ID and "protein".
2. Pipette 650uL from the 1.5mL aliquot into a new labeled 1.5 mL microcentrifuge tube and vortex (put back the rest in the freezer as spare)
3. Centrife at 13000 rpm for 4 minutes at 4°C to separate host from the algae.
4. Take 500uL of the supernatant into a new tube lables "HOST protein".
5. Add 10 μL of 1M NaOH to the tube.  
6. Pipette a very small amount of sample onto pH paper to confirm the pH ~10.  
7. Incubate the tube at 50°C for 4 hours, shaking at 300 rpm.  
8. Add 280 μL of 0.1M HCl to the tube to neutralize the sample. Add this volume in small amounts and continue to test the pH of the sample using pH paper. pH needs to be at 7.0 to move onto the next steps. _Take note of how much volume of HCL was added!_.  

**Preparation of Diluted Albumin (BSA) Standards**  
*These standards can be made during the 4 hour incubation period in the sample preparation section.*
1. Use the following table as a guide to prepare a set of protein standards. For this project we will use the microplate procedure. Diluent is DI water Type II. Each vial will be a sterile 1.5 mL microcentrifuge tube. Label the cap of the microcentrifuge tube with the Vial ID ("A", "B", etc.).  

| Vial | Volume of Diluent (μL) | Volume of Source of BSA (μL) | Final BSA Concentration (μg/mL) |
|------|------------------------|------------------------------|---------------------------------|
| A    | 0                      | 300 of Stock                 | 2000                            |
| B    | 125                    | 375 of Stock                 | 1500                            |
| C    | 325                    | 325 of Stock                 | 1000                            |
| D    | 175                    | 175 of vial B dilution       | 750                             |
| E    | 325                    | 325 of vial C dilution       | 500                             |
| F    | 325                    | 325 of vial E dilution       | 250                             |
| G    | 325                    | 325 of vial F dilution       | 125                             |
| H    | 400                    | 100 of vial G dilution       | 25                              |
| I    | 400                    | 0 (Blank)                    | 0                               |

**Preparation of the BCA Working Reagent (WR)**   
1. Use the following formula to determine the total volume of WR required:  
(# standards + # unknowns) x (# replicates) x (volume of WR per sample) = total volume WR required  
I will use here 2 replicates for the standards and 3 replicates for each sample. The Working Reagent (WR) to be added in the plate is 200uL, I'm using 200.5uL in the equation to account volume lost during pipetting.
> *(18 standards (9x2 rep) + 18 samples (6x3 rep)) x (200.5 μL of Working reagent WR) = total volume of WR required*  
(18 standards + 18 samples) x (200.5 μL of WR) = 7,218 μL WR  
2. Prepare WR by mixing 50 parts of BCA Reagent A with 1 part of BCA Reagent B (50:1, Reagent A:B) in a sterile glass bottle of the appropriate size based on how many samples are going to be run.  

**Microplate Procedure (Sample to WR ratio = 1:8) from Pierce BCA Protein Assay Kit:**  
1. Pipette 25 μL of each standard or unknown sample replicate into a microplate well.  
2. Add 200 μL of the working reagent (WR) to each well and mix the plate thoroughly on a plate shaker for 30 seconds.  
3. Cover the plate and incubate at 37°C for 30 minutes.  
4. Subtract the average 562 nm absorbance measurement of the Blank standard replicates from the 562 nm measurements of all other individual standard and unknown sample replicates.  
5. Pepare a standard curve by plotting the average Blank-corrected 562nm measurement for each BSA standard vs. its concentration in μg/mL. Use the standard curve to determine the protein concentration of each unknown sample.  