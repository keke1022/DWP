---
title: Discussion
date: 2023-01-08 14:52:40
tags: discussion
categories: discussion
---

## Discussion
1. Simulation:
   
Due to a lack of data, many assumptions are made, which may not be consistent with the real situation here. This will cause errors. However, those missing information can be acquired somehow for better simulation.
#### Assumptions:
- The pattern of movement between zones within the region in a typical day is randomized
  - Solution: the exchange of population between zones can be obtained by phone data like public transportation usage
- The transition rate between Infected and Recovered is the same for all regions
  - Solution: count the average recovering time for each region, which is related to population structure and clinics scale, etc.

2. Evaluate Supply and Demand relation

Currently, we use the formula peak value for infected cases divided by the time to peak to reflect the seriousness of outbreak in a region. However, we should also take into account factors such as the proportion of severe disease and the extent of economic damage. For example, communities with a large proportion of elderly people should be given priority.

3. Select the location for the fifth clinic

We design the effectiveness of a new location as a formula. $cost=\sum_{i=0}^n w_0((x - x_0)^2 + (y - y_0)^2)$ $w_0$ reflects the seriousness of the outbreak in the community. For the convenience, the clinic should be built nearer to area with serious situation. We aim to minimize the cost value in order to select the optimal location. There is still some room for improvement.
- We divide the Jinshan Street into $n=21$ communities, and treat them as a point with correspoinding population for the sake of convenience. However, a community consists of many residential quarters, and each residential quarter has many buildings. This method can be optimized given real population data of Jinshan Street. In this way, we could treat people in the same building as a whole and build more complex but accurate models 
- The distance between the new clinic and communities are all straight-line distance. However, we should consider public transport development and road condition. For future research, we may take advantage of map software to calculate the real distance.
  
