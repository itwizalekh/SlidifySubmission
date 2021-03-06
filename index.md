---
title       : BMI Calculator on ShinyApps
subtitle    : Coursera Submission for "Developing Data Products"
author      : Alekh Jain
job         : Data Warehousing Consultant
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## About the BMI calculator

- This **BMI calculator** is a simple *ShinyApp*.    
- It can be used to calculate BMI in **two simple steps**.  
- The application is **reactive**, so it updates the BMI result as you type-in the inputs.  
- This application uses **Standard** units.  
- Later slides will cover **unit conversions** if you have inputs in metric units.  
- Key features of the application:
  - Simple and elegant
  - Fast
  - Light-weight
  - No advertisements
  - Hosted by Shinyapps.io  

--- .class #id 

## Calculate your BMI in two simple steps

- Step 1: Input your <b>Height</b> in Inches  
- Step 2: Input your <b>Weight</b> in Pounds  
<br>
<u>Note:</u> 
- Decimal values for weight / height are also accepted  
- You can use arrow buttons to increment / decrement values  
- Alternatively, you may type in the values manually  
- When using the up button you may only go to next nearest whole number  
- When using the down button you may only go to next nearest whole number  
- If you know values in metric units, see subsequent slides for help  

--- .class #id 

## An example

Lets see it in action:



```r
height <- 72  # height in inches
weight <- 172  # weight in pounds

BMI <- computeBMI(72, 172)
```

<p></p>
The BMI for a person *72 inches tall* and *172 pounds heavy*: **23.3248**

--- .class #id 

## Conversion from Metric to Standard units

### Conversion from centimeters to Inches

Divide value in centimeters with 2.54 to get value in inches.  
<p></p>
<u>Example:</u>  
Let, Height in centimeters = 180 cms  
Then, Height in inches would be = 70.8661 inches

### Conversion from Kilograms to Pounds

Multiply value in Kilograms with 2.20462 to get value in pounds.  
<p></p>
<u>Example:</u>  
Let, Weight in Kilograms = 78 kgs  
Then, Weight in pounds would be = 171.9604 pounds

