---
layout: post
title: Library prep using Zymo SwitchFree kit - Hawaii TPC samples - 012425
date: '2025-01-24'
category: Protocol
tags: [DNA, Zymo, RNA, library]
---

#### Using the Zymo-Seq SwitchFree 3′ mRNA Library Kit for in-house library prep of the Hawaii TPC samples - 012425

**Protocols used**
- [Zymo-Seq SwitchFree 3′ mRNA Library Kit protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/_r3008_r3009__zymo_seq_switchfree_3_mrna_library_kit.pdf)
- [TapeStation protocol DNA D5000](https://github.com/meschedl/MESPutnam_Open_Lab_Notebook/blob/master/_posts/2019-07-30-DNA-Tapestation.md)
- [High Sensitivity dsDNA QBIT protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/MAN0017455_Qubit_1X_dsDNA_HS_Assay_Kit_UG.pdf)

Using the [Zymo-Seq SwitchFree 3′ mRNA Library Kit](https://www.zymoresearch.com/products/zymo-seq-switchfree-3-mrna-library-kit) (CAT.  R3009-A, LOT. 252649) to prepare libraries starting from RNA samples exctracted from adult coral fragments from the Hawaii TPC project. RNA extraction posts can be found [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-TPCA-Summary/).

For the library prep I followed the protocol of [Jill Ashey](https://github.com/JillAshey/JillAshey_Putnam_Lab_Notebook/blob/master/_posts/2024-03-29-Zymo-SwitchFree.md) and the kit protocol above.
The kit needs a minimum of 10 ng of total RNA or a maximum of 500 ng of total RNA.
I'm using 20 ng of RNA input, 13 ng, 30 ng and 55.5 ng didn't work well. 25 ng has worked for only some of the samples (see previous posts).
Skipping the step in the Zymo protocol that says "for low quality RNA" worked with the last batch of samples (see post of 23rd), so I will try again with these samples skipping it.

I've used the primers in the 96 well plate (CAT. D3096, LOT. 250838) provided with the kit. 
All samples were eluted in 18uL of elution buffer.

## Library prep
I ran the library prep protocol linked above. I used 21 PCR cycles. With 6-8 samples, it takes about 6 hours to run the protocol and do QC on the final library.
I've re-prepped the following samples, that had failed on the 22nd, skipping the "low quality RNA" step according to the Zymo kit protocol above.

Here's a breakdown of input RNA volume and quantity:

| sample_id || RNA_QBIT_AVG (ng/uL) || RNA (uL) || Ultrapure water (uL) || Total input RNA (ng) |
| Mcap-F8     ||   29.1     ||   1.03    ||     3.97       ||        30         |
| Pcom-G9     ||   62.9     ||   0.48  ||      4.52           ||        30         |
| Pcom-F10    ||   44.0     ||   0.68  ||      4.32           ||        30         |
| Pacu-E8     ||  25.8      ||  1.16  ||      3.84           ||        30         |
| Pacu-H6     ||  36.5     ||   0.82  ||    4.18            ||        30         |
| Pcom-H9     ||  47.1     ||   0.64    ||    4.36             ||      30         |

## Qubit Results
I used High Sensitivity dsDNA Qubit Protocol linked above. Library samples were read twice, standard only read once.
- Standard 1: 66.02  
- Standard 2: 26117.11 

| QBIT date  || sample_id  ||     Species       || Temp   ||  DNA read1 || DNA read2  || DNA_AVG (ng/ul) |
|  20250123 || Mcap-G9 || *Montipora capitata*  || 30   || 0.479   || 0.466     || 0.4725            |
|  20250123 || Mcap-H6   || *Montipora capitata* || 12    || 2.45  ||  2.33    || 2.39            |
|  20250123 || Mcap-E10 || *Montipora capitata*  || 26.8 ||   1.25       ||  1.22   || 1.235            |
|  20250123 || Pcom-F6  || *Porites compressa* || 12   ||  4.11     ||    4.0      || 4.055            |
|  20250123  || Pacu-G7 || *Pocillopora acuta*  ||  35 ||   14.2    ||   13.8      || 14.0            |
|  20250123  || Pcom-H1  || *Porites compressa* ||  18  ||  4.95   ||   4.74      || 4.845            |

## TapeStation
After the library prep, I run samples on the tapestation (D5000), protocol linked above.

| TapeStation date  || sample_id  ||     Species       || Temp   || TapeStation conc. ||   Primer set  |
|  20250123 || Mcap-G9   || *Montipora capitata*  || 30   || 0.491    ||   45    |
|  20250123 || Mcap-H6    || *Montipora capitata* || 12   || 3.11     ||    46    |
|  20250123 || Mcap-E10  || *Montipora capitata*  || 26.8 || 1.96     ||    47   |
|  20250123 || Pcom-F6   || *Porites compressa* ||  12   ||  5.50    ||     48    |
|  20250123  || Pacu-G7   || *Pocillopora acuta*  ||  35  ||  7.66   ||  49      |
|  20250123  || Pcom-H1    || *Porites compressa* ||  18   || 7.14    ||  50   |

![LibPrepRun7_complete.png](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/LibPrepRun7_complete.png?raw=true)

 - _Things to consider for next time_: skipping the step in the Zymo protocol that says "for low quality RNA" worked much better! I got higher concentrations that previous preps, altough some of the samples have weird peaks (see TapeStation results). I'll try again skipping that step with samples that didn't work before and see what happens.