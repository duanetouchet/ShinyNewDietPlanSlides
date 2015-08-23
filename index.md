---
title       : Shiny New Diet Plan
subtitle    : How to lose weight and reach your goal
author      : Duane Touchet
job         : Student in Developing Data Products MOOC from Johns Hopskins
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Shiny New Diet Plan

Many Americans and some other country's citizens need to lose weight.
We turn to online tools to do so, but how good are they?
This presentation will explain why you should use the Shiny New Diet Plan
instead of the other diet plans out there!

--- 

## Diet and Weight Loss

Recent studies have implied that dieting is 80% of weight loss and exercise is the other 20%.
So for efficiency, we should focus mostly on changing our diet to lose weight.
Although there is some variability, the main way to loose weight is to:

Burn more calories than you Consume

Of course, the calculation that the app will give is a general rule. If you exercise at different intensities over time, this will affect your weight loss. If you try to lose too much weight too fast, you may have health problems.

--- 

## How many calories do we burn? 1 - BMR

How many calories you burn in a day is composed of two numbers.
The first is Basal Metabolic Rate (aka BMR) which comprised how much energy your
body needs to keep itself running. The BMR has a different formula for males and females.
Consider the example with two people, 1 female, 1 male, with the same weight, height, and age.



```r
weight <- 150
height <- 66
age <- 30

maleBMR <- 66 + ( 6.23 * weight ) + ( 12.7 * height ) - ( 6.8 * age )

femaleBMR <- 655 + ( 4.35 * weight ) + ( 4.7 * height ) - ( 4.7 * age )
```

---

## How many calories do we burn? 2 - Activity Level

After figuring out your BMR, your activity level will give a factor to estimate how many more calories you need so your weight loss is consistent. Yo-yo dieting is prone to failure so if you want to lose 10 pounds they should be shed slowly and evenly.

Total calories needed for statis (static weight) is BMR * ActivityLevelFactor.

To lose weight, simply eat less than that number.

---

## What makes Shiny New Diet Plan different?

What's different about the Shiny New Diet Plan is that it re-calcuates weight, BMR, and calories needed each week.

After 5 weeks, you may lose 7.5 pounds so your BMR will be different and your calories needed to keep losing weight will change.

Shiny New Diet Plan will adjust your calories needed as you lose weight so you don't plateau before your goal is achieved.

---



