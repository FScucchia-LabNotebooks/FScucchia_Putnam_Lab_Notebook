---
layout: post
title: S. pistillata DNA/RNA extraction with Zymo kit
category: Extraction
tags: [ RNA, DNA, Stylophora, pH, shallow, mesophotic ]
---

Using the [Zymo Quick-DNA/RNA Miniprep Plus Kit](https://www.zymoresearch.com/collections/quick-dna-rna-kits/products/quick-dna-rna-miniprep-plus-kit) on _Stylophora pistillata_ shallow and mesophotic samples from the pH experiment. 

For this extraction I used the [protocol](https://emmastrand.github.io/EmmaStrand_Notebook/Zymo-Duet-RNA-DNA-Extraction-Protocol/) of emmastrand with some adjustments.

### Reagents preparation

1. Add 96 mL 100% ethanol (104 mL 95% ethanol) to the 24 mL DNA/RNA Wash Buffer concentrate before use. DNA/RNA Wash Buffer included with D7003T (Mini Prep Plus Kit) is supplied ready-to-use and does not require the addition of ethanol prior to use. Check kit contents and instructions to confirm prep steps.  
2. Reconstitute the lyophilized (freeze-dried) DNase I as indicated on the vial prior to use. Mix by inversion. Store frozen aliquots.  
3. Prepare the 10 mM Tris HCl following this [protocol](https://github.com/fscucchia/FScucchia_Lab_Notebook-Mass_Lab/blob/master/protocols/Tris%20HCL%2C%20RNA-DNA%20extraction.docx).

### Adult fragment sample preparation

1. Add 345 uL of DNA/RNA shield to a new 2 ml tube.  
2. Using sterilized clippers, clip off 2-3 small pieces of coral and place them in the 2 mL tube from step 1. The DNA/RNA shield needs to cover the fragments.  Sterilize clippers in between every sample.   
3. Put samples into a cell disruptor for < 2 minutes at 2000 rpm. The amount of time for vortexing will depend on the coral skeletal structure and how easily the tissue separates from the skeleton. Too much vortexing can cause DNA/RNA degradation, but too little vortexing can result in minimal DNA/RNA yield.  
4. Transfer the liquid into a new 1.5 ml tube. Save the tube with the skeleton fragment in -80°C freezer as a potential back-up in case the extraction doesn't work.  
5. Proceed to DNA Extraction steps.  

### DNA Extraction
1. Set up yellow DNA spin columns and collection tubes, label appropriately
2. Warm elution liquids to 70°C (10mM Tris HCl pH. 8.0 and RNase free water)
3. Add equal volume (345 µl) DNA/RNA lysis buffer to each sample tube
4. Finger flick to mix tubes
5. Add 700 µl (total volume) of sample gently to the yellow DNA spin column
6. Centrifuge at 16,000 rcf (g) for 30 seconds
7. **Important** Save the flow through from this step: transfer to a new 1.5mL tube labeled for RNA
8. Add 400µl DNA/RNA Prep Buffer gently to the yellow DNA spin columns
9. Centrifuge at 16,000 rcf (g) for 30 seconds
10. Discard flow through (Zymo kit waste)
11. Add 700 µl DNA/RNA Wash Buffer gently to the yellow DNA spin columns
12. Centrifuge at 16,000 rcf (g) for 30 seconds
13. Discard flow through (Zymo kit waste)
14. Add 400 µl DNA/RNA Wash Buffer genetly to the yellow DNA spin columns
15. Centrifuge at 16,000 rcf (g) for **2 minutes**
16. Discard flow through (Zymo kit waste)
17. Transfer yellow columns to new 1.5mL microcentrifuge tubes
18. Add 50 µl warmed 10 mM Tris HCl to each yellow DNA column by dripping slowly directly on the filter
19. Incubate at room temp for 5 minutes
20. Centrifuge at 16,000 rcf (g) for 30 seconds
21. Repeat steps 18-20 for a final elution volume of 100 µl
22. Label tubes, store at 4°C if quantifying the same day or the next (Nanodrop), if waiting longer store in -20°C

### RNA Extraction
*Can do concurrently with DNA Extraction after DNA Extraction Step 7*
1. Add equal volume (700 µl) 100% EtOH to the 1.5mL tubes labeled for RNA containing the original yellow column flow through
2. Vortex and spin down to mix
3. Add 700 µl of that liquid to the green RNA spin columns
4. Centrifuge at 16,000 rcf (g) for 30 seconds
5. Discard flow through (Zymo kit waste)
6. Add 700 µl to the green RNA spin columns (the rest from the 1.5mL RNA tubes)
7. Centrifuge at 16,000 rcf (g) for 30 seconds
    - Get DNase I from freezer
8. Discard flow through (Zymo kit waste)
9. Add 400 µl DNA/RNA Wash Buffer gently to each green RNA column
10. Centrifuge at 16,000 rcf (g) for 30 seconds
11. Discard flow through (Zymo kit waste)
12. Make DNase I treatment master mix:
    - 75µl DNA Digestion buffer x # of samples
    - 5µl DNase I x # of samples
13. Add 80 µl DNase I treatment master mix directly to the filter of the green RNA columns
14. Incubate at room temp for 15 minutes
15. Add 400 µl DNA/RNA Prep Buffer gently to each column
16. Centrifuge at 16,000 rcf (g) for 30 seconds
17. Discard flow through (Zymo kit waste)
18. Add 700 µl DNA/RNA Wash Buffer gently to the green RNA spin columns
19. Centrifuge at 16,000 rcf (g) for 30 seconds
20. Discard flow through (Zymo kit waste)
21. Add 400 µl DNA/RNA Wash Buffer genetly to the green RNA spin columns
22. Centrifuge at 16,000 rcf (g) for **2 minutes**
23. Discard flow through (Zymo kit waste)
24. Transfer green columns to new 1.5mL microcentrifuge tubes
25. Add 50µl warmed DNase/RNase free water to each green RNA column by dripping slowly directly on the filer
26. Incubate at room temp for 5 minutes
27. Centrifuge at 16,000 rcf (g) for 30 seconds
28. Repeat steps 25-27 for a final elution volume of 100µl
29. Label 1.5mL tubes on ice afterwards, and aliquot 5µl into PCR strip tubes to save for Nanodrop and Tape Station to avoid freeze-thaw of your stock sample
30. Store all tubes in the -80°C

#### DNA Quality  
If DNA quantity is sufficient (typically >10 ng/µL), check the quality by running the sample on an agarose gel. "Good" DNA should form a distinct band a the very top of the gel. 

#### RNA Quality  
If RNA quantity is sufficient (for sequencing you need to have a total of 500 ng per sample), determine RNA quality using the Tape Station. "Good" RNA should have a RIN above 8.0 and form two distinct peaks at the 18S and 28S locations. 