---
layout: post
title: Library prep using Zymo SwitchFree kit - Hawaii TPC samples - 011325
date: '2025-01-13'
category: Protocol
tags: [DNA, Zymo, RNA, library]
---

#### Using the Zymo-Seq SwitchFree 3′ mRNA Library Kit for in-house library prep of the Hawaii TPC samples - 011325

**Protocols used**
- [Zymo-Seq SwitchFree 3′ mRNA Library Kit protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/_r3008_r3009__zymo_seq_switchfree_3_mrna_library_kit.pdf)
- [TapeStation protocol DNA D5000](https://github.com/meschedl/MESPutnam_Open_Lab_Notebook/blob/master/_posts/2019-07-30-DNA-Tapestation.md)
- [High Sensitivity dsDNA QBIT protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/MAN0017455_Qubit_1X_dsDNA_HS_Assay_Kit_UG.pdf)

Using the [Zymo-Seq SwitchFree 3′ mRNA Library Kit](https://www.zymoresearch.com/products/zymo-seq-switchfree-3-mrna-library-kit) (CAT.  R3009-A, LOT. 252649) to prepare libraries starting from RNA samples exctracted from adult coral fragments from the Hawaii TPC project. RNA extraction posts can be found [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-TPCA-Summary/).

For the library prep I followed the protocol of [Jill Ashey](https://github.com/JillAshey/JillAshey_Putnam_Lab_Notebook/blob/master/_posts/2024-03-29-Zymo-SwitchFree.md) and the kit protocol above.
The kit needs a minimum of 10 ng of total RNA or a maximum of 500 ng of total RNA. I'm using 13 ng of input RNA, since it's the amount the gave me the highest concentration of library with the first samples I tried prepping. 
_Note:_ Using more input RNA (55.5 ng) got me low library concentration (<2n ng/ul) for many samples so far. Maybe issue with contaminants inhibiting PCR?

I've used the primers in the 96 well plate (CAT. D3096, LOT. 250838) provided with the kit. For sample Pacu-H1, I've used UDI primer 12 from the 12 prep kit (CAT. D3008, LOT. 250968), as I've used the day before primer 12 from the 96 plate.
All samples were eluted in 20uL of elution buffer.

## Library prep
I ran the library prep protocol linked above. I used 21 PCR cycles.

Here's a breakdown of input RNA volume and quantity:

| sample_id || RNA_QBIT_AVG (ng/uL) || RNA (uL) || Ultrapure water (uL) || Total input RNA (ng) |
| Pacu-H1      ||   20.5           ||    0.64     ||        4.37           ||        13          |
| Pacu-F8      ||   17.9           ||   0.73     ||        4.27             ||        13          |
| Pcom-F8     ||    14.4          ||     0.90    ||         4.10            ||        13          |
| Mcap-G6      ||    21.2           ||   0.61     ||        4.39             ||        13          |
| Mcap-H9      ||    27.6          ||   0.47     ||        4.53             ||        13          |
| Pcom-H6      ||    16.2           ||   0.80     ||        4.20             ||        13          |
| Pcom-B6     ||    21.2           ||     0.61    ||         4.39            ||        13          |
| Mcap-B9      ||   18.7           ||    0.70    ||         4.30            ||        13          |

I'm re-doing sample Pacu-E9 from the day before. This time I'm using UDI primer 11 from the 12prep kit (CAT. D3008, LOT. 250968).

## Qubit Results
I used High Sensitivity dsDNA Qubit Protocol linked above. Library samples were read twice, standard only read once.
- Standard 1: 70.54 
- Standard 2: 27629.65

| QBIT date  || sample_id  ||     Species       || Temp   ||  DNA read1 || DNA read2  || DNA_AVG (ng/ul) |
|  20250113  || Pacu-H1   || *Pocillopora acuta*  || 18   ||  0.476          ||    0.376     ||  0.426         |
|  20250113 || Pacu-F8    || *Pocillopora acuta* || 25     ||     1.06       ||   0.91       ||  0.985         |
|  20250113    || Pcom-F8   || *Porites compressa*  ||  25   ||   3.31         ||   2.99      ||  3.15          |
|  20250113    || Mcap-G6   || *Montipora capitata* ||  12   ||  2.61         ||   2.31       ||  2.46          |
|  20250113   || Mcap-H9     || *Montipora capitata*  ||  30   ||  1.31      ||   1.18    ||  1.245         |
|  20250113   || Pcom-H6    || *Porites compressa* ||  12   ||    1.68        ||   1.57          ||  1.625         |
|  20250113   || Pcom-B6   || *Porites compressa*  ||  12   ||   LOW         ||   LOW          ||  LOW           |
|  20250113   || Mcap-B9    || *Montipora capitata*  ||  30   ||   0.299         ||  0.301    ||  0.3           |

## TapeStation
After the library prep, I run samples on the tapestation (D5000), protocol linked above.

| TapeStation date  || sample_id  ||     Species       || Temp   || TapeStation conc. ||   Primer set  |
|  20250113  || Pacu-H1   || *Pocillopora acuta*  || 18   ||   0.746    ||     12       |
|  20250113 || Pacu-F8    || *Pocillopora acuta* || 25     ||   1.84  ||       19    |
|  20250113    || Pcom-F8   || *Porites compressa*  ||  25   || 5.02   ||     20     |
|  20250113    || Mcap-G6   || *Montipora capitata* ||  12   ||  4.55 ||      21    |
|  20250113   || Mcap-H9     || *Montipora capitata*  ||  30   ||  2.48  ||    22      |
|  20250113   || Pcom-H6    || *Porites compressa* ||  12   ||  2.88    ||     23    |
|  20250113   || Pcom-B6   || *Porites compressa*  ||  12   ||  0.034   ||      24   |
|  20250113   || Mcap-B9    || *Montipora capitata*  ||  30   ||  0.6 ||   25      |

![LibPrepRun3_complete.png](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/LibPrepRun3_complete.png?raw=true)

 - _Things to consider for next time_: Decreasing the input RNA didn't help, samples look worse. I will increase the input again to 25ng, and keep 21 PCR cycles.
