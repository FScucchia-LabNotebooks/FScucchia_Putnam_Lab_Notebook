---
layout: post
title: Library prep using Zymo SwitchFree kit - Hawaii TPC samples - 011125
date: '2025-01-11'
category: Protocol
tags: [DNA, Zymo, RNA, library]
---

#### Using the Zymo-Seq SwitchFree 3′ mRNA Library Kit for in-house library prep of the Hawaii TPC samples - 011125

**Protocols used**
- [Zymo-Seq SwitchFree 3′ mRNA Library Kit protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/_r3008_r3009__zymo_seq_switchfree_3_mrna_library_kit.pdf)
- [TapeStation protocol DNA D5000](https://github.com/meschedl/MESPutnam_Open_Lab_Notebook/blob/master/_posts/2019-07-30-DNA-Tapestation.md)
- [QBIT protocol](https://github.com/meschedl/MESPutnam_Open_Lab_Notebook/blob/master/_posts/2019-03-08-Qubit-Protocol.md)

Using the [Zymo-Seq SwitchFree 3′ mRNA Library Kit](https://www.zymoresearch.com/products/zymo-seq-switchfree-3-mrna-library-kit) (CAT.  R3009-A, LOT. 252649) to prepare libraries starting from RNA samples exctracted from adult coral fragments from the Hawaii TPC project. RNA extraction posts can be found [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-TPCA-Summary/).

For the library prep I followed the protocol of [Jill Ashey](https://github.com/JillAshey/JillAshey_Putnam_Lab_Notebook/blob/master/_posts/2024-03-29-Zymo-SwitchFree.md) and the kit protocol above.
The kit needs a minimum of 10 ng of total RNA or a maximum of 500 ng of total RNA. I'm using the max volume of RNA input (5 ul) for the sample with the lowest RNA concentration among all, which is 11.1 ng/uL, which corresponds to a total of _55.5 ng_. I will use this 55.5 as inpout for all other samples. 

I've used the primers in the 96 well plate (CAT. D3096, LOT. 250838) provided with the kit. For sample Pacu-E9, I've used UDI primer 11 from the 12 prep kit (CAT. D3008, LOT. 250968), as I've used the day before primer 11 from the 96 plate.
All samples were eluted in 20uL of elution buffer.

## Library prep
I ran the library prep protocol linked above. I used 20 PCR cycles.

Here's a breakdown of input RNA volume and quantity:

| sample_id || RNA_QBIT_AVG (ng/uL) || RNA (uL) || Ultrapure water (uL) || Total input RNA (ng) |
| Pacu-E9      ||   64.0           ||    0.87     ||        4.13           ||        55.5          |
| Pacu-H1      ||    20.5           ||   2.71     ||        2.29             ||        55.5          |
| Mcap-G1     ||   53.9           ||    1.03     ||        3.97             ||        55.5          |
| Pcom-E1      ||    18.7           ||    2.97     ||        2.03             ||        55.5          |
| Pcom-B7      ||    22.6           ||    2.46     ||        2.54             ||        55.5          |
| Pacu-H8      ||    27.1           ||    2.05     ||        2.95             ||        55.5          |
| Pacu-G1     ||   60.3           ||    0.92     ||        4.08             ||        55.5          |
| Pcom-E10      ||   27.2           ||    2.04    ||        2.96             ||        55.5          |

I'm re-doing sample Pacu-E9 from the day before. This time I'm using UDI primer 11 from the 12prep kit (CAT. D3008, LOT. 250968).

## Qubit Results
I used Broad range dsDNA Qubit Protocol inked above. DNA samples were read twice, standard only read once.
- Standard 1: 
- Standard 2: 

| QBIT date  || sample_id  ||     Species       || Temp   ||  DNA read1 || DNA read2  || DNA_AVG (ng/ul) |
|  20250111  || Pacu-E9   || *Pocillopora acuta*  || 30   ||       ||            ||            |
|  20250111 || Pacu-H1    || *Pocillopora acuta* || 18     ||     ||           ||      |
|  20250111    || Mcap-G1   || *Montipora capitata*  ||  18   ||    ||           ||  |
|  20250111    || Pcom-E1   || *Porites compressa* ||  18   ||    ||           ||   |
|  20250111   || Pcom-B7     || *Porites compressa*  ||  35   ||    ||            ||   |
|  20250111   || Pacu-H8    || *Pocillopora acuta* ||  25   ||      ||          ||  |
|  20250111   || Pacu-G1   || *Pocillopora acuta*  ||  18   ||     ||         ||   |
|  20250111   || Pcom-E10    || *Porites compressa*  ||  26.8   ||    ||           ||   |


## TapeStation
After the library prep, I run samples on the tapestation (D5000), protocol linked above.

| TapeStation date  || sample_id  ||     Species       || Temp   || TapeStation conc. ||   Primer set  |
|  20250111  || Pacu-E9   || *Pocillopora acuta*  || 30   ||       ||     11       |
|  20250111 || Pacu-H1    || *Pocillopora acuta* || 18     ||     ||       12    |
|  20250111    || Mcap-G1   || *Montipora capitata*  ||  18   ||    ||     13      |
|  20250111    || Pcom-E1   || *Porites compressa* ||  18   ||    ||       14    |
|  20250111   || Pcom-B7     || *Porites compressa*  ||  35   ||    ||      15      |
|  20250111   || Pacu-H8    || *Pocillopora acuta* ||  25   ||      ||      16    |
|  20250111   || Pacu-G1   || *Pocillopora acuta*  ||  18   ||     ||      17   |
|  20250111   || Pcom-E10    || *Porites compressa*  ||  26.8   ||    ||   18        |

![LibPrepRun2_complete.png](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/LibPrepRun2_complete.png?raw=true)

 - _Things to consider for next time_: I
