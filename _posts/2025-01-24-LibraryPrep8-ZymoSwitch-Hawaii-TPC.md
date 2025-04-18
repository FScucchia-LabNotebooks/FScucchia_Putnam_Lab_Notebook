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

Here I'm using primers 39-44 that we already had in the lab, and that were diluted and mixed (5i+i7). The  primers in the 96 well plate (CAT. D3096, LOT. 250838) provided with the kit are single use, so could not reuse them again. 
All samples were eluted in 18uL of elution buffer.

## Library prep
I ran the library prep protocol linked above. I used 21 PCR cycles. With 6-8 samples, it takes about 6 hours to run the protocol and do QC on the final library.
I've re-prepped the following samples, that had failed on the 22nd, skipping the "low quality RNA" step according to the Zymo kit protocol above.

Here's a breakdown of input RNA volume and quantity:

| sample_id || RNA_QBIT_AVG (ng/uL) || RNA (uL) || Ultrapure water (uL) || Total input RNA (ng) |
| Mcap-F8     ||   29.1     ||   0.69   ||     4.31      ||        20         |
| Pcom-G9     ||   62.9     ||   0.32  ||      4.68           ||        20         |
| Pcom-F10    ||   44.0     ||   0.45  ||      4.55           ||        20         |
| Pacu-E8     ||  25.8      ||  0.78  ||      4.22           ||        20         |
| Pacu-H6     ||  36.5     ||   0.55  ||    4.45            ||        20         |
| Pcom-H9     ||  47.1     ||   0.42    ||    4.58             ||      20         |

## Qubit Results
I used High Sensitivity dsDNA Qubit Protocol linked above. Library samples were read twice, standard only read once.
- Standard 1: 66.42   
- Standard 2: 27992.47 

| QBIT date  || sample_id  ||     Species       || Temp   ||  DNA read1 || DNA read2  || DNA_AVG (ng/ul) |
|  20250124  || Mcap-F8 || *Montipora capitata*  || 25   ||   0.057    ||  0.051     || 0.054            |
|  20250124 || Pcom-G9   || *Porites compressa* || 30    ||   LOW     ||  LOW        ||                 |
|  20250124  || Pcom-F10 || *Pocillopora acuta*  || 26.8 ||   LOW     ||  LOW        ||                 |
|  20250124  || Pacu-E8  || *Pocillopora acuta* || 25   ||   LOW      || LOW         ||                 |
|  20250124   || Pacu-H6 || *Pocillopora acuta*  ||  12 ||   0.072    || 0.07        ||   0.071         |
|  20250124   || Pcom-H9  || *Porites compressa* ||  30  ||  LOW      ||  LOW        ||                 |

*LOW: out of range

## TapeStation
After the library prep, I run samples on the tapestation (D5000), protocol linked above.

| TapeStation date  || sample_id  ||     Species       || Temp   || TapeStation conc. ||   Primer set  |
|  20250124  || Mcap-F8 || *Montipora capitata*  || 25   ||  0   ||   39    |
|  20250124 || Pcom-G9   || *Porites compressa* || 30    ||  0    ||   40    |
|  20250124  || Pcom-F10 || *Montipora capitata*  || 26.8 || 0      ||   41   |
|  20250124  || Pacu-E8  || *Porites compressa* ||  12   ||  0    ||    42    |
|  20250124   || Pacu-H6 || *Pocillopora acuta*  ||  35  ||  0    ||  43     |
|  20250124   || Pcom-H9  || *Porites compressa* ||  18   || 0.054    ||  44   |

![LibPrepRun8_complete.png](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/LibPrepRun8_complete.png?raw=true)

 - _Things to consider for next time_: I got nothing for all samples on the Tapestation, which is strange. I think it might have been because of the primers that I used (not part of the kit, already in the lab)