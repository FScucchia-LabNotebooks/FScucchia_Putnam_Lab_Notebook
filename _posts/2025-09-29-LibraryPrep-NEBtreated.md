---
layout: post
title: Library prep using Zymo SwitchFree kit on samples with PolyA isolation - 092925
date: '2025-09-29'
category: Protocol
tags: [DNA, Zymo, RNA, library]
---

#### Using the Zymo-Seq SwitchFree 3′ mRNA Library Kit for in-house library prep of samples treated for PolyA isolation - 092925

**Protocols used**
- [Zymo-Seq SwitchFree 3′ mRNA Library Kit protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/_r3008_r3009__zymo_seq_switchfree_3_mrna_library_kit.pdf)
- [NEBNext Poly(A) Magnetic Isolation Module](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/NEBPolyA.pdf)
- [TapeStation protocol DNA D5000](https://github.com/meschedl/MESPutnam_Open_Lab_Notebook/blob/master/_posts/2019-07-30-DNA-Tapestation.md)
- [High Sensitivity dsDNA QBIT protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/MAN0017455_Qubit_1X_dsDNA_HS_Assay_Kit_UG.pdf)

Using the [Zymo-Seq SwitchFree 3′ mRNA Library Kit](https://www.zymoresearch.com/products/zymo-seq-switchfree-3-mrna-library-kit)(CAT.  R3009-A, LOT. 252649) to prepare libraries starting from RNA samples exctracted from adult coral fragments and spat. RNA extraction posts can be found [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-McapSpat2/), [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-McapSpat3/) and [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-McapSpat1/), and in Zoe's notebook ([here](https://zdellaert.github.io/ZD_Putnam_Lab_Notebook/Switch-Free-TimeSeries-Library-Prep-Test/)).
NEB treatment post can be found [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/PolyAenrichment-NEB-trial/).

The idea is to use the NEB kit before performing the library prep to reduce the amount of rRNA present in the libraries. Libraries of the same samples non-NEB treated will be also prepared in parallel.

For the library prep I followed the protocol of [Jill Ashey](https://github.com/JillAshey/JillAshey_Putnam_Lab_Notebook/blob/master/_posts/2024-03-29-Zymo-SwitchFree.md) and the kit protocol above.
I'm using 20 ng of RNA input for the non-NEB treated samples, and 1.9 ng for the NEB-treated samples.

Here I'm using UDI primers from the 96 well plate (CAT. D3096, LOT. 250838) provided with the kit.

All samples were eluted in 15uL of elution buffer.

## Library prep
I ran the library prep protocol linked above. I used 19 PCR cycles for the non-NEB treated and 21 for the NEB-treated. With 6-8 samples, it takes about 6 hours to run the protocol and do QC on the final library.

Here's a breakdown of input RNA volume and quantity, samples with X are NEB-treated, with Y non-NEB treated:

| sample_id || RNA_QBIT_AVG (ng/uL) || RNA (uL) || Ultrapure water (uL) || Total input RNA (ng) |
| B8X     ||   0.574  ||  3.31 ||     1.69  ||       1.9       |
| C10X    ||   0.71    || 2.68  ||    2.32     ||      1.9       |
| C9X    ||   0.393   ||   5 ||   0    ||        1.9       |
| POC_R12_C3X || 0.42    || 4.52 ||   0.48  ||       1.9        |
| POC_R1_H1X  || 0.389 || 5   ||   0       ||    1.9    |
| POC_R3_C3X   ||  0.47   || 4.02 ||   0.98       ||   1.9     |
| B8Y     ||   21.2   ||  0.94 ||    4.06   ||       20       |
| C10Y    ||   23.7    || 0.84  ||     4.16   ||      20       |
| C9Y    ||   48.9    ||   0.41 ||   4.59    ||        20      |
| POC_R12_C3Y || 28.6    ||  0.7 ||   4.3  ||       20       |
| POC_R1_H1Y  || 24.6  ||   0.81  ||   4.19        ||   20    |
| POC_R3_C3Y   ||  17.7   ||   1.13 ||   3.87       ||   20     |

## Qubit Results
I used High Sensitivity dsDNA Qubit Protocol linked above. Library samples were read twice, standard only read once.
- Standard 1: 53.72
- Standard 2: 23477.17

| QBIT date  || sample_id  ||     Species    ||  Library read1 || Library read2  || Library_AVG (ng/ul) |
|  20250929  || B8X || *Montipora capitata*  || 0.54   || 0.538   || 0.539        |
|  20250929  || C10X   || *Montipora capitata* || 0.458 || 0.456   || 0.457        |
|  20250929  || C9X || *Montipora capitata*  || 0.992  || 0.972   || 0.982        |
|  20250929  || POC_R12_C3X  || *Pocillopora acuta* || 0.16   || 0.16   || 0.16         |
|  20250929  ||  POC_R1_H1X || *Pocillopora acuta*  || 0.232  || 0.228  || 0.23         |
|  20250929  || POC_R3_C3X  || *Pocillopora acuta* || LOW    || LOW    || LOW           |
|  20250929  || B8Y || *Montipora capitata*  || 0.176  || 0.174  || 0.175        |
|  20250929  || C10Y   || *Montipora capitata* || 0.594 || 0.596  || 0.595        |
|  20250929  || C9Y || *Montipora capitata*  || 0.238  || 0.23   || 0.234        |
|  20250929  || POC_R12_C3Y  || *Pocillopora acuta* || 0.132  || 0.132  || 0.132        |
|  20250929  ||  POC_R1_H1Y || *Pocillopora acuta*  || 0.104  || 0.11   || 0.107        |
|  20250929  || POC_R3_C3Y  || *Pocillopora acuta* || 0.134  || 0.128  || 0.131        |

## TapeStation
After the library prep, I run samples on the tapestation (D5000), protocol linked above.

| TapeStation date  || sample_id  ||  TapeStation conc. ng/uL ||   Primer set  |
|  20250929  || B8X || *Montipora capitata*  || 49  |
|  20250929|| C10X   || *Montipora capitata* || too low |
|  20250929  || C9X || *Montipora capitata*  || too low |
|  20250929  || POC_R12_C3X  || *Pocillopora acuta* || too low  |
|  20250929  ||  POC_R1_H1X || *Pocillopora acuta*  || too low |
|  20250929   || POC_R3_C3X  || *Pocillopora acuta* || too low |
|  20250929  || B8Y || *Montipora capitata*  || 57   |
|  20250929|| C10Y   || *Montipora capitata* || too low |
|  20250929  || C9Y || *Montipora capitata*  || too low |
|  20250929  || POC_R12_C3Y  || *Pocillopora acuta* || too low  |
|  20250929  ||  POC_R1_H1Y || *Pocillopora acuta*  || too low |
|  20250929   || POC_R3_C3Y  || *Pocillopora acuta* || too low|

![NEB_compare_library.png](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/NEB_compare_library.png?raw=true)
