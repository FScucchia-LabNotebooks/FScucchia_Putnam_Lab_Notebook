---
layout: post
title: Try again with library prep using Zymo SwitchFree kit - Bermuda TPC samples
date: '2024-11-26'
category: Protocol
tags: [DNA, Zymo, RNA, library]
---

#### Trying again with library prep using the Zymo-Seq SwitchFree 3′ mRNA Library Kit for Bermuda TPC samples - Mcav and Dlab

**Protocols used**
- [Zymo-Seq SwitchFree 3′ mRNA Library Kit protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/_r3008_r3009__zymo_seq_switchfree_3_mrna_library_kit.pdf)
- [Zymo Clean & Concentrator-5 kit protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/_r1013_r1014_r1015_r1016_rna_clean_concentrator-5.pdf)
-
-
-
-



Using the [Zymo-Seq SwitchFree 3′ mRNA Library Kit](https://www.zymoresearch.com/products/zymo-seq-switchfree-3-mrna-library-kit) to try again preparing libraries starting from RNA samples exctracted from adult coral fragments from the Hawaii and Bermuda TPC project. The library prep for Mcav and Dlab RNA samples has not worked so far, so I'm trying again by first cleaning the RNA with the [Zymo Clean & Concentrator-5 kit](https://www.zymoresearch.com/products/rna-clean-concentrator-5) and slightly increasing the input RNA concentration from 13 to 15ng.
Cleaning the RNA should get rid of potential PCR inhibitors that might cause failure of the library prep for these species.

For the library prep I followed the protocol of [Jill Ashey](https://github.com/JillAshey/JillAshey_Putnam_Lab_Notebook/blob/master/_posts/2024-03-29-Zymo-SwitchFree.md).
The kit needs a minimum of 10 ng of total RNA or a maximum of 500 ng of total RNA. I'm using 15 ng and the same number of cycles as my previous attempts, 21 PCR amplification cycles (maximum recommended by the zymo kit for <100ng input RNA).

## RNA clean up
I've followed the [Zymo Clean & Concentrator-5 kit](https://www.zymoresearch.com/products/rna-clean-concentrator-5) protocol above and [this post](https://zdellaert.github.io/ZD_Putnam_Lab_Notebook/Pooling-and-Concentrating-RNA-Clean-Concentrate-2023-05-05/) by Zoe. The minimun sample volume for this kit is 50ul and the column binding capacity is 10ng of RNA, so I'm taking an aliquot from the original RNA sample and adding RNAse-free water.
I will do the cleanup on just the Mcav-F1 sample, then do the library prep for the cleaned Mcav-F1, non-cleaned Mcav-F1 and an additional non-cleaned Dlab-A1 sample.

Here's a breakdown of input RNA volume for the RNA clean-up (QBIT and extraction by Zoe):

|sample_id   || RNA_QBIT_AVG (ng/uL)|| RNA (uL) || Ultrapure water (uL) || Total starting volume (ul) |
| Mcav-F1       || 34.4     ||     10      ||   40                 || 50                        |

Sample eluted after the cleanup in 8ul.

**QBIT after RNA cleanup**

I measured the RNA concentration of the cleaned RNA and of the original RNA sample (non-cleaned), I used the high sensitivity assay.

- Mcav-F1 cleaned: 7.82 ng/ul read 1, 7.44 read 2
- Mcav-F1 non-cleaned: 15.0 ng/ul read 1, 13.9 read 2 *much lower than Zoe's initial qbit

**TapeStation after RNA cleanup**

I run the Mcav-F1 cleaned and non-cleaned on the TS using the High Sensitivity reagents and tape. 
The RIN of the cleaned RNA sample is lower than the non-cleaned but still ok for the library prep kit (>4).

![LibraryPrepZymo4.png](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/LibraryPrepZymo4.png?raw=true)


## Library prep
I run the library prep protocol linked above, with the 2 Mcav-F1 cleaned and non-cleaned samples and Dlab-A1 sample.
Input RNA 15 ug total.

Here's a breakdown of input RNA volume:

| sample_id | RNA_QBIT_AVG (ng/uL) | RNA (uL) | Ultrapure water (uL) | Total starting volume (ul) |
| Mcav-F1_clean | 7.63           | 1.97     | 3.03                  | 5.0                        |
| Mcav-F1 | 14.45           | 1.04      | 3.96                  | 5.0                        |
| Dlab-A1 | 12.6            | 1.19     | 3.81                  | 5.0                        |


**TapeStation**

After the library prep, I run samples on the tapestation (D5000).

| Library prep date  || sample_id  ||     Species            || Temp   ||    TapeStation conc.     ||   Primer set  |
| 20241126  ||  Mcav-F1_clean    || *Montastraea cavernosa*          || 29       ||    Below 1          ||  8  |
| 20241126  ||  Mcav-F1   || *Montastraea cavernosa*          || 29     ||   Below 1         ||  9  |
| 20241126  ||  Dlab-A1   || *Diploria labyrinthiformis*          || 29     ||   Below 1        ||  10  |


![LibraryPrepZymo5.png](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/LibraryPrepZymo5.png?raw=true)
