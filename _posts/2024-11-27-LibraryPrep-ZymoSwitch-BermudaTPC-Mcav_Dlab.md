---
layout: post
title: Try again with library prep using Zymo SwitchFree kit - Bermuda TPC samples - 112724
date: '2024-11-27'
category: Protocol
tags: [DNA, Zymo, RNA, library]
---

#### Trying again with library prep using the Zymo-Seq SwitchFree 3′ mRNA Library Kit for Bermuda TPC samples - Mcav and Dlab 

**Protocols used**
- [Zymo-Seq SwitchFree 3′ mRNA Library Kit protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/_r3008_r3009__zymo_seq_switchfree_3_mrna_library_kit.pdf)
- [QBIT protocol](https://github.com/meschedl/MESPutnam_Open_Lab_Notebook/blob/master/_posts/2019-03-08-Qubit-Protocol.md)
- [TapeStation protocol RNA](https://github.com/meschedl/MESPutnam_Open_Lab_Notebook/blob/master/_posts/2019-03-07-RNA-TapeStation-Protocol.md)
- [TapeStation protocol DNA D5000](https://github.com/meschedl/MESPutnam_Open_Lab_Notebook/blob/master/_posts/2019-07-30-DNA-Tapestation.md)


Using the [Zymo-Seq SwitchFree 3′ mRNA Library Kit](https://www.zymoresearch.com/products/zymo-seq-switchfree-3-mrna-library-kit) to try again preparing libraries starting from RNA samples exctracted from adult coral fragments from the Hawaii and Bermuda TPC project. The library prep for Mcav and Dlab RNA samples has not worked so far, so I'm trying again maxing out the input RNA (5 uL of extracted RNA sample, max staerting volume for this kit). So far I've tried 13ng and 15ng RNA input.

For the library prep I followed the protocol of [Jill Ashey](https://github.com/JillAshey/JillAshey_Putnam_Lab_Notebook/blob/master/_posts/2024-03-29-Zymo-SwitchFree.md) and the kit protocol linked above. These are the last 2 preps with this kit (12 prep kit).
The kit needs a minimum of 10 ng of total RNA or a maximum of 500 ng of total RNA. I'm using the max volume of RNA input (5 ul) and a lower number of cycles as my previous attempts, 19 instead of 21 PCR amplification cycles (see the kit protocol for which number of cycles to choose based on input RNA).

**QBIT before library prep**

|sample_id   || RNA_QBIT_read1 (ng/uL)|| RNA_QBIT_read2 (ng/uL)|| RNA_QBIT_AVG (ng/uL) |
| Mcav-       ||      ||           ||                   ||                 |
| Dlab-       ||      ||           ||                    ||                 |

**TapeStation before library prep**

I run the samples on the TS using the RNA protocol linked above. 

![LibraryPrepZymo4.png](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/LibraryPrepZymo4.png?raw=true)


## Library prep
I run the library prep protocol linked above, with the Mcav- and Dlab- sample extracted by Zoe.

Here's a breakdown of input RNA volume:

| sample_id || RNA_QBIT_AVG (ng/uL) || RNA (uL) || Ultrapure water (uL) || Total starting volume (ul) |
| Mcav-       ||      ||    5       ||        0           ||        5         |
| Dlab-       ||      ||    5       ||        0            ||       5          |



**TapeStation**

After the library prep, I run samples on the tapestation (D5000), protocol linked above.

| Library prep date  || sample_id  ||     Species            || Temp   ||    TapeStation conc.     ||   Primer set  |
| 20241127  ||  Mcav-    || *Montastraea cavernosa*          || 29       ||    Below 1          ||  11  |
| 20241127  ||  Mcav-   || *Diploria labyrinthiformis*       || 29     ||   Below 1         ||  12  |

