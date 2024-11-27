---
layout: post
title: Library prep using Zymo SwitchFree kit - Hawaii and Bermuda TPC samples
date: '2024-11-21'
category: Protocol
tags: [DNA, Zymo]
---

#### Using the Zymo-Seq SwitchFree 3′ mRNA Library Kit for in-house library prep of the Hawaii and Bermuda TPC samples - 112124

**Protocols used**
- [Zymo-Seq SwitchFree 3′ mRNA Library Kit protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/_r3008_r3009__zymo_seq_switchfree_3_mrna_library_kit.pdf)
- [TapeStation protocol](https://github.com/meschedl/MESPutnam_Open_Lab_Notebook/blob/master/_posts/2019-07-30-DNA-Tapestation.md)


Using the [Zymo-Seq SwitchFree 3′ mRNA Library Kit](https://www.zymoresearch.com/products/zymo-seq-switchfree-3-mrna-library-kit) to try preparing libraries starting from RNA samples exctracted from adult coral fragments from the Hawaii and Bermuda TPC project. RNA extraction post about these extractions can be found [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-TPCA/).

For the library prep I followed the protocol of [Jill Ashey](https://github.com/JillAshey/JillAshey_Putnam_Lab_Notebook/blob/master/_posts/2024-03-29-Zymo-SwitchFree.md) and the kit protocol above.
The kit needs a minimum of 10 ng of total RNA or a maximum of 500 ng of total RNA, which is a large range. Since some of the concentrations in these samples were low, I used 13ng of total RNA as input for all species. 
Given the low input for these preps and previous experience of lab members with Zymo kits, I'm using 21 PCR amplification cycles (maximum recommended by the zymo kit for <100ng input RNA).

Here's a breakdown of input RNA volumes for each sample:

| colony_id | RNA_QBIT_AVG (ng/uL) | RNA (uL) | Ultrapure water (uL) | Total starting volume (ul) |
| Pacu-H10 | 13.8           | 0.67      | 4.33                  | 5.0                        |	
| Pcomp-E10 | 27.2          | 0.48      | 4.52                 | 5.0                        |	
| Mdec-D1 | 27.3           | 0.48     | 4.52                  | 5.0                        |
| Mcav-F1 | 34.4           | 0.38      | 4.62                  | 5.0                        |
| Mcav-A6 | 15.1           | 0.86      | 4.14                  | 5.0                        |
| Dlab-B6 | 15.4            | 0.84     | 4.16                  | 5.0                        |
| Mcap-D10 | 17.6            | 0.74      | 4.26                  | 5.0                        |

**TapeStation**

After the library prep, I run samples on the tapestation (D5000), protocol linked above.

| Library prep date  | colony_id  |     Species            | Temp   |    TapeStation conc.     |   Primer set  |
| 20241120  |  Pacu-H10    | *Pocillopora acuta*          | 26.8       |    22.1          |  1  |
| 20241120  |  Pcomp-E10   | *Porites compressa*          | 26.8     |  6.52          |  2  |
| 20241121  |  Mdec-D1    | *Madracis decactis*          | 29      |    8.01        |  3   |
| 20241121  |  Mcav-F1   | *Montastraea cavernosa*          | 29     |   Below 1         |  4  |
| 20241122  |  Mcav-A6   | *Montastraea cavernosa*          | 26     |   Below 1         |  5  |
| 20241122  |  Dlab-B6   | *Diploria labyrinthiformis*          | 26     |   1.97         |  6  |
| 20241122  |  Mcap-D10   | *Montipora capitata*          | 26.8     |    8.28        |  7  |

![LibraryPrepZymo1.png](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/LibraryPrepZymo1.png?raw=true)

![LibraryPrepZymo2.png](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/LibraryPrepZymo2.png?raw=true)

![LibraryPrepZymo3.png](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/LibraryPrepZymo3.png?raw=true)


