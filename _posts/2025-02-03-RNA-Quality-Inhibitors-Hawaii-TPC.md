---
layout: post
title: RNA quality check after PCR inhibitors removal - Hawai TPC
date: '2025-02-05'
category: PCR inhibitors
tags: [RNA, Zymo]
---

#### RNA quality check before and after removal of potential PCR inhibitors - _Pocillopora acuta_, _Montipora capitata_, _Porites compressa_, Hawaii TPC project

**Protocols used**
- [Zymo OneStep PCR Inhibitor Removal Kit protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/d6031_onestep_pcr_inhibitor_removal_kit.pdf)
- [TapeStation protocol RNA](https://github.com/meschedl/MESPutnam_Open_Lab_Notebook/blob/master/_posts/2019-03-07-RNA-TapeStation-Protocol.md)
- [QBIT protocol](https://github.com/meschedl/MESPutnam_Open_Lab_Notebook/blob/master/_posts/2019-03-08-Qubit-Protocol.md)

Here I'm checking the quality of 6 RNA samples (n=2 per species, _Pocillopora acuta_, _Montipora capitata_, _Porites compressa_) by TapeStation, Nanodrop and QBIT before and after using the [Zymo OneStep PCR Inhibitor Removal Kit](https://www.zymoresearch.com/collections/onestep-pcr-inhibitor-removal-kits/products/onestep-pcr-inhibitor-removal-new-kit). Library prep hasn't been very successful, see [summary](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-TPCA-Summary/) so we want to test for the presence of potential PCR inhibitors.
I'm using the same input for all samples, 924 ng in 55 ul (the kit wants a minimum of 50 ul).

**Qubit**

| sample_id  ||     Species       || Temp   ||  RNA_AVG (ng/ul) before || RNA_AVG (ng/ul) after |
| Pcom-E10   || *Porites compressa*  || 26.8   || 27.2    ||   13.0       |
| Pcom-F8   || *Porites compressa* || 25     ||   14.4  ||    17.8       |
| Pacu-H1   || *Pocillopora acuta*  ||  18   || 20.5  ||      11.5       |
| Pacu-D8   || *Pocillopora acuta* ||  25   ||  19.3  ||     13.3       |
| Mcap-H1   || *Montipora capitata*  ||  18  ||  41.5 ||     12.7      |
| Mcap-D10  || *Montipora capitata* ||  26.8  ||  17.6  ||    12.5     |

*before* PCR inhibitors removal
*after* PCR inhibitors removal

**Nanodrop**
- Expected 260/230 values are commonly in the range of 2.0-2.2. If the ratios are lower or abnormally higher it indicates the contamination of the samples with certain protein or phenolic compounds 
- A 260/280 ratio of around 2.0 is generally considered pure for RNA. Abnormal 260/280 ratios usually indicate that a sample is contaminated by residual phenol, guanidine, or other reagent used in the extraction protocol

| sample_id  ||  Species  || Temp  ||  RNA_AVG (ng/ul) before || RNA_AVG (ng/ul) after || 260/230 before || 260/230 after || 260/280 before || 260/280 after |
| Pcom-E10   || *Porites compressa*  || 26.8   || 24.35    ||    19.2      ||     1.08        ||  0.88 || 3.03    ||   2.24     |
| Pcom-F8   || *Porites compressa* || 25     || 26.1    ||    25.25       ||         3.88      || 1.03 || 2.99    ||   2.33     |
| Pacu-H1   || *Pocillopora acuta*  ||  18   ||  20.1  ||    12.95        ||  0.76     || 0.59 || 3.30    ||   2.72     |
| Pacu-D8   || *Pocillopora acuta* ||  25   || 12.1   ||    31.3        ||    0.99    || 0.68 || 3.96   ||   2.70     |
| Mcap-H1   || *Montipora capitata*  ||  18  || 28.96  ||  15.45         ||    3.65   || 0.95 || 3.11   ||   2.58     |
| Mcap-D10  || *Montipora capitata* ||  26.8  || 12.6   ||  20.65       ||    1.67   || 0.73 || 5.45   ||   2.89     |

![Nanodrop_RNA_PCRinhibitors.png](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/Nanodrop_RNA_PCRinhibitors.png?raw=true)

**TapeStation**

| sample_id  ||  Species  || Temp  ||  RNA_conc (ng/ul) before || RNA_conc (ng/ul) after || RIN before || RIN after |
| Pcom-E10   || *Porites compressa*  || 26.8   || 28.5    ||  13.0        ||    9         ||    8.4       |
| Pcom-F8   || *Porites compressa* || 25     ||  21.5   ||   20.8        ||     8.4       ||    8.7    |
| Pacu-H1   || *Pocillopora acuta*  ||  18   ||  23.2  ||    11.3         ||    8.8        ||   8.1            |
| Pacu-D8   || *Pocillopora acuta* ||  25   ||  28.0  ||     14.6       ||     9        ||      8.4          |
| Mcap-H1   || *Montipora capitata*  ||  18  || 40.4   ||    13.0       ||     9.5        ||      8.5           |
| Mcap-D10  || *Montipora capitata* ||  26.8  ||  16.8  ||   13.0      ||      8.1        ||      7.9            |
