---
layout: post
title: Library prep using Zymo SwitchFree kit - Hawaii TPC samples - 012825
date: '2025-01-28'
category: Protocol
tags: [DNA, Zymo, RNA, library]
---

#### Using the Zymo-Seq SwitchFree 3′ mRNA Library Kit for in-house library prep of the Hawaii TPC samples - 012825

**Protocols used**
- [Zymo-Seq SwitchFree 3′ mRNA Library Kit protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/_r3008_r3009__zymo_seq_switchfree_3_mrna_library_kit.pdf)
- [TapeStation protocol DNA D5000](https://github.com/meschedl/MESPutnam_Open_Lab_Notebook/blob/master/_posts/2019-07-30-DNA-Tapestation.md)
- [High Sensitivity dsDNA QBIT protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/MAN0017455_Qubit_1X_dsDNA_HS_Assay_Kit_UG.pdf)

Using the [Zymo-Seq SwitchFree 3′ mRNA Library Kit](https://www.zymoresearch.com/products/zymo-seq-switchfree-3-mrna-library-kit) (CAT.  R3009-A, LOT. 252649) to prepare libraries starting from RNA samples exctracted from adult coral fragments from the Hawaii TPC project. RNA extraction posts can be found [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-TPCA-Summary/).

For the library prep I followed the protocol of [Jill Ashey](https://github.com/JillAshey/JillAshey_Putnam_Lab_Notebook/blob/master/_posts/2024-03-29-Zymo-SwitchFree.md) and the kit protocol above.
The kit needs a minimum of 10 ng of total RNA or a maximum of 500 ng of total RNA.
I'm using 20 ng of RNA input, 13 ng, 30 ng and 55.5 ng didn't work well. 25 ng has worked for only some of the samples (see previous posts).
Skipping the step in the Zymo protocol that says "for low quality RNA" worked with the last batch of samples (see post of 23rd), so I will try again with these samples skipping it.

Here I'm using UDI primers from the 96 well plate (CAT. D3096, LOT. 250838) provided with the kit.
All samples were eluted in 18uL of elution buffer.

## Library prep
I ran the library prep protocol linked above. I used 21 PCR cycles. With 6-8 samples, it takes about 6 hours to run the protocol and do QC on the final library.
I've re-prepped the following samples, that had failed on the 22nd, skipping the "low quality RNA" step according to the Zymo kit protocol above.

Here's a breakdown of input RNA volume and quantity:

| sample_id || RNA_QBIT_AVG (ng/uL) || RNA (uL) || Ultrapure water (uL) || Total input RNA (ng) |
| Pcom-B1     ||   25     ||   0.80   ||     4.20      ||       51         |
| Mcap-H10    ||   23.7     || 0.84  ||      4.16      ||      52         |
| Pacu-E7    ||   41.4     ||   0.48  ||      4.52     ||        53         |
| Pacu-F6     ||  44.8      ||  0.45 ||      4.55      ||       54         |
| Pcom-B9    ||  33.1    ||   0.60  ||    4.40         ||        55       |
| Mcap-H8     ||  11.1     ||   1.80 ||   3.20         ||     56        |

## Qubit Results
I used High Sensitivity dsDNA Qubit Protocol linked above. Library samples were read twice, standard only read once.
- Standard 1: 68.21    
- Standard 2: 27085.45 

| QBIT date  || sample_id  ||     Species       || Temp   ||  DNA read1 || DNA read2  || DNA_AVG (ng/ul) |
|  20250128  || Pcom-B1 || *Porites compressa*  || 18   ||    6.21     || 5.87      || 6.04            |
|  20250128 || Mcap-H10   || *Montipora capitata* || 26.8 ||  3.21     ||  3.06    || 3.14            |
|  20250128  || Pacu-E7 || *Pocillopora acuta*  || 35 ||   17.8        ||  17.2    || 17.5            |
|  20250128  || Pacu-F6  || *Pocillopora acuta* || 12  ||  6.19       ||   5.94     || 6.07            |
|  20250128   || Pcom-B9 || *Porites compressa*  || 30||    15.3      ||   14.4     || 14.85           |
|  20250128   || Mcap-H8  || *Montipora capitata* ||  25 ||  5.64     ||   5.22     || 5.43            |

## TapeStation
After the library prep, I run samples on the tapestation (D5000), protocol linked above.

| TapeStation date  || sample_id  ||     Species       || Temp   || TapeStation conc. ||   Primer set  |
|  20250128  || Pcom-B1 || *Porites compressa*  || 18   ||  7.22   ||   51   |
|  20250128 || Mcap-H10   || *Montipora capitata* || 26.8    ||  3.90   ||   52    |
|  20250128  || Pacu-E7 || *Pocillopora acuta*  || 35 || 23.8     ||   53   |
|  20250128  || Pacu-F6  || *Pocillopora acuta* || 12   ||  10.1   ||    54    |
|  20250128   || Pcom-B9 || *Porites compressa*  ||  30  ||  18.8   ||  55    |
|  20250128   || Mcap-H8  || *Montipora capitata* ||  25   || 7.05    ||  56   |

![LibPrepRun9_complete.png](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/LibPrepRun9_complete.png?raw=true)

 - _Things to consider for next time_: Givem the presence of weird double peaks in some of the samples (also the size looks strange), I don't think that running the library prep protocol skipping the low quality RNA step is the solution.