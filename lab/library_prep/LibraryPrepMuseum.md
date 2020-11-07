---
title: Protocol for Construction of Blunt-End Illumina Libraries
date: \vspace{-6ex}Last revised 26 October 2020
geometry: margin=2.5cm
---

Single index blunt-end Illumina library construction for ancient and historical samples, following Meyer & Kircher 2010 (Meyer oligos and NEBNext E6070L kit). Protocol provided originally by Nicolas Dussex (contact: Nicolas.dussex@gmail.com). This version received from Leidys Murillo and Hamid Ghanavi and reformatted and maintained by Zachary Nolen.

#### Key Considerations:

* Use LoBind Eppendorf tubes.
* Avoid keeping finished libraries out of the fridge for too long and avoid freeze/thaw cycles.
* Index primers are diluted to 100 µM (stock) and stored in freezer, make 1:10 dilutions to working stock (10 µM/µL), these cannot be kept.
* Don't vortex solutions after adding enzymes, rather mix by flicking the tubes.
* Ensure to UV enough filter tips, LoBind tubes, and PCR tubes and trays the night before each work day.

# Buffer Preparation

**Done once, then again when run out**

1. Make Oligo Hybridization Buffer (20 ml for 200 reactions):

| Reagent      | Stock Conc. | Final Conc. | Volume from Stock (ml) |
| :----------- | ----------- | ----------- | ---------------------- |
| NaCl         | 0.5 M       | 500 mM      | 19.76                  |
| Tris-Cl pH 8 | 1 M         | 10 mM       | 0.2                    |
| EDTA pH 8    | 0.5 M       | 1 mM        | 0.04                   |

2. Make Adapter Hybridization Mix (100 µl for 200 reactions):

*  Make P5 hybridization mix (200 µM):

| Reagent                    | Stock Conc. | Final Conc. | Volume from Stock (µl) |
| -------------------------- | ----------- | ----------- | ---------------------- |
| IS1_adapter_P5.F           | 500 µM      | 200 µM      | 40                     |
| IS3_adapter_P5+P7.R        | 500 µM      | 200 µM      | 40                     |
| Oligo Hybridization Buffer | 10X         | 1X          | 10                     |
| ddH~2~0                    |             |             | 10                     |

*  Make P7 hybridization mix (200 µM):

| Reagent                    | Stock Conc. | Final Conc. | Volume from Stock (µl) |
| -------------------------- | ----------- | ----------- | ---------------------- |
| IS2_adapter_P7.F           | 500 µM      | 200 µM      | 40                     |
| IS3_adapter_P5+P7.R        | 500 µM      | 200 µM      | 40                     |
| Oligo Hybridization buffer | 10X         | 1X          | 10                     |
| ddH~2~0                    |             |             | 10                     |

* Mix and incubate the reactions for **10 sec** at **95°C**, followed by a **ramp** from **95°C to 12°C** at a rate of **0.1°C/sec** (eg. **-1°/10sec**) (**Adapter1** program).

* Combine both reactions as ready to use mix, with **100 µM** of **each adapter**. Can be saved in freezer.

# Day 1 - Blunt-End Repair and Adapter Ligation

Required reagents:

