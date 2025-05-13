---
layout: post
title: Troubleshooted Zymo SwitchFree library prep - Hawaii TPC samples - 051325
date: '2025-03-13'
category: Protocol
tags: [DNA, Zymo, RNA, library]
---

#### Throubleshooting library prep using the Zymo-Seq SwitchFree 3′ mRNA Library Kit following recommendations from Zymo team - Hawaii TPC samples - 051325

**Protocols used**
- [Zymo-Seq SwitchFree 3′ mRNA Library Kit protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/_r3008_r3009__zymo_seq_switchfree_3_mrna_library_kit.pdf)
- [TapeStation protocol DNA D5000](https://github.com/meschedl/MESPutnam_Open_Lab_Notebook/blob/master/_posts/2019-07-30-DNA-Tapestation.md)
- [High Sensitivity dsDNA QBIT protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/MAN0017455_Qubit_1X_dsDNA_HS_Assay_Kit_UG.pdf)

Using the [Zymo-Seq SwitchFree 3′ mRNA Library Kit](https://www.zymoresearch.com/products/zymo-seq-switchfree-3-mrna-library-kit) (CAT.  R3009-A, LOT. 252649) to prepare libraries starting from RNA samples exctracted from adult coral fragments from the Hawaii TPC project. RNA extraction posts can be found [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-TPCA-Summary/).

For this library prep (performed on 05/11/25.), I followed the protocol of [Jill Ashey](https://github.com/JillAshey/JillAshey_Putnam_Lab_Notebook/blob/master/_posts/2024-03-29-Zymo-SwitchFree.md) and the kit protocol above.
I used the Zymo team recommendations to troubleshoot the library prep as detailed [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/Troubleshooting-LibraryPrep-ZymoSwitch/). In particular, I've done the following:

1. I've used 10 ng as input RNA.
2. I've decreased the volume of Poly A R1 Reagent from 5 ul to 3 ul (supplementing with 2 ul of DNase/RNase Free water) 
3. I've used 19 PCR cycles, final elution 20 ul.
4. I've performed an extra cleanup (following Appendix C of the Zymo kit manual above) on individual libraries (I didn't pool them). With the extra cleanup, I eluted in 15 ul instead of 20 ul.
5. I've let the beads to dry for 6-7 minutes.

Here I'm using UDI primers for WGBS that we had in the lab. 

## Library prep

Here's a breakdown of input RNA volume and quantity:

| sample_id || RNA_QBIT_AVG (ng/uL) || RNA (uL) || Ultrapure water (uL) || Total input RNA (ng) |
|  Pacu-F9  || 34.1   || 0.29  || 4.71   ||       10        |
|  Pcom-F7   || 43.4 || 0.23   || 4.77   ||     10       |
|  Mcap-F1  || 17.3  || 0.58   || 4.42   ||      10        |

The library prep for these samples didn't work before, see [previous post](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/LibraryPrep11-ZymoSwitch-Hawaii-TPC/).

## Qubit Results

I used High Sensitivity dsDNA Qubit Protocol linked above. Library samples were read twice, standard only read once.
- Standard 1: 82.18   
- Standard 2: 27184.51

| QBIT date  || sample_id  ||     Species       || Library read1 || Library read2  || Library_AVG (ng/ul) |
|  20250511  || Pacu-F9 || *Pocillopora acuta*  || 19.1  ||   18.7   || 18.9       |
|  20250511 || Pcom-F7  || *Porites compressa* || 4.9  ||   4.7     || 4.8      |
|  20250511  || Mcap-F1 || *Montipora capitata*  || 6.5   || 6.1  || 6.3           |

## TapeStation

After the library prep, I run samples on the tapestation (D5000), protocol linked above.

| TapeStation date  || sample_id  ||     Species       || TapeStation conc. ||   Primer set  |
|  20250513  || Pacu-F9 || *Pocillopora acuta*  || 23.2  ||  34     |
|  20250513 ||Pcom-F7  || *Porites compressa* || 5.88    ||  35     |
|  20250513  || Mcap-F1 || *Montipora capitata* || 7.46    ||  36    |

![LibPrepRun.png](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/LibPrepRun.png?raw=true)

