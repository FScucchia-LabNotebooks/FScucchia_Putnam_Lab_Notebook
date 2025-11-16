---
layout: post
title: Library prep using Zymo SwitchFree kit on spat samples with PolyA isolation and pooling - 111625
date: '2025-11-16'
category: Protocol
tags: [DNA, Zymo, RNA, library]
---

#### Using the Zymo-Seq SwitchFree 3′ mRNA Library Kit for in-house library prep of coral spat samples treated for PolyA isolation and pooling - 111625

**Protocols used**
- [Zymo-Seq SwitchFree 3′ mRNA Library Kit protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/_r3008_r3009__zymo_seq_switchfree_3_mrna_library_kit.pdf)
- [NEBNext Poly(A) Magnetic Isolation Module](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/NEBPolyA.pdf)
- [TapeStation protocol high sensitivity DNA D1000](https://github.com/meschedl/MESPutnam_Open_Lab_Notebook/blob/master/_posts/2019-07-30-DNA-Tapestation.md)
- [High Sensitivity dsDNA QBIT protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/MAN0017455_Qubit_1X2_dsDNA_HS_Assay_Kit_UG.pdf)

Using the [Zymo-Seq SwitchFree 3′ mRNA Library Kit](https://www.zymoresearch.com/products/zymo-seq-switchfree-3-mrna-library-kit) (CAT.  R3009-A, LOT. 252649) to prepare libraries starting from RNA samples exctracted from coral spat of _Montipora capitata_. RNA extraction posts can be found [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-McapSpat2/), [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-McapSpat3/) and [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-McapSpat1/).
NEB PolyA treatment post can be found [here](hhttps://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/PolyAenrichment-NEB-McapSpat/).

The idea is to use the NEB kit before performing the library prep to reduce the amount of rRNA present in the libraries.

For the library prep I followed the protocol of [Jill Ashey](https://github.com/JillAshey/JillAshey_Putnam_Lab_Notebook/blob/master/_posts/2024-03-29-Zymo-SwitchFree.md) and the kit protocol above. I'm using 1.05 ng of RNA input.

Here I'm using UDI primers from the 96 well plate (CAT. D3096, LOT. 250838) provided with the kit.

All samples were eluted in 15uL of elution buffer.

## Library prep
I ran the library prep protocol linked above. I used 23 PCR cycles. With 15 samples, it took about 7 hours to run the protocol and do QC on the final library.

Here's a breakdown of input RNA volume and quantity:

| sample_id || RNA_QBIT_AVG (ng/uL) || RNA (uL) || Ultrapure water (uL) || Total input RNA (ng) |
| B8  || 0.4835 || 2.17 || 2.83 || 1.05 |
| C10 || 0.431  || 2.44 || 2.56 || 1.05 |
| D1  || 0.32   || 3.28 || 1.72 || 1.05 |
| A4  || 0.255  || 4.12 || 0.88 || 1.05 |
| A9  || 0.514  || 2.04 || 2.96 || 1.05 |
| D8  || 0.5635 || 1.86 || 3.14 || 1.05 |
| C9  || 0.3315 || 3.17 || 1.83 || 1.05 |
| C13 || 0.275  || 3.82 || 1.18 || 1.05 |
| B6  || 0.33   || 3.18 || 1.82 || 1.05 |
| B11 || 0.463  || 2.27 || 2.73 || 1.05 |
| D6  || 0.2975 || 3.53 || 1.47 || 1.05 |
| D11 || 0.211  || 4.98 || 0.02 || 1.05 |
| A6  || 0.45   || 2.33 || 2.67 || 1.05 |
| C6  || 0.4735 || 2.22 || 2.78 || 1.05 |
| D12 || 0.624  || 1.68 || 3.32 || 1.05 |

## Qubit Results
I used High Sensitivity dsDNA Qubit Protocol linked above. Library samples were read twice, standard only read once.
- Standard 1: 50.82
- Standard 2: 22722.93

| QBIT date  || sample_id  || Species ||  Library read1 || Library read2  || Library_AVG (ng/ul) |
|  20251116 || B8 || *Montipora capitata*  || LOW  || LOW  || LOW        |
|  20251116 || C10   || *Montipora capitata* || 3.98  || 3.88     || 3.93       |
|  20251116 || D1 || *Montipora capitata*  || 4.58  || 4.48   || 4.53       |
|  20251116 || A4 || *Montipora capitata*  || 5.08  || 5.00   || 5.04       |
|  20251116 || A9 || *Montipora capitata*  ||  9.88 ||  9.66  || 9.77       |
|  20251116 || D8 || *Montipora capitata*  || 9.30  ||  9.18  || 9.24       |
|  20251116 || C9 || *Montipora capitata*  ||  3.16 || 3.10   || 3.13       |
|  20251116 || C13 || *Montipora capitata*  || 12.5  || 12.0   || 12.25      |
|  20251116 || B6 || *Montipora capitata*  || 1.75  || 1.76   || 1.755      |
|  20251116 || B11 || *Montipora capitata*  || 14.1  || 13.9   || 14.0       |
|  20251116 || D6 || *Montipora capitata*  || 18.9  || 18.7   || 18.8       |
|  20251116 || D11 || *Montipora capitata*  ||21.8   ||  21.2  || 21.5       |
|  20251116 || A6 || *Montipora capitata*  || 14.7  || 14.6   || 14.65      |
|  20251116 || C6 || *Montipora capitata*  || 12.2  || 12.0   || 12.1       |
|  20251116 || D12 || *Montipora capitata*  ||  15.5 || 15.2   || 15.35      |

## TapeStation
After the library prep, I run samples on the tapestation (HS D1000), protocol linked above.
Full tapestation report [here](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/docs/2025-11-16%20-%20Hawaii_Mcap_spat_polyA_LIBRARIES.pdf).

| TapeStation date  || sample_id  ||  TapeStation conc. pg/uL ||   Primer set  |
|  20251116 || B8 || 2.59  || 17 |
|  20251116 || C10 || 2410  || 18 |
|  20251116 || D1 || 2320  || 19 |
|  20251116 || A4 || 293  || 20 |
|  20251116 || A9 || 4500  || 21 |
|  20251116 || D8 ||  / || 22 |
|  20251116 || C9 || 1520  || 23 |
|  20251116 || C13 || 4890  || 24 |
|  20251116 || B6 || 424  ||  25|
|  20251116 || B11 || 6610  ||  26|
|  20251116 || D6 || 7000  ||  27|
|  20251116 || D11 || 8660  ||  28|
|  20251116 || A6 || 7640  ||  29|
|  20251116 || C6 || 5730  ||  30|
|  20251116 || D12 || 7130  ||  31|

- it is weird that D8 has 9.24ng/ul from the qbit and nothing from the tapestation, I will re-run this sample.

![vacuum.png](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/images/Mcap_spat_libraries.png?raw=true)

## Libraries pooling

Pooling calculations were done following [Zoe's protocol](https://zdellaert.github.io/ZD_Putnam_Lab_Notebook/Switch-Free-TimeSeries-Library-Prep-Test/).

| Library_prep_date || Species || Sample.ID || Library_ID || Primer || TubeID || Average_Qubit_Conc || TS_Peak_Size || Molarity_nM_Qubit || Amount_Library_0.67nM - POOL 1 |



