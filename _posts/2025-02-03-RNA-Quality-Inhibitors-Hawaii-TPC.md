---
layout: post
title: RNA quality check after PCR inhibitors removal - Hawai TPC
date: '2025-02-03'
category: PCR inhibitors
tags: [RNA, Zymo]
---

#### RNA quality check before and after removal of potential PCR inhibitors - _Pocillopora acuta_, _Montipora capitata_, _Porites compressa_, Hawaii TPC project

**Protocols used**
- [Zymo OneStep PCR Inhibitor Removal Kit protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/d6031_onestep_pcr_inhibitor_removal_kit.pdf)
- [TapeStation protocol RNA](https://github.com/meschedl/MESPutnam_Open_Lab_Notebook/blob/master/_posts/2019-03-07-RNA-TapeStation-Protocol.md)
- [QBIT protocol](https://github.com/meschedl/MESPutnam_Open_Lab_Notebook/blob/master/_posts/2019-03-08-Qubit-Protocol.md)

Here I'm checking the quality of 6 RNA samples (n=2 per species, _Pocillopora acuta_, _Montipora capitata_, _Porites compressa_) by TapeStation, Nanodrop and QBIT before and after using the [Zymo OneStep PCR Inhibitor Removal Kit](https://www.zymoresearch.com/collections/onestep-pcr-inhibitor-removal-kits/products/onestep-pcr-inhibitor-removal-new-kit). Library prep hasn't been very successful, see [summary](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-TPCA-Summary/) so we want to test for the presence of potential PCR inhibitors.

**Qubit**

| sample_id  ||     Species       || Temp   ||  RNA_AVG (ng/ul) before || RNA_AVG (ng/ul) after |
| Pcom-E10   || *Porites compressa*  || 26.8   || 27.2    ||          |
| Pcom-F8   || *Porites compressa* || 25     ||   14.4  ||           |
| Pacu-H1   || *Pocillopora acuta*  ||  18   || 20.5  ||             |
| Pacu-D8   || *Pocillopora acuta* ||  25   ||  19.3  ||            |
| Mcap-H1   || *Montipora capitata*  ||  18  ||  41.5 ||           |
| Mcap-D10  || *Montipora capitata* ||  26.8  ||  17.6  ||         |

*before* PCR inhibitors removal
*after* PCR inhibitors removal

**Nanodrop**

| sample_id  ||  Species  || Temp  ||  RNA_AVG (ng/ul) before || RNA_AVG (ng/ul) after || 260/230 || 260/280 |
| Pcom-E10   || *Porites compressa*  || 26.8   ||     ||          ||             |
| Pcom-F8   || *Porites compressa* || 25     ||     ||           ||              |
| Pacu-H1   || *Pocillopora acuta*  ||  18   ||    ||             ||            |
| Pacu-D8   || *Pocillopora acuta* ||  25   ||    ||            ||             |
| Mcap-H1   || *Montipora capitata*  ||  18  ||    ||           ||             |
| Mcap-D10  || *Montipora capitata* ||  26.8  ||    ||         ||              |

**TapeStation**

| sample_id  ||  Species  || Temp  ||  RNA_conc (ng/ul) before || RNA_conc (ng/ul) after || RIN before || RIN after |
| Pcom-E10   || *Porites compressa*  || 26.8   || 28.5    ||          ||    9         ||           |
| Pcom-F8   || *Porites compressa* || 25     ||  21.5   ||           ||     8.4       ||        |
| Pacu-H1   || *Pocillopora acuta*  ||  18   ||  23.2  ||             ||    8.8        ||               |
| Pacu-D8   || *Pocillopora acuta* ||  25   ||  28.0  ||            ||     9        ||                |
| Mcap-H1   || *Montipora capitata*  ||  18  || 40.4   ||           ||     9.5        ||                 |
| Mcap-D10  || *Montipora capitata* ||  26.8  ||  16.8  ||         ||      8.1        ||                  |
