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
- Simulation of the outbreak for a period
    - Use SEIR model
    - Set parameters to reflect the real situation in a region

- Evaluate whether supply and demand meets
    - Draw the curve of severe cases
    - The slower rate of increase, the lower peak value, the better supply and demand meets

### Part II: Optimal Location of the Next Clinic
- Divide the map into grid
- Take advantage of a heat map to show the effectiveness of each cell as the fifth location