---
layout: post
title: Library prep using Zymo SwitchFree kit - Hawaii TPC samples - 121724
date: '2024-12-17'
category: Protocol
tags: [DNA, Zymo, RNA, library]
---

#### Using the Zymo-Seq SwitchFree 3′ mRNA Library Kit for in-house library prep of the Hawaii TPC samples - 121724

**Protocols used**
- [Zymo-Seq SwitchFree 3′ mRNA Library Kit protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/_r3008_r3009__zymo_seq_switchfree_3_mrna_library_kit.pdf)
- [TapeStation protocol DNA D5000](https://github.com/meschedl/MESPutnam_Open_Lab_Notebook/blob/master/_posts/2019-07-30-DNA-Tapestation.md)

Using the [Zymo-Seq SwitchFree 3′ mRNA Library Kit](https://www.zymoresearch.com/products/zymo-seq-switchfree-3-mrna-library-kit) to prepare libraries starting from RNA samples exctracted from adult coral fragments from the Hawaii TPC project. RNA extraction posts can be found [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-TPCA-Summary/).

For the library prep I followed the protocol of [Jill Ashey](https://github.com/JillAshey/JillAshey_Putnam_Lab_Notebook/blob/master/_posts/2024-03-29-Zymo-SwitchFree.md) and the kit protocol above.
The kit needs a minimum of 10 ng of total RNA or a maximum of 500 ng of total RNA. I'm using the max volume of RNA input (5 ul) for the sample with the lowest RNA concentration among all, which is 11.1 ng/uL, which corresponds to a total of _55.5 ng_. I will use this 55.5 as inpout for all other samples. 

## Library prep
I ran the library prep protocol linked above. I used 19 PCR cycles.

Here's a breakdown of input RNA volume and quantity:

| sample_id || RNA_QBIT_AVG (ng/uL) || RNA (uL) || Ultrapure water (uL) || Total input RNA (ng) |
| Pacu-D8       ||   19.3           ||    2.88     ||        2.12             ||        55.5         |
| Pacu-H10      ||   20.5           ||    2.71     ||        2.29             ||        55.5          |
| Mcap-H1      ||    41.5           ||    1.34     ||        3.66             ||        55.5          |
| Pcomp-G8      ||   36.1           ||    1.54     ||        3.46             ||        55.5          |
| Mcap-E8      ||    25.4           ||    2.19     ||        2.81             ||        55.5          |
| Pacu-B8      ||    23.5           ||    2.36     ||        2.64             ||        55.5          |
| Mcap-B7      ||    24.2           ||    2.29     ||        2.71             ||        55.5          |
| Pcomp-G1      ||   30.9           ||    1.80     ||        3.20             ||        55.5          |

**TapeStation**

After the library prep, I run samples on the tapestation (D5000), protocol linked above.

| Library prep date  || sample_id  ||     Species       || Temp   ||    TapeStation conc.     ||   Primer set  |
|   ||      ||           ||       ||              ||   |
|   ||     ||        ||     ||            ||   |

![LibraryPrepZymo.png](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/LibraryPrepZymo.png?raw=true)

