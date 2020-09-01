---
layout: transcript
title:  CHEM 370 Week 4 Activity
permalink: /chem370/assignments/week04x
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

1. Create a data frame that contains the `Formaldehyde` dataset.  Call it `form`.

   ```r
   # save the Formaldehyde data into a data frame called `form`.
   form <- Formaldehyde
   ```

   <label class="tooltip-r" style = "top: 50%; left: 20px; font-size: 14px;">
    HINT
    <input type="checkbox">
      <span>
         <code class = "r">form <- Formaldehyde</code> <br>
         is all you need to do!  Make sure you can see the data in your workspace.
      </span>
   </label>

1. Plot the data in the `form` data frame.  Don't forget to add x and y labels (with units)!
   
   Remember that you need to load the `instRumental` package if you want to use `chemplot()`.

   ```r
   plot(dataframe)
   ```
   
   <div>
      <label class="tooltip-r" style = "top: 50%; left: 20px; font-size: 14px;">
      HINT
      <input type="checkbox">
         <span>
            <code class = "r">
            require(instRumental) <br>
            chemplot(form, xlab = 'Carbohydrate Added (mL)', ylab = expression(OD[660]))</code>
         </span>
      </label>
   </div>

1. Fit a linear model to the data.  Call it `calcurve`.

   ```r
   calcurve <- lm(y ~ x, data = df)
   ```

   <div>
      <label class="tooltip-r" style = "top: 50%; left: 20px; font-size: 14px;">
      HINT
      <input type="checkbox">
         <span>
            <code class = "r">
            calcurve <- lm(optden ~ carb, data = form)</code>
         </span>
      </label>
   </div>

1. What is the sensitivity coefficient?  Call it `k.a`.

   ```r
   k.a. <- 0
   ```

   <div>
      <label class="tooltip-r" style = "top: 50%; left: 20px; font-size: 14px;">
      HINT
      <input type="checkbox">
         <span>
         You can use <code class = "r"> summary(calcurve) </code> to view the model output and find k_a.  Then type the value in place of 0 above.
         </span>
      </label>
   </div>

1. What is the $R^2$ value from the model?  Call it `rsq`.

   ```r
   rsq <- 0
   ```

   <div>
      <label class="tooltip-r" style = "top: 50%; left: 20px; font-size: 14px;">
      HINT
      <input type="checkbox">
         <span>
         You can use <code class = "r"> summary(calcurve) </code> to view the model output and find multiple R-squared.  Then type the value in place of 0 above.
         </span>
      </label>
   </div>

1. What is the intercept?  Call it `b`.

   ```r
   b <- 0
   ```

   <div>
      <label class="tooltip-r" style = "top: 50%; left: 20px; font-size: 14px;">
      HINT
      <input type="checkbox">
         <span>
         You can use <code class = "r"> summary(calcurve) </code> to view the model output and find b0.  Then type the value in place of 0 above.
         </span>
      </label>
   </div>

1. Use your calibration curve to determine the concentration and 95% confidence interval for a sample measured 3 times that yields $S_A$ = 0.6214, 0.6431, and 0.6055.  Call your answer `c.a`.

   ```r
   c.a. <- inverse.predict(model, replicates, alpha = level)
   ```

   <div>
      <label class="tooltip-r" style = "top: 50%; left: 20px; font-size: 14px;">
      HINT
      <input type="checkbox">
         <span>
         <code class = "r"> 
            require(chemCal) <br>
            c.a. <- inverse.predict(calcurve, c(0.6214, 0.6431, 0.6055), alpha = 0.05) 
         </code> 
         </span>
      </label>
   </div>

# Comparing Two Methods

# Detecting Outliers

# Limits of Detection

```r
require(instRumental)

form <- Formaldehyde
chemplot(form, xlab = 'Carbohydrate Added (mL)', ylab = expression(OD[660]))
calcurve <- lm(optden ~ carb, data = form)
summary(calcurve)

require(chemCal)
c.a. <- inverse.predict(calcurve, c(0.6214, 0.6431, 0.6055), alpha = 0.05)
c.a.


#######
set.seed(20)

conc <- c(2.5, 6, 10, 20, 30) # ppm
s.stdmeth <- c(10.38, 22.27, 32.14, 66.84, 99.75)
s.newmeth <- stdmeth * runif(5, 1.8, 2.2) + runif(5, 16.1, 16.3)
chemplot(s.stdmeth, s.newmeth, xlim = c(0, 100), ylim = c(0, 300))
fit <- lm(s.newmeth ~ s.stdmeth)
abline(fit)
summary(fit)

chemplot(conc, s.newmeth, xlim = c(0, 100), ylim = c(0, 300))
chemplot(conc, s.stdmeth, xlim = c(0, 100), ylim = c(0, 300))
fit <- lm(s.stdmeth ~ conc)
abline(fit)
summary(fit)

chemplot(conc, s.newmeth, xlim = c(0, 100), ylim = c(0, 300))
fit <- lm(s.newmeth ~ conc)
abline(fit)
summary(fit)
```
