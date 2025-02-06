---
layout: post
title: Library prep using Zymo SwitchFree kit, PCR inhibitors removed - Hawaii TPC samples - 020525
date: '2025-02-05'
category: Protocol
tags: [DNA, Zymo, RNA, library]
---

#### Using the Zymo-Seq SwitchFree 3′ mRNA Library Kit for in-house library prep of the Hawaii TPC samples after removal of PCR inhibitors - 020525

**Protocols used**
- [Zymo-Seq SwitchFree 3′ mRNA Library Kit protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/_r3008_r3009__zymo_seq_switchfree_3_mrna_library_kit.pdf)
- [TapeStation protocol DNA D5000](https://github.com/meschedl/MESPutnam_Open_Lab_Notebook/blob/master/_posts/2019-07-30-DNA-Tapestation.md)
- [High Sensitivity dsDNA QBIT protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/MAN0017455_Qubit_1X_dsDNA_HS_Assay_Kit_UG.pdf)

Using the [Zymo-Seq SwitchFree 3′ mRNA Library Kit](https://www.zymoresearch.com/products/zymo-seq-switchfree-3-mrna-library-kit) (CAT.  R3009-A, LOT. 252649) to prepare libraries starting from RNA samples exctracted from adult coral fragments from the Hawaii TPC project. RNA extraction posts can be found [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-TPCA-Summary/).
The RNA samples I'm using were treated with the [Zymo OneStep PCR Inhibitor Removal Kit](https://www.zymoresearch.com/collections/onestep-pcr-inhibitor-removal-kits/products/onestep-pcr-inhibitor-removal-new-kit) for removal of potential PCR inhibitors that have caused the library to fail for most of the samples so far. See the post [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/RNA-Quality-Inhibitors-Hawaii-TPC/) about PCR inhibitors removal.

For the library prep I followed the protocol of [Jill Ashey](https://github.com/JillAshey/JillAshey_Putnam_Lab_Notebook/blob/master/_posts/2024-03-29-Zymo-SwitchFree.md) and the kit protocol above.
The kit needs a minimum of 10 ng of total RNA or a maximum of 500 ng of total RNA.
I'm using 20 ng of RNA input, 13 ng, 30 ng and 55.5 ng didn't work well. 25 ng has worked for only some of the samples (see previous posts).

Here I'm using UDI primers from the 96 well plate (CAT. D3096, LOT. 250838) provided with the kit.
All samples were eluted in 18uL of elution buffer.

## Library prep
I ran the library prep protocol linked above. I used 21 PCR cycles. With 6-8 samples, it takes about 6 hours to run the protocol and do QC on the final library.

Here's a breakdown of input RNA volume and quantity:

| sample_id || RNA_QBIT_AVG (ng/uL) || RNA (uL) || Ultrapure water (uL) || Total input RNA (ng) |
| Pcom-G10     ||   13.0     ||   1.54 ||     3.46    ||       20        |
| Pcom-F8    ||   17.8     || 1.12  ||     3.88      ||      20       |
| Pacu-H1    ||   11.5     ||   1.74  ||   3.26     ||        20        |
| Pacu-D8     ||  13.3       ||  1.57 ||   3.43     ||       20        |
| Mcap-G1    ||   12.7    ||   1.60  ||    3.40         ||       20     |
| Mcap-F10     ||   12.5    ||   1.50 ||   3.50         ||    20       |

## Qubit Results
I used High Sensitivity dsDNA Qubit Protocol linked above. Library samples were read twice, standard only read once.
- Standard 1: 75.28   
- Standard 2: 28194.13

| QBIT date  || sample_id  ||     Species       || Temp   ||  DNA read1 || DNA read2  || DNA_AVG (ng/ul) |
|  20250205  || Pcom-G10 || *Porites compressa*  || 26.8  ||   0.222     || 0.210      || 0.216          |
|  20250205 || Pcom-F8   || *Porites compressa* || 25 ||  too low    ||  too low    ||    too low        |
|  20250205  || Pacu-H1 || *Pocillopora acuta*  || 18 ||   0.699      ||   0.701  || 0.700          |
|  20250205  || Pacu-D8  || *Pocillopora acuta* || 25  ||  too low   ||   too low   ||    too low        |
|  20250205   || Mcap-G1 || *Montipora capitata*  || 18 ||  0.432      || 0.430      || 0.431          |
|  20250205   || Mcap-F10  || *Montipora capitata* || 26.8 ||  0.439    ||   0.426     || 0.4325         |

## TapeStation
After the library prep, I run samples on the tapestation (D5000), protocol linked above.

| TapeStation date  || sample_id  ||     Species       || Temp   || TapeStation conc. ||   Primer set  |
|  20250205  || Pcom-G10 || *Porites compressa*  || 26.8   || 0.208   ||  20   |
|  20250205 || Pcom-F8   || *Porites compressa* || 25    ||      ||   32    |
|  20250205  || Pacu-H1 || *Pocillopora acuta*  || 18 ||   1.41     ||   12   |
|  20250205  || Pacu-D8  || *Pocillopora acuta* || 25   ||      ||    13    |
|  20250205   || Mcap-G1 || *Montipora capitata*  || 18  ||  0.508   ||  30  |
|  20250205   || Mcap-F10  || *Montipora capitata* || 26.8  || 0.389   ||  57   |

![LibPrepRun10_complete.png](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/LibPrepRun10_complete.png?raw=true)
