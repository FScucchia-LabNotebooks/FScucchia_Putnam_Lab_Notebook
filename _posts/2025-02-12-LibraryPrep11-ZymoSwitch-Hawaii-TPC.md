---
layout: post
title: Library prep using Zymo SwitchFree kit - Hawaii TPC samples - 021225
date: '2025-02-12'
category: Protocol
tags: [DNA, Zymo, RNA, library]
---

#### Using the Zymo-Seq SwitchFree 3′ mRNA Library Kit for in-house library prep of the Hawaii TPC samples - 020525

**Protocols used**
- [Zymo OneStep PCR Inhibitor Removal Kit protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/d6031_onestep_pcr_inhibitor_removal_kit.pdf)
- [Zymo-Seq SwitchFree 3′ mRNA Library Kit protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/_r3008_r3009__zymo_seq_switchfree_3_mrna_library_kit.pdf)
- [TapeStation protocol DNA D5000](https://github.com/meschedl/MESPutnam_Open_Lab_Notebook/blob/master/_posts/2019-07-30-DNA-Tapestation.md)
- [High Sensitivity dsDNA QBIT protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/MAN0017455_Qubit_1X_dsDNA_HS_Assay_Kit_UG.pdf)

Using the [Zymo-Seq SwitchFree 3′ mRNA Library Kit](https://www.zymoresearch.com/products/zymo-seq-switchfree-3-mrna-library-kit) (CAT.  R3009-A, LOT. 252649) to prepare libraries starting from RNA samples exctracted from adult coral fragments from the Hawaii TPC project. RNA extraction posts can be found [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-TPCA-Summary/).
The RNA samples I'm using were treated with the [Zymo OneStep PCR Inhibitor Removal Kit](https://www.zymoresearch.com/collections/onestep-pcr-inhibitor-removal-kits/products/onestep-pcr-inhibitor-removal-new-kit) for removal of potential PCR inhibitors that have caused the library to fail for most of the samples so far. 

For the library prep I followed the protocol of [Jill Ashey](https://github.com/JillAshey/JillAshey_Putnam_Lab_Notebook/blob/master/_posts/2024-03-29-Zymo-SwitchFree.md) and the kit protocol above.
The kit needs a minimum of 10 ng of total RNA or a maximum of 500 ng of total RNA.
I'm using 20 ng of RNA input, 13 ng, 30 ng and 55.5 ng didn't work well. 25 ng has worked for only some of the samples (see previous posts).

Here I'm using UDI primers from the 96 well plate (CAT. D3096, LOT. 250838) provided with the kit.
All samples were eluted in 18uL of elution buffer.

## Library prep
I ran the library prep protocol linked above. I used 21 PCR cycles. With 6-8 samples, it takes about 6 hours to run the protocol and do QC on the final library.

Here's a breakdown of input RNA volume and quantity:

| sample_id || RNA_QBIT_AVG (ng/uL) || RNA (uL) || Ultrapure water (uL) || Total input RNA (ng) |
|  Pcom-G6    || 35.8   || 0.56   || 4.44 ||       20        |
|  Pcom-E9    || 45.9   || 0.44   || 4.56     ||      20       |
|  Pacu-F9    || 34.1   || 0.59   || 4.41  ||        20        |
|  Mcap-F1    || 17.3   || 1.16   || 3.84  ||       20        |
|  Pcom-F7    || 43.4   || 0.46   || 4.54   ||       20     |
|  Mcap-E7    || 57.2   || 0.35   || 4.65     ||    20       |
|  Mcap-F9    || 16.9   || 1.18   || 3.82      ||       20     |
|  Pacu-F11   || 19     || 1.05   || 3.95       ||    20       |

## Qubit Results
I used High Sensitivity dsDNA Qubit Protocol linked above. Library samples were read twice, standard only read once.
- Standard 1: 67.78     
- Standard 2: 26433.03 

| QBIT date  || sample_id  ||     Species       || Temp ||  DNA read1 || DNA read2  || DNA_AVG (ng/ul) |
|  20250212  || Pcom-G6 || *Porites compressa*  || 12 ||    0.098   ||   0.09        || 0.094           |
|  20250212 || Pcom-E9   || *Porites compressa* || 30 ||    2.90   ||    2.74         || 2.82            |
|  20250212  || Pacu-F9 || *Pocillopora acuta*  || 30 ||    0.281  ||    0.27         || 0.276           |
|  20250212  || Mcap-F1  || *Montipora capitata* || 18 ||   0.394  ||  0.362          || 0.378           |
|  20250212   || Pcom-F7 || *Porites compressa*  || 35 ||   0.134  ||  0.120          || 0.127           |
|  20250212   || Mcap-E7  || *Montipora capitata* || 35 ||  0.654  || 0.621           || 0.6375          |
|  20250212   || Mcap-F9 || *Montipora capitata*  || 30 ||  1.56   ||   1.49          || 1.525           |
|  20250212   || Pacu-F11  || *Pocillopora acuta* || 26.8 ||  0.271||  0.25           || 0.2605          |

## TapeStation
After the library prep, I run samples on the tapestation (D5000), protocol linked above.

| TapeStation date  || sample_id  ||     Species       || Temp   || TapeStation conc. ||   Primer set  |
|  20250212  || Pcom-G6 || *Porites compressa*  || 12   ||   0    ||  59     |
|  20250212 || Pcom-E9   || *Porites compressa* || 30    || 4.09      ||  60     |
|  20250212  || Pacu-F9 || *Pocillopora acuta*  || 30 ||  0.531     ||  61     |
|  20250212  || Mcap-F1  || *Montipora capitata* || 18 ||  0.686     ||   62    |
|  20250212   || Pcom-F7 || *Porites compressa*  || 35 ||  0.0547     ||     63  |
|  20250212   || Mcap-E7  || *Montipora capitata* || 35  ||  1.02     ||   64    |
|  20250212   || Mcap-F9 || *Montipora capitata*  || 30  || 1.31      ||   65    |
|  20250212   || Pacu-F11  || *Pocillopora acuta* || 26.8  ||  0.343     ||  66     |

![LibPrepRun11_complete.png](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/LibPrepRun11_complete.png?raw=true)
