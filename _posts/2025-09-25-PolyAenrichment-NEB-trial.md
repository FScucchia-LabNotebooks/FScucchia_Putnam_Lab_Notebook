---
layout: post
title: Trying the NEB Poly(A) mRNA enrichment prior library prep - 092525
date: '2025-09-25'
category: Protocol
tags: [PolyA, NEB, RNA, library]
---

#### Using the NEBNext Poly(A) Magnetic Isolation Module to isolate mRNA prior in-house library prep

**Protocols used**
- [NEBNext Poly(A) Magnetic Isolation Module](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/NEBPolyA.pdf)
- [TapeStation protocol High Sensitivity RNA](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/HS-RNA_QuickGuide_TapeStation.pdf)
- [High Sensitivity RNA QBIT protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/Qubit_RNA_HS_Assay_UG.pdf)

Using the [NEBNext Poly(A) Magnetic Isolation Module](https://www.neb.com/en-us/products/e7490-nebnext-polya-mrna-magnetic-isolation-module) to isolate intact poly(A)+RNA from previously isolated total RNA. The idea is to use this kit before performing the library prep with the Zymo SwitchFree kit, and try to reduce the amount of rRNA present in the libraries.

The RNA samples I'm using here are from _Montipora capitata_ spat (posts [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-McapSpat2/), [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-McapSpat3/) and [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-McapSpat1/)) and from _Pocillopora acuta_ adults ([Zoe's samples](https://zdellaert.github.io/ZD_Putnam_Lab_Notebook/Switch-Free-TimeSeries-Library-Prep-Test/))

I followed the kit protocol linked above (express protocol, pages 1-3) and used 30ng of input RNA. The kit is designed to isolate intact poly(A)+ RNA from 1-5µg of previously isolated total RNA.

All samples were eluted in 15uL of elution buffer (NEBNext Tris Buffer).

## Sample prep

Here's a breakdown of input RNA volume and quantity (the kit requires a total starting volume of 50uL):

| sample_id || RNA_QBIT_AVG (ng/uL) || RNA (uL) || Ultrapure water (uL) || Total input RNA (ng) |
| B8     ||   21.2   ||   1.42 ||     48.58   ||       30       |
| C10    ||   23.7    || 1.27  ||     48.73     ||      30       |
| C9    ||   48.9    ||   0.61 ||   49.39    ||        30       |
| POC_R12_C3 || 28.6    ||  1.05 ||   48.95  ||       30        |
| POC_R1_H1  || 24.6  ||   1.22  ||   48.78        ||       30    |
| POC_R3_C3   ||  17.7   ||   1.69 ||   48.31       ||   30     |

## Qubit Results
I used High Sensitivity RNA Qubit Protocol linked above. RNA samples were read twice, standard only read once.
- Standard 1: 48.04   
- Standard 2: 939.78

| QBIT date  || sample_id  ||     Species       || RNA_read1 ||RNA_read2 |
|  20250925  || B8 || *Montipora capitata*  || too low (out of range)  ||   too low   |
|  20250925|| C10   || *Montipora capitata* || too low ||  too low    |
|  20250925  || C9 || *Montipora capitata*  || too low ||   too low     |
|  20250925  || POC_R12_C3  || *Pocillopora acuta* || too low  ||  too low   |
|  20250925  ||  POC_R1_H1 || *Pocillopora acuta*  || too low ||  too low    |
|  20250925   || POC_R3_C3  || *Pocillopora acuta* || too low||  too low    |

## TapeStation
After the isolation, I run samples on the tapestation, protocol linked above.
See full report [here](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/docs/2025-09-25_NEB_PolyA_trial.pdf).

| TapeStation date  || sample_id  ||  TapeStation conc. ng/uL |
|  20250925 || B8 ||  0.574  |
|  20250925 || C10   ||  0.71  |
|  20250925  || C9 ||   0.393  |
|  20250925  || R12 ||  0.42  |
|  20250925  || R1 ||   0.389  |
|  20250925   || R3 || 0.473 |


