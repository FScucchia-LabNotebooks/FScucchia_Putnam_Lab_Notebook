---
layout: post
title: Carbohydrates Protocol
date: '2025-04-16'
category: [ Physiology ]
tags: [ Coral, Carbohydrates]
---

#### Measuring concentration of carbohydrates in coral host tissue 

**Protocols used**
- [Putnam Lab Carbohydrate Protocol](https://github.com/Putnam-Lab/Lab_Management/tree/master/Lab_Resources/Physiology_Protocols/Carbohydrates/Bove_Baumann_96well_Protocol)


For the published protocol, see [dx.doi.org/10.17504/protocols.io.bvb9n2r6](https://www.protocols.io/view/coral-carbohydrate-assay-for-96-well-plates-bvb9n2r6). This protocol was modified and based off [this protocol](https://www.protocols.io/view/coral-carbohydrate-assay-for-96-well-plates-bvb9n2r6). 
I used the protocol linked above to quantify carbohydrates concentration in host tissue of of  _Pocillopora acuta_ (Pacu), _Montipora capitata_ (Mcap) and _Porites compressa_ (Pcom) for the ENCORE Hawaii TPC project.

Coral homogenate prep can be found in my [previous post](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/Sample-Prep-Physio-Hawaii-TPC/).

# Detailed Protocol  

**Reagent and Standard preparations**

***10 mM Glucose stock solution (50mL)***
- Calculation to get to 10 mM L-(-)-Glucose:
  - Molecular Weight of L-(-)-Glucose: 180.16g
  - 1 M = 180.16g/1L Water
  - 1 mM (or 0.001 M) = 0.18g/L of water
  - 10 mM = 1.8g/1L of water
  - g of  L-(-)-Glucose needed for 10mM in 50mL = 1.8g/200 = **0.009g** (9mg)

1. Add 50mL of milliQ water to a 50 mL falcon tube
  - *label: 10 mM Glucose stock solution, Date, Initials*
2. Add 0.009g of [L-(-)-Glucose](https://www.sigmaaldrich.com/catalog/product/sigma/g5500?lang=en&region=US&gclid=Cj0KCQjw2NyFBhDoARIsAMtHtZ5C7ue3ciohFrpwseZgAYYvwQDzMdudL-xTZ7d94oJd6AzG398G9gYaArqVEALw_wcB)
3. Vortex and store in 4°C fridge.

***1 mM Glucose stock solution (50mL)***
1. Add 45mL if milliQ water to a 50mL falcon tube
  - *label: 1 mM Glucose stock solution, Date, Initials*
2. Add 5mL of 10 mM Glucose stock solution
3. Vortex and store in 4°C fridge.

**Sample Preparation**  

1. Thaw coral homogenate aliquot and vortex sample for 15 seconds.
2. To separate host and algae, centrifuge the 1.5 tube for 4 minutes at 5000rpm at 4°C. 
3. Remove the supernatant (host tissue) and put in new labeled tube.

**Carbohydrates measurement**

1. Take out samples and thaw at room temperature
  - If running each sample in triplicates, you can do 22 samples per plate
2. Label (10 + # of samples) 5 mL tubes
3. While samples are thawing, make the standards and blanks as shown in the table below:

| Tube ID | Concentration (mg/mL) | Vol water (uL) | Vol 1 mM Glucose (ul) | Vol 10mM Glucose (uL) |
|:-------:|:---------------------:|:--------------:|:---------------------:|:---------------------:|
|    B    |         0.0000        |      1000      |           0           |           0           |
|    1    |        0.00901        |       950      |           50          |           0           |
|    2    |        0.01802        |       900      |          100          |           0           |
|    3    |        0.02703        |       850      |          150          |           0           |
|    4    |        0.03604        |       800      |          200          |           0           |
|    5    |        0.05406        |       700      |          300          |           0           |
|    6    |         0.0901        |       500      |          500          |           0           |
|    7    |         0.1802        |        0       |          1000         |           0           |
|    8    |         0.3604        |       800      |           10          |          200          |
|    9    |         0.901         |       500      |           0           |          500          |

4. Vortex samples after thawing
5. Add 100 uL of coral slurry and 900 uL milliQ water to pre-labelled test tube for all samples
  * **Note:** You many need to concentrate or dilute your samples more depending on how they were collected.
6. Set up a room temperature water bath in the fume hood with test tube rack (i.e. DI water in a plastic bin)
  * This is to prevent the tubes from over heating from the addition of sulphuric acid
7. Add 25 uL of phenol to first sample
8. Vortex (in the hood) for 3 seconds
9. Immediately add 2.5 mL sulphuric acid to the sample
10. Incubate the sample at room temperature for 1 minute then transfer to water bath
11. **Repeat steps 6-10 for all tubes, standards included**
12. When the last sample is placed in the water bath, incubate all samples for 30 minutes
13. Pipette 200 uL of all standards and samples into the bottom of the wells in a 96-well plate
  * Have a printed plate layout with well numbers and sample IDs
14. Read on spectrophotometer at 485 nm

**Calculations**

1. Create standard curve with known standard concentrations and absorbance values (y = mx + b)
2. Using the resulting equation, convert sample absorbance to concentrations (mg/mL)
3. Multiply sample concentration (mg/mL) by total slurry volume (mL) and dilution factor (1000/v of sample, usually 100 mL), then divide by surface area (cm2) for resulting units: mg/cm2