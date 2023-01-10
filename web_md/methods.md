---
title: Methods
date: 2023-01-08 14:50:58
tags: 
- Methods
- categories: 
- Methods
---

## Method
1. Simulation of coronavirus outbreak: SEIR model (sample code + pic)
    - The population can be divided into four compartments:   
      - Susceptible (those who can catch the disease)
      - Exposed (those who are exposed to the disease but don’t have symptoms yet)
      - Infected (those who show symptoms and are infective)
      - Recovered (those who have recovered and become immune).
    - The model takes into account following factors, which is reflected in initially set parameters.
      - the transition rate between Susceptible and Exposed
      - the transition rate between Infected and Recovered
      - an incubation period, during which those who are exposed are not infective
      - outbreak starts from an initial 10 infected cases
      - the pattern of movement between zones within the region in a typical day
    - The relationship between Susceptible, Exposed, Infected, Recovered is reflected in differential equations.
      $Susceptible \rightarrow Exposed \rightarrow Infected \rightarrow Recovered$
      - $dS \over dT$
      - eq2
      - eq3
      - eq4

2. Evaluate whether supply and demand meets
   - Draw the curve of infected cases with in the region. The seriousness is defined as the peak value divided by the time of reaching the peak.
      - pic1
3. Decide the location of the fifth clinic based on current simulation
   - Use a mathematical formula to determine the effectiveness of a new location. The lower the value is, the better the location will be.
     - $Effectiveness=\sum_{i=0}^n w_0((x - x_0)^2 + (y - y_0)^2)$
   - Divide the map into grid and calculate the effectiveness for each cell
   - Display the effectiveness in the form of heatmap, which will indicate the optimal location
