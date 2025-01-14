---
layout: post
title: Library prep using Zymo SwitchFree kit - Hawaii TPC samples - 011425
date: '2025-01-14'
category: Protocol
tags: [DNA, Zymo, RNA, library]
---

#### Using the Zymo-Seq SwitchFree 3′ mRNA Library Kit for in-house library prep of the Hawaii TPC samples - 011425

**Protocols used**
- [Zymo-Seq SwitchFree 3′ mRNA Library Kit protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/_r3008_r3009__zymo_seq_switchfree_3_mrna_library_kit.pdf)
- [TapeStation protocol DNA D5000](https://github.com/meschedl/MESPutnam_Open_Lab_Notebook/blob/master/_posts/2019-07-30-DNA-Tapestation.md)
- [High Sensitivity dsDNA QBIT protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/MAN0017455_Qubit_1X_dsDNA_HS_Assay_Kit_UG.pdf)

Using the [Zymo-Seq SwitchFree 3′ mRNA Library Kit](https://www.zymoresearch.com/products/zymo-seq-switchfree-3-mrna-library-kit) (CAT.  R3009-A, LOT. 252649) to prepare libraries starting from RNA samples exctracted from adult coral fragments from the Hawaii TPC project. RNA extraction posts can be found [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-TPCA-Summary/).

For the library prep I followed the protocol of [Jill Ashey](https://github.com/JillAshey/JillAshey_Putnam_Lab_Notebook/blob/master/_posts/2024-03-29-Zymo-SwitchFree.md) and the kit protocol above.
The kit needs a minimum of 10 ng of total RNA or a maximum of 500 ng of total RNA. I'm using 13 ng of input RNA, since it's the amount the gave me the highest concentration of library with the first samples I tried prepping. 
I'm trying thsi time with 25 ng of RNA input, 13 ng and 55.5 ng didn't work well (see previous posts).

I've used the primers in the 96 well plate (CAT. D3096, LOT. 250838) provided with the kit. For sample Mcap-H1, I've used UDI primer 4 from the 12 prep kit (CAT. D3008, LOT. 250968).
All samples were eluted in 20uL of elution buffer.

## Library prep
I ran the library prep protocol linked above. I used 21 PCR cycles.

Here's a breakdown of input RNA volume and quantity:

| sample_id || RNA_QBIT_AVG (ng/uL) || RNA (uL) || Ultrapure water (uL) || Total input RNA (ng) |
| Mcap-H1      ||              ||    0.64     ||        4.37           ||        25          |
| Mcap-G7      ||              ||   0.73     ||        4.27             ||        25          |
| Pacu-G10     ||             ||     0.90    ||         4.10            ||        25          |
| Pacu-H9      ||              ||   0.61     ||        4.39             ||        25          |
| Pacu-F7      ||              ||   0.47     ||        4.53             ||        25          |
| Mcap-F10      ||               ||   0.80     ||        4.20             ||      25          |

I'm re-doing sample Mcap-H1 from the 10th of January. I'm using UDI primer 4 from the 12prep kit (CAT. D3008, LOT. 250968) for this sample. The 96 well plate with the UDI primer is single use, no volume left for re-trying samples.

## Qubit Results
I used High Sensitivity dsDNA Qubit Protocol linked above. Library samples were read twice, standard only read once.
- Standard 1: 
- Standard 2: 

| QBIT date  || sample_id  ||     Species       || Temp   ||  DNA read1 || DNA read2  || DNA_AVG (ng/ul) |
|  20250114  || Pacu-H1   || *Pocillopora acuta*  || 18   ||  0.476          ||    0.376     ||  0.426         |
|  20250114 || Pacu-F8    || *Pocillopora acuta* || 25     ||     1.06       ||   0.91       ||  0.985         |
|  20250114    || Pcom-F8   || *Porites compressa*  ||  25   ||   3.31         ||   2.99      ||  3.15          |
|  20250114    || Mcap-G6   || *Montipora capitata* ||  12   ||  2.61         ||   2.31       ||  2.46          |
|  20250114   || Mcap-H9     || *Montipora capitata*  ||  30   ||  1.31      ||   1.18    ||  1.245         |
|  20250114   || Pcom-H6    || *Porites compressa* ||  12   ||    1.68        ||   1.57          ||  1.625         |


## TapeStation
After the library prep, I run samples on the tapestation (D5000), protocol linked above.

| TapeStation date  || sample_id  ||     Species       || Temp   || TapeStation conc. ||   Primer set  |
|  20250114  || Pacu-H1   || *Pocillopora acuta*  || 18   ||   0.746    ||     12       |
|  20250114 || Pacu-F8    || *Pocillopora acuta* || 25     ||   1.84  ||       19    |
|  20250114    || Pcom-F8   || *Porites compressa*  ||  25   || 5.02   ||     20     |
|  20250114    || Mcap-G6   || *Montipora capitata* ||  12   ||  4.55 ||      21    |
|  20250114   || Mcap-H9     || *Montipora capitata*  ||  30   ||  2.48  ||    22      |
|  20250114   || Pcom-H6    || *Porites compressa* ||  12   ||  2.88    ||     23    |


![LibPrepRun3_complete.png](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/LibPrepRun3_complete.png?raw=true)

 - _Things to consider for next time_: 
