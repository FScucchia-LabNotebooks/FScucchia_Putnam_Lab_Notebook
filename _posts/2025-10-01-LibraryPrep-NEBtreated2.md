---
layout: post
title: Library prep using Zymo SwitchFree kit on samples with PolyA isolation - 100125
date: '2025-10-01'
category: Protocol
tags: [DNA, Zymo, RNA, library]
---

#### Using the Zymo-Seq SwitchFree 3′ mRNA Library Kit for in-house library prep of samples treated for PolyA isolation - 100125

**Protocols used**
- [Zymo-Seq SwitchFree 3′ mRNA Library Kit protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/_r3008_r3009__zymo_seq_switchfree_3_mrna_library_kit.pdf)
- [NEBNext Poly(A) Magnetic Isolation Module](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/NEBPolyA.pdf)
- [TapeStation protocol DNA D5000](https://github.com/meschedl/MESPutnam_Open_Lab_Notebook/blob/master/_posts/2019-07-30-DNA-Tapestation.md)
- [High Sensitivity dsDNA QBIT protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/MAN0017455_Qubit_1X2_dsDNA_HS_Assay_Kit_UG.pdf)

Using the [Zymo-Seq SwitchFree 3′ mRNA Library Kit](https://www.zymoresearch.com/products/zymo-seq-switchfree-3-mrna-library-kit)(CAT.  R3009-A, LOT. 252649) to prepare libraries starting from RNA samples exctracted from adult coral fragments and spat. RNA extraction posts can be found [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-McapSpat2/), [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-McapSpat3/) and [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-McapSpat1/), and in Zoe's notebook ([here](https://zdellaert.github.io/ZD_Putnam_Lab_Notebook/Switch-Free-TimeSeries-Library-Prep-Test/)).
NEB treatment post can be found [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/PolyAenrichment-NEB-trial/).

The idea is to use the NEB kit before performing the library prep to reduce the amount of rRNA present in the libraries. Libraries of the same samples non-NEB treated will be also prepared in parallel.

The [first trial](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/LibraryPrep-NEBtreated/) of this protocol didn't work, the number of PCR cycles was probably too low. I'm trying again increasing the number of cycles.

For the library prep I followed the protocol of [Jill Ashey](https://github.com/JillAshey/JillAshey_Putnam_Lab_Notebook/blob/master/_posts/2024-03-29-Zymo-SwitchFree.md) and the kit protocol above.
I'm using 20 ng of RNA input for the non-NEB treated samples, and 1.9 ng for the NEB-treated samples.

Here I'm using UDI primers from the 96 well plate (CAT. D3096, LOT. 250838) provided with the kit.

All samples were eluted in 15uL of elution buffer.

## Library prep
I ran the library prep protocol linked above. I used 21 PCR cycles for the non-NEB treated and 23 for the NEB-treated. With 6-8 samples, it takes about 6 hours to run the protocol and do QC on the final library.

Here's a breakdown of input RNA volume and quantity, samples with X2 are NEB-treated, with Y2 non-NEB treated:

| sample_id || RNA_QBIT_AVG (ng/uL) || RNA (uL) || Ultrapure water (uL) || Total input RNA (ng) |
| B8X2     ||   0.574  ||  3.31 ||     1.69  ||       1.9       |
| C10X2    ||   0.71    || 2.68  ||    2.32     ||      1.9       |
| C9X2    ||   0.393   ||   5 ||   0    ||        1.9       |
| POC_R12_C3X2 || 0.42    || 4.52 ||   0.48  ||       1.9        |
| POC_R1_H1X2  || 0.389 || 5   ||   0       ||    1.9    |
| POC_R3_C3X2   ||  0.47   || 4.02 ||   0.98       ||   1.9     |
| B8Y2     ||   21.2   ||  0.94 ||    4.06   ||       20       |
| C10Y2    ||   23.7    || 0.84  ||     4.16   ||      20       |
| C9Y2    ||   48.9    ||   0.41 ||   4.59    ||        20      |
| POC_R12_C3Y2 || 28.6    ||  0.7 ||   4.3  ||       20       |
| POC_R1_H1Y2  || 24.6  ||   0.81  ||   4.19        ||   20    |
| POC_R3_C3Y2   ||  17.7   ||   1.13 ||   3.87       ||   20     |

## Qubit Results
I used High Sensitivity dsDNA Qubit Protocol linked above. Library samples were read twice, standard only read once.
- Standard 1: 58.50
- Standard 2: 24225.64

| QBIT date  || sample_id  ||     Species    ||  Library read1 || Library read2  || Library_AVG (ng/ul) |
|  20251001 || B8X2 || *Montipora capitata*  || 0.356  || 0.342  || 0.349        |
|  20251001 || C10X2   || *Montipora capitata* || 1.04   || 1     || 1.02         |
|  20251001 || C9X2 || *Montipora capitata*  || 0.428  || 0.42   || 0.424        |
|  20251001 || POC_R12_C3X2  || *Pocillopora acuta* || 0.738  || 0.731  || 0.7345      |
|  20251001 ||  POC_R1_H1X2 || *Pocillopora acuta*  || 0.872  || 0.869  || 0.8705      |
|  20251001 || POC_R3_C3X2  || *Pocillopora acuta* || 0.2    || 0.191  || 0.1955      |
|  20251001 || B8Y2 || *Montipora capitata*  || 0.118  || 0.111  || 0.1145      |
|  20251001 || C10Y2   || *Montipora capitata* || 0.104  || 0.102  || 0.103        |
|  20251001 || C9Y2 || *Montipora capitata*  || LOW    || LOW    || none         |
|  20251001 || POC_R12_C3Y2  || *Pocillopora acuta* || LOW    || LOW    || none         |
|  20251001 ||  POC_R1_H1Y2 || *Pocillopora acuta*  || LOW    || LOW    || none         |
|  20251001 || POC_R3_C3Y2  || *Pocillopora acuta* || LOW    || LOW    || none         |

## TapeStation
After the library prep, I run samples on the tapestation (D5000), protocol linked above.
Full tapestation report [here](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/docs/2025-10-01%20-%20NEB_regular_trial2.pdf)

| TapeStation date  || sample_id  ||  TapeStation conc. ng/uL ||   Primer set  |
|  20251001 || B8X2 || 0.249  || 1  |
|  20250929|| C10X2   || 0.756|| 2 |
|  20251001 || C9X2 || 0.554 || 3 |
|  20251001 || POC_R12_C3X2  || 0.768 || 4  |
|  20251001 ||  POC_R1_H1X2 || 1.06  || 5 |
|  20251001  || POC_R3_C3X2  || 0.076 || 6 |
|  20251001 || B8Y2 || 0.041  || 9   |
|  20250929|| C10Y2   || / || 10|
|  20251001 || C9Y2 || /  || 11 |
|  20251001 || POC_R12_C3Y2  || / || 12  |
|  20251001 ||  POC_R1_H1Y2 || 0.071 || 13 |
|  20251001  || POC_R3_C3Y2  || / || 14 |

![NEB_compare_library2.png](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/NEB_compare_library2.png?raw=true)