* Tango Buffer (10X)
* dNTPs (25 mM each)
* ATP (100mM)
* T4 PNK (10 U/µl)
* T4 DNA Polymerase (5 U/µl)
* T4 DNA Ligase Buffer (10X)
* PEG-4000 (50%)
* Adapter Hybridization Mix (100 µM per adapter, prepared in [Buffer Preparation](#buffer-preparation))
* T4 DNA ligase (5U/µl)
* Isothermal Amp. Buffer (10X)
* Bst Polymerase, Large Fragment (8 U/µl)

**UV** the following for at least **4 hours** the **night before**:

* ddH~2~0

## Part 1A - Blunt-Ending

1. Remove reagents from freezer, ensure **ATP** is **covered in foil**, and all enzymes are in the **cold block**.

2. Prepare master mix:

   | Reagent           | Stock Conc. | Final Conc. | Volume/Sample (µl) | MM x13 Samples (µl) |
   | ---------------------- | ------------------- | ------------|----------|------------|
   | Tango Buffer      | 10X         | 1X          | 4                  | 52                  |
   | dNTPs             | 25 mM       | 100 µM      | 0.16               | 2.08                |
   | ATP               | 100 mM      | 1 mM        | 0.4                | 5.2                 |
   | T4 PNK            | 10 U/µl     | 0.5 U/µl    | 2                  | 26                  |
   | T4 DNA Polymerase | 5 U/µl      | 0.1 U/µl    | 0.8                | 10.4                |
   | ddH~2~0           |             |             | 12.64              | 164.32              |
   | DNA               |             |             | 20                 |                     |
   |                   |             |             |                    |                     |
   | Total Volume | | | 40 | |

3. Add **20 µl master mix** to clean labeled **PCR tubes**.

4. Add **20 µl sonicated DNA**, briefly **spin down**.

5. Incubate for **15 min** at **25°C**, followed by **5 min** at **12°C** (**Nouser** program).

6. Turn on **incubator to 37°C** and prepare MinElute Columns while running.

7. Place reactions on ice or immediately proceed to next step (total reaction volume: 40 µl).

## Part 1B - MinElute Reaction Clean-Up

1. Add **40 µl reactions** from above to **new LoBind Eppendorf tubes**.

2. Add **200 µl PB buffer** to each, **mix by pipetting**.

3. **Apply mix to MinElute column** and **spin** at **13,000 rpm** for **1 min**.

4. **Discard waste** and change to **new collection tube**.

5. **Wash with PE Buffer**:
   * Apply **700 µl of PE Buffer** to column and **spin** at **13,000 rpm** for **1 min**.
   * **Discard waste** and change to **new collection tube**.

6. **Repeat step 5**.

7. **Spin** at **13,000 rpm** for **1 min** to dry column.

8. **Discard waste** and place column in **new, labeled LoBind Eppendorf tube**.

9. Leave column with open lid for **5 min** to dry out column.

10. Apply **22 µl** of **EB buffer** to column, incubate at **37°C** for **5 min**.

11. **Elute DNA** by spinning at **13,000 rpm** for **1 min**.

## Part 2A - Adapter Ligation

1. Remove reagents from freezer, check that **T4 ligase buffer** has **no precipitate** after thawing. If present, warm to **37°C** and **vortex** until precipitate is dissolved.

2. **Adapter hybridization mix** (see [Buffer Preparation](#buffer-preparation)) needs to be **diluted 1:10** before adding to the master mix. **Note**: This dilution needs to be made fresh each time (**1.5 µl adapter hybridization mix**, **13.5 µl ddH~2~0** for 13 samples).

3. Prepare master mix:

   | Reagent              | Stock Conc. | Final Conc. | Volume/Sample (µl) | MM x13 Samples (µl) |
   | -------------------- | ----------- | ----------- | ------------------ | ------------------- |
   | T4 DNA Ligase Buffer | 10X         | 1X          | 4                  | 52                  |
   | PEG-4000             | 50%         | 5%          | 4                  | 52                  |
   | Adapter hybrid. mix* |             |             | 1                  | 13                  |
   | T4 DNA Ligase        | 5 U/µL      | 0.125 U/µL  | 1                  | 13                  |
   | ddH20                |             |             | 10                 | 130                 |
   | Blunt-ended DNA      |             |             | 20                 |                     |
   |                      |             |             |                    |                     |
   | Total Volume         |             |             | 40                 |                     |

   *Prepared in previous step.

4. Add **20 µl master mix** to new **PCR tubes**.

5. Add **20 µl** of **Blunt-ended DNA** from Part 1. Briefly spin down.

6. Incubate for **30 min** at **22°C** (**Adapter2** program).

7. Turn on **incubator to 37°C** and prepare MinElute Columns while running.

## Part 2B - MinElute Reaction Clean-Up

1. Add **40 µl reactions** from above to **new LoBind Eppendorf tubes**.

2. Add **200 µl PB buffer** to each, **mix by pipetting**.

3. **Apply mix to MinElute column** and **spin** at **13,000 rpm** for **1 min**.

4. **Discard waste** and change to **new collection tube**.

5. **Wash with PE Buffer**:
   * Apply **700 µl of PE Buffer** to column and **spin** at **13,000 rpm** for **1 min**.
   * **Discard waste** and change to **new collection tube**.

6. **Repeat step 5**.

7. **Spin** at **13,000 rpm** for **1 min** to dry column.

8. **Discard waste** and place column in **new, labeled LoBind Eppendorf tube**.

9. Leave column with open lid for **5 min** to dry out column.

10. Apply **22 µl** of **EB buffer** to column, incubate at **37°C** for **5 min**.

11. **Elute DNA** by spinning at **13,000 rpm** for **1 min**.

## Part 3 - Adapter Fill-In

1. Remove reagents from freezer, ensure the **Isothermal Amp Buffer** has **not precipitated** before starting. If present, warm to **37°C** and **vortex**.

2. Prepare master mix:

   | Reagent               | Stock Conc. | Final Conc. | Volume/Sample (µl) | MM x13 Samples (µl) |
   | --------------------- | ----------- | ----------- | ------------------ | ------------------- |
   | Isothermal Amp Buffer | 10X         | 1X          | 4                  | 52                  |
   | dNTPs                 | 25 mM       | 250 µM      | 0.4                | 5.2                 |
   | Bst Polymerase, LF    | 8 U/µl      | 0.3 U/µl    | 1.5                | 19.5                |
   | ddH20                 |             |             | 14.1               | 183.3               |
   | Adapter-ligated DNA   |             |             | 20                 |                     |
   |                       |             |             |                    |                     |
   | Total Volume          |             |             | 40                 |                     |

3. Add **20 µL master mix** to new **PCR tubes**.

4. Add **20 µL adapter ligated DNA** from Part 2. Briefly spin down.

5. Incubate at **37°C** for **20 min**, followed by **80°C** for **20 min** to inactivate the Bst Polymerase (**Fill-In** program).



**Safe stopping point - Libraries can be stored in the freezer overnight or until ready to do the next step. Can be transferred to clean, labeled LoBind tubes for easier storage**

\newpage

# Day 2 - Indexing

Reagents required:

* AccuPrime Reaction Mix (10X)
* AccuPrime Pfx
* Index Combinations

**UV** the following for at least **4 hours** the **night before**:

* ddH~2~O
* PCR plates and strip caps

## Part 4A - Indexing PCR Test

1. Remove index combinations from the freezer. Prepare **1:10 dilutions** (**1 µl primer, 9 µl ddH~2~O**). These **cannot** be kept **overnight**.

2. Prepare PCR master mix (Always do **1x negative reaction** for the first library test):

   | Reagent                | Stock Conc. | Final Conc. | Volume/Sample (µl) | MM x14 samples (µl) |
   | ---------------------- | ----------- | ----------- | ------------------ | ------------------- |
   | AccuPrime reaction mix | 10X         | 1X          | 2.5                | 35                  |
   | AccuPrime Pfx          |             |             | 0.5                | 7                   |
   | ddH~2~O                |             |             | 16.75              | 234.5               |


3. Add **20.5 µl master mix**.

4. Add **0.75 µl** of **Index Primer 1**.

5. Add **0.75 µl** of **Index Primer 2**.

6. Add **3 µl adapter-ligated DNA** from Part 3. Spin tubes down.

7. Incubate using cycler program **Index**: 2 min at 95°C, (15 sec at 95°C, 30 sec at 60°C, 60 sec at 68°C) x 15 cycles, hold at 4°C for infinity.

8. Make **0.8% agarose gel**, run **5 µl** of **PCR product** on gel at **100V** for **2 hours** with **1kb+ ladder** for sizing. It is important you can determine the size of the library and you can distinguish between primer and library bands as the size is key to pooling the samples.

9. Based on the brightness of the library, determine how many cycles for the next round. If too bright, reduce to 12, too weak, increase to 18, if okay, leave at 15.

## Part 4B - Indexing PCR

**Note**: If you determined a different cycle number for some samples, you will need to prepare one plate per cycling count, putting only the samples requiring the same cycle count on the same plate.

1. If new index dilutions are needed, prepare first as in Part 4A.

2. Prepare master mix for **5 reactions per sample**:

   | Reagent                | Stock Conc. | Final Conc. | Volume/Sample (µl) | MM x65 samples (µl) |
   | ---------------------- | ----------- | ----------- | ------------------ | ------------------- |
   | AccuPrime reaction mix | 10X         | 1X          | 2.5                | 162.5               |
   | AccuPrime Pfx          |             |             | 0.5                | 32.5                |
   | ddH~2~O                |             |             | 16.75              | 1088.75             |

\smallskip
For each batch with the same cycle count, prepare a PCR plate:

3. Add **20.5 µl master mix** to **5 wells per sample**.

4. Add **0.75 µl** of **Index Primer 1** to **same 5 wells per sample**.

5. Add **0.75 µl** of **Index Primer 2** to **same 5 wells per sample**.

6. Add **3 µl** of **adapter-ligated DNA** from Part 3 to the **same 5 sample wells**.

7. Spin the plate down briefly and run on the **Index** program from Part 4A, Step 7, with the **cycle number adjusted** based on the number determined for each set of samples. Be sure to record the cycle count for each sample.

8. **Pool the 6 reactions** (these 5 plus the reaction from Part 4A) into a **single LoBind Eppendorf tube** for each sample.



**Safe stopping point - Libraries can be stored in the freezer overnight or until ready to do the next step. Pooling to single Eppendorf tube in last step can also wait until the next step.**

\newpage

# Day 3 - Size Selection and Purification

Required reagents:

* Speedbeads
* 1% Tween

**UV** the following for at least **4 hours** the **night before**:

* ddH~2~O
* TE Buffer
* 95% EtOH (do not reuse EtOH that has been UV'd several times)

**Note**: Always use clean fresh 80% ethanol from clean and pure 99% ethanol and thoroughly vortex before use.

1. Remove Speedbeads from the fridge at least 30 mins before starting. Ensure beads are well mixed before use. Do not shake the beads to mix, or else bubbles will form. Instead, gently rock or rotate to mix.

2. Prepare TE-tween mix by mixing 800 µl UV-treated TE buffer with 40 µl 1% Tween. Cover tube with foil.

3. Prepare fresh 80% EtOH (42 ml 95% EtOH with 8 ml ddH~2~O).

4. Allocate 100 µl of PCR product from Part 4 to a new LoBind tube. This new tube will be carried forward.

5. Add 50 µl Speedbeads to the PCR product (0.5X volume). Ensure beads are well mixed before use.

6. Vortex, pulse spin, and incubate at room temperature for 5 min.

7. Place tubes on magnetic rack for 1 min or until all beads have migrated to wall and supernatant is clear.

8. Carefully remove supernatant to new LoBind tube without disturbing the pellet.
   * The pellet contains long fragments that you don't need. As a precaution, add 20 µl TE buffer to the pellet and store in the fridge.)

9. Add 270 µl Speedbeads to supernatant (1.8X volume). Ensure beads are well mixed before use.

10. Vortex, pulse spin, and incubate at room temperature for 10 min.

11. Place tube on rack and incubate for 3 min or until beads have migrated to wall and supernatant is clear.

12. While on rack, discard supernatant, keeping the pellet. The beads are attached to the fragments you want.

13. While on rack, add 500 µl EtOH, incubate for 1 min, then remove by pipetting.

14. Repeat Step 13 two more times.

15. Remove from rack and very quickly pulse spin to collect EtOH at the bottom of the tube.

16. Place back on magnetic rack, when beads have migrated to the wall, open carefully to stop ethanol moving, and remove any excess with small pipette.

17. Leaving the tubes open on the rack, air dry to remove all EtOH.
    * This step is critical and any carryover EtOH will interfere with downstream sequencing. The pellet should look like mud when dry. If it is shiny, wait until it is no longer. It is better to over dry than to under dry your samples.

18. Remove tube from rack and add 36 µl TE-tween buffer.

19. Vortex for 20 sec.

20. Pulse spin and incubate at room temperature for 5 min.

21. Place on magnetic rack for 5 minutes or until the supernatant is clear.

22. Remove 3 µl supernatant and transfer to a set of clean, labelled LoBind tubes for pico green analysis.

23. Remove the remainder of the library to clean, LoBind tubes, being very careful not to disturb the beads. Store in freezer until pooling.
    * If you disturb the beads, pulse spin sample and place back on rack until supernatant is clear again. It is crucial you don't carry over any of the beads, as this tube now contains the final library.

**Safe stopping point - Libraries can be stored in the freezer overnight or until ready to pool.**



