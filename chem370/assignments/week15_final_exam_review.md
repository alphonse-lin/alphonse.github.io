---
layout: transcript
title: Final Exam Review
---

# What to Expect

The final will be composed of short answer questions.  It is open book and open notes, and you will have 24 hours to complete the exam.  You may use online databases (e.g. NIST Web Book, PubChem) and primary literature, so long as you cite them as sources.  You may not confer with other students about the exam and you may not use online study sites, discussion boards, Q & A sites, etc., to answer questions.  Online course materials and video lectures may not be available during the exam period.

You will be able to write your answers by hand and scan them to a PDF or complete them in a word processor and save them to a PDF.  You should still show your work for calculation problems.  You may use a calculator, R, or spreadsheet program to do your calculations.  You should make arrangements now to be able to download and/or print the exam (sent as a PDF), complete the exam, and scan/save/send your completed exam by the deadline (for example, if home does not have a good internet connection you should figure out how you plan to submit the exam now rather than at the last minute).

Our exam period is Wednesday, December 2 from 08:30-11:00.  I will email you an exam no later than 00:00 on December 2 and you will have until 23:59:59 on December 2 to turn it in. Obviously it won't take you 24 hours to complete, but I will expect coherent, polished answers given the open-book nature of the exam.

Some example questions are below.  They are meant to give you an idea of what the questions will be like.  They are not meant to cover everything that will be on the exam!

# Example Problems

1. Below are several two data sets from separate instruments (A and B) that measured the concentration of nitrogen dioxide in air.  For each data set, determine: (show your work)

    - The sensitivity factor, $k_A$.
    - The concentration of the unknown (+/- 95% CI).
    - Whether the two techniques give significantly different results, or if they are the same.
    - Possible reasons for any differences observed.
    - Any other differences you observe (linearity, signs of interference, precision, etc.)
    
   | concentration (ppb) | signal-A | signal-B |
   | ------------------- | -------- | -------- |
   | 101 (standard)      | 205227   | 5777     |
   | 110 (standard)      | 332425   | 6250     |
   | 122 (standard)      | 368677   | 6955     |
   | 137 (standard)      | 414007   | 7809     |
   | 160 (standard)      | 483772   | 9223     |
   | unknown (rep 1)     | 377761   | 7156     |
   | unknown (rep 2)     | 377776   | 7141     |
   | unknown (rep 3)     | 377752   | 7179     |
      

2. Discuss, from a statistical perspective, why FT-IR is superior to dispersive IR.

3. You have been asked to measure calcium concentration in water originating from a carbonate bedrock aquifer.  Choose the best technique for this, and discuss:

    - Why you chose the technique.  If there is more than one suitable method for the analysis, discuss why you chose one over the other.
    - Any unique challenges this analyte and/or matrix might present, and what you would do to overcome them.
  
1. Rank the following molecules from shortest $\lambda\_{max}$ to longest: pentacene, anthracene, naphthalene, benzene, hexacene.  Discuss why this trend exists.

1. You work as a chemist at an analytical lab that has just acquired a major contract from an environmental consulting firm remediating the site of a former herbicide factory.  You will need to test many samples for trace-levels of (1) 2,4-D, (2) atrazine, and (3) glyphosate.  What technique(s) would choose and why?  Include a discussion of the specific detector you would choose and why that detector is good for this particular analysis.

    <!-- soot! -->

    <!-- 4.9.9Nickel -- High concentrations of iron, cobalt, or chromium may interfere,requiring either matrix matching or use of a nitrous-oxide/acetylene flame.  A non-response line of Ni at 232.14 nm causes non-linear calibration curves at moderate to highnickel concentrations, requiring sample dilution or use of the 352.4 nm line. -->


1. You are building a time-of-flight mass spectrometer.  In this instrument, ions are separated by mass-to-charge ratio as they travel over a distance of 2-3 meters.  Discuss specific devices you could use to move ions over this distance.

1. The term "hyphenated technique" is used to describe methods that combine two or more techniques, such as ICP-MS, which couples an inductively coupled plasma to a mass spectrometer.  Discuss how the hyphenated nature of GC-MS makes it more powerful than either of the techniques individually.  What are problems that would arise for either method on it's own?

1. Determine the structure of the compound represented by the spectra below.  Show your work.

**IR Spectrum**

![unknown 5 ms]({{site.url}}\chem370\assignments\img\unk5ir.png)

<div class="check-understanding">
   What functional groups might be present in this molecule?
   <label class="tooltip-understand" style = "top: 50%; left: 20px; font-size: 14px;">
    ANSWER 
    <input type="checkbox">
   <span>
         The sharp, medium-intense peak at ~3050 cm^-1 is indicative of an aromatic hydrocarbon, as are the peaks below 1000 cm^-1.  There is little evidence for anything else in the spectrum.
   </span>
   </label>
</div>

**Mass Spectrum**

![unknown 5 ms]({{site.url}}\chem370\assignments\img\unk5ms.png)

<div class="check-understanding">
   What is the A peak (molecular ion)?
   <label class="tooltip-understand" style = "top: 50%; left: 20px; font-size: 14px;">
    ANSWER 
    <input type="checkbox">
   <span>
         There are several logical options for the molecular ion.  180 might make sense, but the C count does not work out using only C and H for a molecular weight of 180 (since the IR shows no evidence of anything else).  Another choice could be 178.  Test this out, we see percent abundances for A, A+1, A+2, and A+3 of 9999/9999 = 100%, 1569/9999 = 15.7%, 149/9999 = 1.5%, 30/9999 = 0.3%, respectively.  From isotopic contributions for carbon (i.e. Table 2.2 in McLafferty), these ratios suggest a C-14 or C-15 compound.  I will assume the 178 is the M.W. and move forward.
   </span>
   </label>
