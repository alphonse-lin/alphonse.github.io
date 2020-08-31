---
layout: transcript
title:  CHEM 370 Week 4 Activity
permalink: /chem370/assignments/week04
---

# Introduction

In this tutorial you'll learn how to conduct a linear regression in R.

You'll prepare a calibration curve from standard data and calculate the concentration and associated confidence interval for an unknown sample.

You'll also use linear regression to compare two methods.

You will create an R script as you complete this exercise.  You will turn it in for a grade.  

Use the *pseudocode* to help you as you go along (this is code that looks functional but doesn't actually run, usually used to convey examples). You can reveal hints as you go along when you get stuck by clicking the "HINT" links.  

# Preparing a Standard Curve

In this portion of the exercise, you'll prepare a standard curve from data collected using [NIOSH Method 3500](http://www.cromlab.es/Articulos/Metodos/NIOSH/NIOSH%203000/3500.pdf).

This data set comes pre-packaged with R.  The dataset is called `Formaldehyde`.

1. Open RStudio and create an empty R script by clicking **New File** button and choosing **R Script**.

1. **Create a data frame that contains the `Formaldehyde` dataset.**


```r
# save the Formaldehyde data into a data frame called `form`.
form <- Formaldehyde
plot(Formaldehyde)
data.frame(Formaldehyde)
if (form) {
  mean(x)
}
```


adfjkaldj 

```html
  <label class="tooltip-r" style = "top: 50%; left: 20px; font-size: 14px;">
   HINT
   <input type="checkbox">
     <span>
        <code>form <- Fromaldehyde</code> 
        is all you need to do!
     </span>
  </label>
```

1. 
