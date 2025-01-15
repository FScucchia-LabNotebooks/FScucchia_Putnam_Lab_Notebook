---
layout: post
title: Library prep using Zymo SwitchFree kit - Hawaii TPC samples - 011525
date: '2025-01-15'
category: Protocol
tags: [DNA, Zymo, RNA, library]
---

#### Using the Zymo-Seq SwitchFree 3′ mRNA Library Kit for in-house library prep of the Hawaii TPC samples - 011525

**Protocols used**
- [Zymo-Seq SwitchFree 3′ mRNA Library Kit protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/_r3008_r3009__zymo_seq_switchfree_3_mrna_library_kit.pdf)
- [TapeStation protocol DNA D5000](https://github.com/meschedl/MESPutnam_Open_Lab_Notebook/blob/master/_posts/2019-07-30-DNA-Tapestation.md)
- [High Sensitivity dsDNA QBIT protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/MAN0017455_Qubit_1X_dsDNA_HS_Assay_Kit_UG.pdf)

Using the [Zymo-Seq SwitchFree 3′ mRNA Library Kit](https://www.zymoresearch.com/products/zymo-seq-switchfree-3-mrna-library-kit) (CAT.  R3009-A, LOT. 252649) to prepare libraries starting from RNA samples exctracted from adult coral fragments from the Hawaii TPC project. RNA extraction posts can be found [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-TPCA-Summary/).

For the library prep I followed the protocol of [Jill Ashey](https://github.com/JillAshey/JillAshey_Putnam_Lab_Notebook/blob/master/_posts/2024-03-29-Zymo-SwitchFree.md) and the kit protocol above.
The kit needs a minimum of 10 ng of total RNA or a maximum of 500 ng of total RNA. I'm using 13 ng of input RNA, since it's the amount the gave me the highest concentration of library with the first samples I tried prepping. 
I'm using 25 ng of RNA input, 13 ng and 55.5 ng didn't work well (see previous posts).

I've used the primers in the 96 well plate (CAT. D3096, LOT. 250838) provided with the kit. 
All samples were eluted in 20uL of elution buffer.

## Library prep
I ran the library prep protocol linked above. I used 21 PCR cycles.

Here's a breakdown of input RNA volume and quantity:

| sample_id || RNA_QBIT_AVG (ng/uL) || RNA (uL) || Ultrapure water (uL) || Total input RNA (ng) |
| Pcom-H10     ||     54.0         ||   0.42    ||        4.77         ||        25          |
| Pcom-G10      ||    51.8        ||   0.48    ||       4.52             ||        25          |
| Pacu-B1     ||     37.3     ||     0.67    ||         4.33            ||        25          |
| Mcap-B6      ||    12.9         ||    1.94    ||       3.06             ||        25          |
| Mcap-B10      ||   12.1          ||    2.07  ||        2.93             ||        25          |
| Mcap-B1      ||    18.6          ||   1.34    ||     3.66              ||      25          |
| Mcap-E9      ||    22.6          ||   1.11    ||     3.89              ||      25          |
| Pcom-E8     ||     48.1       ||    0.52     ||        4.48           ||        25          |

## Qubit Results
I used High Sensitivity dsDNA Qubit Protocol linked above. Library samples were read twice, standard only read once.
- Standard 1: 66.00
- Standard 2: 26812.77

| QBIT date  || sample_id  ||     Species       || Temp   ||  DNA read1 || DNA read2  || DNA_AVG (ng/ul) |
|  20250115  || Pcom-H10   || *Porites compressa*  || 26.8   ||   2.26       ||   2.26      ||  2.26        |
|  20250115 || Pcom-G10   || *Porites compressa* || 26.8     ||  1.2    ||    1.22      ||  1.21         |
|  20250115    || Pacu-B1   || *Pocillopora acuta*  || 18   ||    1.41   ||   1.38     ||  1.395       |
|  20250115    || Mcap-B6    || *Montipora capitata* || 12   ||   1.66  ||    1.62      ||  1.64        |
|  20250115   || Mcap-B10    || *Montipora capitata*  ||  26.8 || 1.4   ||  1.35    ||  1.375       |
|  20250115   || Mcap-B1   || *Montipora capitata* ||  18   ||   1.45      ||   1.40       ||  1.425      |
|  20250115   || Mcap-E9    || *Montipora capitata*  || 30   ||  0.789    ||  0.77    ||  0.7795      |
|  20250115   || Pcom-E8   || *Porites compressa* ||  25   ||   1.62     ||   1.55     ||  1.585      |

## TapeStation
After the library prep, I run samples on the tapestation (D5000), protocol linked above.

| TapeStation date  || sample_id  ||     Species       || Temp   || TapeStation conc. ||   Primer set  |
|  20250115  || Pcom-H10   || *Porites compressa*  || 26.8   || 4.07    ||   31    |
|  20250115 || Pcom-G10    || *Porites compressa* || 26.8   || 1.8    ||    32    |
|  20250115  || Pacu-B1   || *Pocillopora acuta*  ||  18 ||  1.94   ||     33   |
|  20250115  || Mcap-B6   || *Montipora capitata* ||  12   || 2.87    ||      34    |
|  20250115   || Mcap-B10   || *Montipora capitata*  ||  26.8  || 1.91   ||  35      |
|  20250115   || Mcap-B1    || *Montipora capitata* ||  18   ||  2.35    ||     36    |
|  20250115   || Mcap-E9    || *Montipora capitata*  ||  30   ||  1.07   ||    37      |
|  20250115   || Pcom-E8    || *Porites compressa* ||  25   ||  3.12   ||     38    |

![LibPrepRun5_complete.png](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/LibPrepRun5_complete.png?raw=true)

 - _Things to consider for next time_: Only one sample, Pcom-H10, seems to have enough concentration for the sequencing (>2 ng/ul). Something during this run of library prep maybe went wrong? Will re-do the other 7 samples.