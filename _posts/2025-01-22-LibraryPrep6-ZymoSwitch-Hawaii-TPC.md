---
layout: post
title: Library prep using Zymo SwitchFree kit - Hawaii TPC samples - 012225
date: '2025-01-22'
category: Protocol
tags: [DNA, Zymo, RNA, library]
---

#### Using the Zymo-Seq SwitchFree 3′ mRNA Library Kit for in-house library prep of the Hawaii TPC samples - 012225

**Protocols used**
- [Zymo-Seq SwitchFree 3′ mRNA Library Kit protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/_r3008_r3009__zymo_seq_switchfree_3_mrna_library_kit.pdf)
- [TapeStation protocol DNA D5000](https://github.com/meschedl/MESPutnam_Open_Lab_Notebook/blob/master/_posts/2019-07-30-DNA-Tapestation.md)
- [High Sensitivity dsDNA QBIT protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/MAN0017455_Qubit_1X_dsDNA_HS_Assay_Kit_UG.pdf)

Using the [Zymo-Seq SwitchFree 3′ mRNA Library Kit](https://www.zymoresearch.com/products/zymo-seq-switchfree-3-mrna-library-kit) (CAT.  R3009-A, LOT. 252649) to prepare libraries starting from RNA samples exctracted from adult coral fragments from the Hawaii TPC project. RNA extraction posts can be found [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-TPCA-Summary/).

For the library prep I followed the protocol of [Jill Ashey](https://github.com/JillAshey/JillAshey_Putnam_Lab_Notebook/blob/master/_posts/2024-03-29-Zymo-SwitchFree.md) and the kit protocol above.
The kit needs a minimum of 10 ng of total RNA or a maximum of 500 ng of total RNA.
I'm using 30 ng of RNA input, 13 ng and 55.5 ng didn't work well. 25 ng has worked for only some of the samples (see previous posts).

I've used the primers in the 96 well plate (CAT. D3096, LOT. 250838) provided with the kit. 
All samples were eluted in 20uL of elution buffer.

## Library prep
I ran the library prep protocol linked above. I used 21 PCR cycles. With 6-8 samples, it takes about 6 hours to run the protocol and do QC on the final library.

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
- Standard 1: 68.80
- Standard 2: 26748.39

| QBIT date  || sample_id  ||     Species       || Temp   ||  DNA read1 || DNA read2  || DNA_AVG (ng/ul) |
|  20250122  || Mcap-F8 || *Montipora capitata*  || 25   ||  0.362    ||  0.342      ||  0.352        |
|  20250122 || Pcom-G9   || *Porites compressa* || 30    ||  0.891    ||  0.860     ||  0.8755       |
|  20250122  || Pcom-F10 || *Pocillopora acuta*  || 26.8 ||  1.46    || 1.40     ||  1.43        |
|  20250122  || Pacu-E8  || *Pocillopora acuta* || 25   ||  0.176     || 0.163      ||  0.1695       |
|  20250122   || Pacu-H6 || *Pocillopora acuta*  ||  12 ||  0.214     ||  0.195    ||  0.2045       |
|  20250122   || Pcom-H9  || *Porites compressa* ||  30  || 0.371      || 0.353     ||  0.362        |

## TapeStation
After the library prep, I run samples on the tapestation (D5000), protocol linked above.

| TapeStation date  || sample_id  ||     Species       || Temp   || TapeStation conc. ||   Primer set  |
|  20250122  || Mcap-F8   || *Montipora capitata*  || 25   || 0.577    ||   39    |
|  20250122 || Pcom-G9    || *Porites compressa* || 30   || 1.36    ||    40    |
|  20250122  || Pcom-F10  || *Pocillopora acuta*  ||  26.8 ||  2.41   ||     41   |
|  20250122  || Pacu-E8   || *Pocillopora acuta* ||  25   ||  0.183   ||      42    |
|  20250122   || Pacu-H6   || *Pocillopora acuta*  ||  12  ||  0.302  ||  43      |
|  20250122   || Pcom-H9    || *Porites compressa* ||  30   || 0.315     ||     44    |

![LibPrepRun6_complete.png](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/LibPrepRun6_complete.png?raw=true)

 - _Things to consider for next time_: at this point I tried with different amounts of input RNA and most of the samples didn't work. I will try next time to skip the step in the Zymo protocol that says "for low quality RNA" and see what output I get.