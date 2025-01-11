---
layout: post
title: Library prep using Zymo SwitchFree kit - Hawaii TPC samples - 011025
date: '2025-01-10'
category: Protocol
tags: [DNA, Zymo, RNA, library]
---

#### Using the Zymo-Seq SwitchFree 3′ mRNA Library Kit for in-house library prep of the Hawaii TPC samples - 011025

**Protocols used**
- [Zymo-Seq SwitchFree 3′ mRNA Library Kit protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/_r3008_r3009__zymo_seq_switchfree_3_mrna_library_kit.pdf)
- [TapeStation protocol DNA D5000](https://github.com/meschedl/MESPutnam_Open_Lab_Notebook/blob/master/_posts/2019-07-30-DNA-Tapestation.md)
- [QBIT protocol](https://github.com/meschedl/MESPutnam_Open_Lab_Notebook/blob/master/_posts/2019-03-08-Qubit-Protocol.md)

Using the [Zymo-Seq SwitchFree 3′ mRNA Library Kit](https://www.zymoresearch.com/products/zymo-seq-switchfree-3-mrna-library-kit)(CAT.  R3009-A, LOT. 252649) to prepare libraries starting from RNA samples exctracted from adult coral fragments from the Hawaii TPC project. RNA extraction posts can be found [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-TPCA-Summary/).

For the library prep I followed the protocol of [Jill Ashey](https://github.com/JillAshey/JillAshey_Putnam_Lab_Notebook/blob/master/_posts/2024-03-29-Zymo-SwitchFree.md) and the kit protocol above.
The kit needs a minimum of 10 ng of total RNA or a maximum of 500 ng of total RNA. I'm using the max volume of RNA input (5 ul) for the sample with the lowest RNA concentration among all, which is 11.1 ng/uL, which corresponds to a total of _55.5 ng_. I will use this 55.5 as inpout for all other samples. 

I've used the primers in the 96 well plate (CAT. D3096, LOT. 250838) provided with the kit. 
All samples were eluted in 20uL of elution buffer.

## Library prep
I ran the library prep protocol linked above. I used 19 PCR cycles.

Here's a breakdown of input RNA volume and quantity:

| sample_id || RNA_QBIT_AVG (ng/uL) || RNA (uL) || Ultrapure water (uL) || Total input RNA (ng) |
| Pacu-H10      ||   19.5           ||    2.85     ||        2.15             ||        55.5          |
| Mcap-H1      ||    41.5           ||    1.34     ||        3.66             ||        55.5          |
| Pcomp-G8      ||   36.1           ||    1.54     ||        3.46             ||        55.5          |
| Mcap-E8      ||    25.4           ||    2.19     ||        2.81             ||        55.5          |
| Pacu-B8      ||    23.5           ||    2.36     ||        2.64             ||        55.5          |
| Mcap-B7      ||    24.2           ||    2.29     ||        2.71             ||        55.5          |
| Pcomp-G1     ||   30.9           ||    1.80     ||        3.20             ||        55.5          |
| Pacu-E9      ||   64.0           ||    0.87     ||        4.13             ||        55.5          |


## Qubit Results
I used Broad range dsDNA Qubit Protocol inked above. DNA samples were read twice, standard only read once.
- Standard 1: 181.49
- Standard 2: 30941.59

| QBIT date  || sample_id  ||     Species       || Temp   ||  DNA read1 || DNA read2  || DNA_AVG (ng/ul) |
|  20250110  || Pacu-H10   || *Pocillopora acuta*  || 26.8   ||  8    ||    8.38        ||    8.19        |
|  20250110  || Mcap-H1    || *Montipora capitata* || 18     ||  LOW   ||  LOW          ||    LOW |
|  20250110    || Pcomp-G8   || *Porites compressa*  ||  25   ||  6.14  ||   5.76        || 5.95 |
|  20250110    || Mcap-E8    || *Montipora capitata* ||  25   || LOW   ||   LOW         ||  LOW |
|  20250110    || Pacu-B8    || *Pocillopora acuta*  ||  25   ||  2.86  ||   2.94         || 2.9 |
|  20250110    || Mcap-B7    || *Montipora capitata* ||  35   ||  2.50   ||  2.86        || 2.68 |
|  20250110    || Pcomp-G1   || *Porites compressa*  ||  18   ||  3.6  ||    3.64       || 3.62 |
|  20250110    || Pacu-E9    || *Pocillopora acuta*  ||  30   || LOW   ||    LOW        ||  LOW |


## TapeStation
After the library prep, I run samples on the tapestation (D5000), protocol linked above.

| Library prep date  || sample_id  ||     Species       || Temp   || TapeStation conc. ||   Primer set  |
|  20250110  || Pacu-H10   || *Pocillopora acuta*  || 26.8      ||    7.12       ||    3           |
|  20250110  || Mcap-H1    || *Montipora capitata* || 18       ||     1.85            ||   4            |
|  20250110    || Pcomp-G8   || *Porites compressa*  ||  25      ||   5.38         ||   5            |
|  20250110    || Mcap-E8    || *Montipora capitata* ||  25      ||    2.01        ||   6            |
|  20250110    || Pacu-B8    || *Pocillopora acuta*  ||  25      ||    2.77       ||   8            |
|  20250110    || Mcap-B7    || *Montipora capitata* ||  35      ||    2.94       ||   9            |
|  20250110    || Pcomp-G1   || *Porites compressa*  ||  18      ||    4.06     ||   10            |
|  20250110    || Pacu-E9    || *Pocillopora acuta*  ||  30      ||    1.98      ||   11            |

![LibPrepRun1_complete.png](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/LibPrepRun1_complete.png?raw=true)


 - _Things to consider for next time_: I got pretty low concentrations, next time I will use 20 PCR cycles instead of 19. I will also use the high sensitivity assay for the QBIT, since the broad range doesn't always give the concentration. Samples Pacu-E9 is the one that look the worst (both from the TapeStation and the qbit) so I will re-do this sample on the 01/11.