</div>

<div class="check-understanding">
   How many C atoms are there in this molecule?
   <label class="tooltip-understand" style = "top: 50%; left: 20px; font-size: 14px;">
    ANSWER 
    <input type="checkbox">
   <span>
         Using a M.W. of 178 and the guess of C-14 or C-15 from the previous answer: 15*12=180, which is too much; 14*12=168, which seems about right.  I will rule out C-15 and assume the molecule is C-14.
   </span>
   </label>
</div>

<div class="check-understanding">
   What does the nitrogen rule tell you about the molecule?
   <label class="tooltip-understand" style = "top: 50%; left: 20px; font-size: 14px;">
    ANSWER 
    <input type="checkbox">
   <span>
         A is even, so there is like 0 or 2 N atoms.  The IR shows no evidence of N, so likely there is 0.
   </span>
   </label>
</div>

<div class="check-understanding">
   Can you come up with a formula?
   <label class="tooltip-understand" style = "top: 50%; left: 20px; font-size: 14px;">
    ANSWER 
    <input type="checkbox">
   <span>
         The IR suggests only (aromatic) C and H, so let's start there.  Isotopic abundances and inference from the M.W. suggests 14 C.  C14 = 168, meaning we need 10 H to make up the difference.  C14H10 works for the M.W.  
   </span>
   </label>
</div>

<div class="check-understanding">
   Can you find evidence of a particular structure from the formula you determined?
   <label class="tooltip-understand" style = "top: 50%; left: 20px; font-size: 14px;">
    ANSWER 
    <input type="checkbox">
   <span>
         The formula C14H10 would require 14-0.5*10+1 = 9 rings or double bonds!  This is highly suggestive of an aromatic molecule, which agrees with the IR.  The molecular ion is also the base peak, meaning the entire molecule is very stable.  Actually, the most common loss seems to be losing 1 or two hydrogen.  All of this together suggests a structure like anthracene. [anthracene]
   </span>
   </label>
</div>


| Ion [m/z] | Intensity [counts] | Intensity [%] |
| --------- | ------------------ | ------------- |
| 27.0      | 20.0               | 0.0936        |
| 28.0      | 10.0               | 0.0468        |
| 38.0      | 30.0               | 0.1404        |
| 39.0      | 109.0              | 0.5102        |
| 50.0      | 129.0              | 0.6038        |
| 51.0      | 129.0              | 0.6038        |
| 52.0      | 30.0               | 0.1404        |
| 61.0      | 40.0               | 0.1872        |
| 62.0      | 129.0              | 0.6038        |
| 63.0      | 289.0              | 1.3527        |
| 64.0      | 20.0               | 0.0936        |
| 65.0      | 20.0               | 0.0936        |
| 69.0      | 20.0               | 0.0936        |
| 73.0      | 10.0               | 0.0468        |
| 74.0      | 219.0              | 1.0250        |
| 75.0      | 299.0              | 1.3995        |
| 76.0      | 619.0              | 2.8973        |
| 77.0      | 80.0               | 0.3744        |
| 78.0      | 10.0               | 0.0468        |
| 83.0      | 50.0               | 0.2340        |
| 85.0      | 30.0               | 0.1404        |
| 86.0      | 99.0               | 0.4634        |
| 87.0      | 169.0              | 0.7910        |
| 88.0      | 439.0              | 2.0548        |
| 89.0      | 759.0              | 3.5525        |
| 90.0      | 10.0               | 0.0468        |
| 98.0      | 119.0              | 0.5570        |
| 99.0      | 90.0               | 0.4212        |
| 100.0     | 50.0               | 0.2340        |
| 101.0     | 50.0               | 0.2340        |
| 102.0     | 60.0               | 0.2808        |
| 110.0     | 40.0               | 0.1872        |
| 111.0     | 50.0               | 0.2340        |
| 113.0     | 60.0               | 0.2808        |
| 114.0     | 20.0               | 0.0936        |
| 115.0     | 50.0               | 0.2340        |
| 122.0     | 40.0               | 0.1872        |
| 123.0     | 20.0               | 0.0936        |
| 124.0     | 20.0               | 0.0936        |
| 125.0     | 50.0               | 0.2340        |
| 126.0     | 149.0              | 0.6974        |
| 127.0     | 60.0               | 0.2808        |
| 128.0     | 80.0               | 0.3744        |
| 137.0     | 30.0               | 0.1404        |
| 138.0     | 30.0               | 0.1404        |
| 139.0     | 209.0              | 0.9782        |
| 140.0     | 80.0               | 0.3744        |
| 149.0     | 70.0               | 0.3276        |
| 150.0     | 419.0              | 1.9612        |
| 151.0     | 629.0              | 2.9441        |
| 152.0     | 689.0              | 3.2249        |
| 153.0     | 80.0               | 0.3744        |
| 163.0     | 50.0               | 0.2340        |
| 164.0     | 20.0               | 0.0936        |
| 174.0     | 129.0              | 0.6038        |
| 175.0     | 199.0              | 0.9314        |
| 176.0     | 1409.0             | 6.5949        |
| 177.0     | 799.0              | 3.7398        |
| 178.0     | 9999.0             | 46.8008       |
| 179.0     | 1569.0             | 7.3438        |
| 180.0     | 149.0              | 0.6974        |
| 181.0     | 30.0               | 0.1404        |
