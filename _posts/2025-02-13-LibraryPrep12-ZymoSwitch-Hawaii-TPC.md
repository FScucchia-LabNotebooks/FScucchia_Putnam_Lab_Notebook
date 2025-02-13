---
layout: post
title: Library prep using Zymo SwitchFree kit - Hawaii TPC samples - 021325
date: '2025-02-13'
category: Protocol
tags: [DNA, Zymo, RNA, library]
---

#### Using the Zymo-Seq SwitchFree 3′ mRNA Library Kit for in-house library prep of the Hawaii TPC samples - 021325

**Protocols used**
- [Zymo-Seq SwitchFree 3′ mRNA Library Kit protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/_r3008_r3009__zymo_seq_switchfree_3_mrna_library_kit.pdf)
- [TapeStation protocol DNA D5000](https://github.com/meschedl/MESPutnam_Open_Lab_Notebook/blob/master/_posts/2019-07-30-DNA-Tapestation.md)
- [High Sensitivity dsDNA QBIT protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/MAN0017455_Qubit_1X_dsDNA_HS_Assay_Kit_UG.pdf)

Using the [Zymo-Seq SwitchFree 3′ mRNA Library Kit](https://www.zymoresearch.com/products/zymo-seq-switchfree-3-mrna-library-kit) (CAT.  R3009-A, LOT. 252649) to prepare libraries starting from RNA samples exctracted from adult coral fragments from the Hawaii TPC project. RNA extraction posts can be found [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-TPCA-Summary/).

For the library prep I followed the protocol of [Jill Ashey](https://github.com/JillAshey/JillAshey_Putnam_Lab_Notebook/blob/master/_posts/2024-03-29-Zymo-SwitchFree.md) and the kit protocol above.
The kit needs a minimum of 10 ng of total RNA or a maximum of 500 ng of total RNA.
I'm try again using 25 ng of RNA input, 13 ng, 30 ng and 55.5 ng didn't work well. 20 ng has worked for only some of the samples (see previous posts).

Here I'm using UDI primers from the 96 well plate (CAT. D3096, LOT. 250838) provided with the kit.
All samples were eluted in 18uL of elution buffer.

## Library prep
I ran the library prep protocol linked above. I'm trying with 22 PCR cycles (so far I used the max recommended by the kit, which is 21). With 6-8 samples, it takes about 6 hours to run the protocol and do QC on the final library.

Here's a breakdown of input RNA volume and quantity:

| sample_id || RNA_QBIT_AVG (ng/uL) || RNA (uL) || Ultrapure water (uL) || Total input RNA (ng) |
|  Mcap-G11  || 14     || 1.79   || 3.21   ||       25        |
|  Pcom-F9   || 46.8   || 0.53   || 4.47   ||      25       |
|  Pacu-B10  || 153.5  || 0.16   || 4.84   ||       25        |
|  Pacu-G6   || 43.8   || 0.57   || 4.43   ||       25        |
|  Mcap-H7   || 42.9   || 0.58   || 4.42   ||       25     |
|  Mcap-E1   || 48.7   || 0.51   || 4.49   ||    25       |
|  Pacu-G9   || 13.9   || 1.80   || 3.20   ||      25     |
|  Pcom-E6   || 24.3   || 1.03   || 3.97   ||    25       |

## Qubit Results
I used High Sensitivity dsDNA Qubit Protocol linked above. Library samples were read twice, standard only read once.
- Standard 1: 66.40    
- Standard 2: 28121.89

| QBIT date  || sample_id  ||     Species       || Temp ||  DNA read1 || DNA read2  || DNA_AVG (ng/ul) |
|  20250213  || Mcap-G11 || *Montipora capitata*  || 26.8 || 0.826  ||   0.786   || 0.806           |
|  20250213 || Pcom-F9   || *Porites compressa* || 30 ||  0.289   ||    0.278      || 0.284         |
|  20250213  || Pacu-B10 || *Pocillopora acuta*  || 26.8 || 1.52    || 1.43   || 1.475           |
|  20250213  || Pacu-G6  || *Pocillopora acuta* || 12 ||  0.784    || 0.699    || 0.742         |
|  20250213   || Mcap-H7 || *Montipora capitata*  || 35 ||  2.68  ||   2.58    || 2.63           |
|  20250213   || Mcap-E1  || *Montipora capitata* || 18 ||  5.10  || 4.84     || 4.97           |
|  20250213   || Pacu-G9 || *Pocillopora acuta*  || 30 ||  2.3    ||  2.25    || 2.275          |
|  20250213   || Pcom-E6  || *Porites compressa* || 12 ||   0.403 ||  0.380    || 0.392        |

## TapeStation
After the library prep, I run samples on the tapestation (D5000), protocol linked above.

| TapeStation date  || sample_id  ||     Species       || Temp   || TapeStation conc. ||   Primer set  |
|  20250213  || Mcap-G11 || *Montipora capitata*  || 26.8   ||       ||  67     |
|  20250213 || Pcom-F9   || *Porites compressa* || 30    ||       ||  68     |
|  20250213  || Pacu-B10 || *Pocillopora acuta*  || 26.8 ||       ||  69     |
|  20250213  || Pacu-G6  || *Pocillopora acuta* || 12 ||       ||  70     |
|  20250213   || Mcap-H7 || *Montipora capitata*  || 35 ||       ||  71     |
|  20250213   || Mcap-E1  || *Montipora capitata* || 18  ||       ||   72    |
|  20250213   || Pacu-G9 || *Pocillopora acuta*  || 30  ||       ||  73     |
|  20250213   || Pcom-E6  || *Porites compressa* || 12  ||       ||   74    |

![LibPrepRun12_complete.png](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/LibPrepRun12_complete.png?raw=true)

 - _Things to consider for next time_: increasing the number of PCR cycles to 22 doesn't improve things. Need to re-think about a strategy with these samples.
