---
layout: post
title: NEB Poly(A) mRNA enrichment prior library prep for Mcap spat samples - 111425
date: '2025-11-14'
category: Protocol
tags: [PolyA, NEB, RNA, library]
---

#### Using the NEBNext Poly(A) Magnetic Isolation Module to isolate mRNA prior in-house library prep

**Protocols used**
- [NEBNext Poly(A) Magnetic Isolation Module](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/NEBPolyA.pdf)
- [TapeStation protocol High Sensitivity RNA](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/HS-RNA_QuickGuide_TapeStation.pdf)
- [High Sensitivity RNA QBIT protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/Qubit_RNA_HS_Assay_UG.pdf)

Using the [NEBNext Poly(A) Magnetic Isolation Module](https://www.neb.com/en-us/products/e7490-nebnext-polya-mrna-magnetic-isolation-module) to isolate intact poly(A)+RNA from previously isolated total RNA. The idea is to use this kit before performing the library prep with the Zymo SwitchFree kit, and try to reduce the amount of rRNA present in the libraries.

The RNA samples I'm using here are from _Montipora capitata_ spat settled on plugs (posts [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-McapSpat2/), [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-McapSpat3/) and [here](https://fscucchia-labnotebooks.github.io/FScucchia_Putnam_Lab_Notebook/DNA-RNA-Hawaii-McapSpat1/)).

I followed the kit protocol linked above (express protocol, pages 1-3) and used 200ng of input RNA. The kit is designed to isolate intact poly(A)+ RNA from 1-5µg of previously isolated total RNA.

All samples were eluted in 15uL of elution buffer (NEBNext Tris Buffer).

## Sample prep

Here's a breakdown of input RNA volume and quantity (the kit requires a total starting volume of 50uL):

| sample_id || RNA_QBIT_AVG (ng/uL) || RNA (uL) || Ultrapure water (uL) || Total input RNA (ng) |
| B8  || 21.2 || 9.43 || 40.57 || 200 |
| C10 || 23.7 || 8.44 || 41.56 || 200 |
| D1  || 20.5 || 9.76 || 40.24 || 200 |
| A4  || 81.5 || 2.45 || 47.55 || 200 |
| A9  || 40   || 5.00 || 45.00 || 200 |
| D8  || 46   || 4.35 || 45.65 || 200 |
| C9  || 48.9 || 4.09 || 45.91 || 200 |
| C13 || 21.2 || 9.43 || 40.57 || 200 |
| B6  || 59   || 3.39 || 46.61 || 200 |
| B11 || 48.2 || 4.15 || 45.85 || 200 |
| D6  || 60.8 || 3.29 || 46.71 || 200 |
| D11 || 36.7 || 5.45 || 44.55 || 200 |
| A6  || 46.4 || 4.31 || 45.69 || 200 |
| C6  || 27   || 7.41 || 42.59 || 200 |
| D12 || 30.4 || 6.58 || 43.42 || 200 |

## Qubit Results
I used High Sensitivity RNA Qubit Protocol linked above. RNA samples were read twice, standard only read once.
- Standard 1: 52.910
- Standard 2: 1077.43

| QBIT date  || sample_id  || Species || RNA_read1 || RNA_read2 || RNA_AVG |
| 20251114 || B8  || *Montipora capitata* || 0.484 || 0.483 || 0.484 |
| 20251114 || C10 || *Montipora capitata* || 0.432 || 0.43  || 0.431 |
| 20251114 || D1  || *Montipora capitata* || 0.321 || 0.319 || 0.320 |
| 20251114 || A4  || *Montipora capitata* || 0.256 || 0.254 || 0.255 |
| 20251114 || A9  || *Montipora capitata* || 0.517 || 0.511 || 0.514 |
| 20251114 || D8  || *Montipora capitata* || 0.566 || 0.561 || 0.564 |
| 20251114 || C9  || *Montipora capitata* || 0.332 || 0.331 || 0.332 |
| 20251114 || C13 || *Montipora capitata* || 0.281 || 0.269 || 0.275 |
| 20251114 || B6  || *Montipora capitata* || 0.331 || 0.329 || 0.330 |
| 20251114 || B11 || *Montipora capitata* || 0.466 || 0.46  || 0.463 |
| 20251114 || D6  || *Montipora capitata* || 0.298 || 0.297 || 0.298 |
| 20251114 || D11 || *Montipora capitata* || 0.212 || 0.21  || 0.211 |
| 20251114 || A6  || *Montipora capitata* || 0.451 || 0.449 || 0.450 |
| 20251114 || C6  || *Montipora capitata* || 0.475 || 0.472 || 0.474 |
| 20251114 || D12 || *Montipora capitata* || 0.627 || 0.621 || 0.624 |

## TapeStation
After the isolation, I run some of the samples on the tapestation, protocol linked above for high sensitivity.
See full report [here](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/docs/2025-11-14%20-%20Hawaii_Mcap_spat_NEB_polyA.pdf).

| TapeStation date  || sample_id  ||  TapeStation conc. ng/uL |
|  20251114 || B8 ||  0.590  |
|  20251114 || C10 ||  0.548 |
|  20251114  || D1 ||   0.412  |
|  20251114  || A4 ||   0.567  |



