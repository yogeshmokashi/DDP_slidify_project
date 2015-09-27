---
title       : BMI calculator 
subtitle    : Coursera project submission 
author      : Yogesh Mokashi 
job         : R Developer 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [shiny]       # {mathjax, quiz, bootstrap, interactive}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---



## Body Mass Index (BMI) 

Body Mass Index (BMI) is a measure of body fat based on height and weight that applies to adult men and women.  The BMI is an attempt to quantify the amount of tissue mass (muscle, fat, and bone) in an individual, and then categorize that person as underweight, normal weight, overweight, or obese based on that value.

### BMI Categories: 
* Underweight = < 18.5
* Normal weight = 18.5 - 24.9 
* Overweight = 25 - 29.9 
* Obese = BMI of 30 or greater

--- 

## Details of BMI calculator

Shiny app on next page calculates BMI and BMI category.  

Please follow given instructions:

1. Enter your weight and height using standard measures. i.e. weight in lbs; height in feet and inches. 
2. Click "Compute BMI" button. Your BMI and Category will appear as output. 

--- 

## BMI calculator

<div class="row-fluid">
  <div class="col-sm-4">
    <form class="well">
      <div class="form-group shiny-input-container" style="width: 400px;">
        <label for="weight">Body weight (lbs)</label>
        <input id="weight" type="number" class="form-control" value="0"/>
      </div>
      <p> </p>
      <h3>Height (feet, inches): </h3>
      <div class="form-group shiny-input-container" style="width: 100px;">
        <label for="heightfeet">feet</label>
        <input id="heightfeet" type="number" class="form-control" value="0"/>
      </div>
      <div class="form-group shiny-input-container" style="width: 100px;">
        <label for="heightinch">inches</label>
        <input id="heightinch" type="number" class="form-control" value="0"/>
      </div>
      <p> </p>
      <div>
        <button type="submit" class="btn btn-primary" style="width: 150px;">
          <strong>Compute BMI</strong>
        </button>
      </div>
    </form>
  </div>
  <div class="col-sm-8">
    <p> </p>
    <h3>Calculated BMI and Category: </h3>
    <pre id="bmictg" class="shiny-text-output"></pre>
    <span id="bmictg" class="shiny-html-output"></span>
  </div>
</div>

--- 

## Conclusion 

Based on height and weight, one can find out BMI and category (whether normal weight or overweight).  Knowing BMI helps one to take corrective actions like exercise, diet plan etc. 

Thanks for your time! 
