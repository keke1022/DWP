---
title: Abstract
date: 2023-01-08 14:39:50
tags: 
- Problems
categories: 
- Problems
---

## Purpose
Explore the rationality of the supply and demand of medical resources in fever clinic in Jinshan Street in Fuzhou and then determine the next location of a clinic.

## Description
The covid-19 virus is getting serious at present. It is obvious that the medical resource could not meet with the increasing need. Therefore, we aim to explore how to distribute medical resource to ensure the health of the population in Jinshan Street to the greatest extent possible. In our project, medical resource is reflected in fever clinics. The overall health condition is evaluated by local severe cases.

## Data needed
- Addresses of communities in Jinshan Street 
- Population of communities in Jinshan Street 
- Scale of fever clinics in Jinshan Street


## Steps
### Part I: Supply and Demand Evaluation
- Simulation of three months
    - Total infection cases follow the S-curve
    - A certain percentage of infected patients are severely ill
    - Patients of different communities will only go to a particular clinic
    - Severe cases are considered to have recovered after they go to clinic
     

- Evaluate whether supply and demand meets
    - Draw the curve of severe cases
    - The slower rate of increase, the lower peak value, the better supply and demand meets

### Part II: Optimal Location of the Next Clinic
- Use a mathematical formula to determine the effectiveness of a new location. The lower the value is, the better the location will be.
  - $Effectiveness=\sum_{i=0}^n w_0((x - x_0)^2 + (y - y_0)^2)$
- Divide the map into grid and calculate the effectiveness for each cell
- Display the effectiveness in the form of heatmap, which will  indicate the optimal location