---
layout: post
title: Recommendation for troubleshooting library prep using Zymo SwitchFree kit
date: '2025-04-03'
category: Protocol
tags: [DNA, Zymo]
---

#### Recommendations from Zymo team for throubleshooting library prep using the Zymo-Seq SwitchFree 3′ mRNA Library Kit 

**Protocols used**
- [Zymo-Seq SwitchFree 3′ mRNA Library Kit protocol](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/protocols/_r3008_r3009__zymo_seq_switchfree_3_mrna_library_kit.pdf)
- [Putnam Lab refined library prep protocol](https://github.com/JillAshey/JillAshey_Putnam_Lab_Notebook/blob/master/_posts/2024-03-29-Zymo-SwitchFree.md)

**Throubleshooting details**

We sent a few of our coral RNA samples to the Zymo team to try library prepping using their kit, and they sent us the following recommendations (modified steps from the protocols linked above):

- perform SwitchFree library preparation using 10 ng of RNA
- decreasing the volume of Poly A R1 Reagent from 5 ul to 3 ul (supplementing with 2 ul of DNase/RNase Free water), it can be helpful for samples that are challenging or more prone to dimer formation (it appears that the coral samples are more prone to dimer formation than the Hela control, se Tapestation results [here](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/docs/2025-04-01_Federica_Mcap%20and%20Pacu%20coral_3'libraries%20with%20human%20Hela%20control.pdf))
- libraries amplified for 19 cycles, and the final elution is in 20 ul
- to further reduce dimers, libraries can be pooled together based on the molarity of the library region (240 - 1000 bp) and cleaned up following the last paragraph in Appendix C in the kit protocol. The extra cleanup greatly reduces the dimer without impacting the library yield too much, see Tapestation results [here](https://github.com/FScucchia-LabNotebooks/FScucchia_Putnam_Lab_Notebook/blob/master/docs/2025-04-01_Federica_Mcap%20and%20Pacu%20library%20pool_before%20and%20after%20extra%200.85x%20cleanup.pdf). Alternatively, this extra cleanup can be done on individual libraries. With the extra cleanup, you can elute in a smaller volume to further concentrate the pool if needed (elute in 15 ul instead of 20 ul)
- timing for beads drying is critical during each of the cleanups. Typically, the bead cleanups are the most sensitive part of the protocol, and there may be room for improvement