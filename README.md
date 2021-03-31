# gerrymander-sims
## A set of simulations for teaching and learning some of the data science of gerrymandering

As a first goal, we want to be able to simulate the following

+ Brute force search for districts in toy model (rectangular map, start with 5x5)
+ + Using rejection sampling of units
+ + Starting from canonical case (stripes) and using single swaps across neighboring boundaries, followed by rejection if necessary
+ For both algorithms, store districts as a list 
+ + Either using coordinates of all units, 
+ + + E.g. one district = [x1y1 x2y2 x3y3 x4y4 x5y5] =  [11,12,13,14,15]
+ + + Where xiyi are coordinates on the map
+ + Or using shapefile standard (which I’ve never used generatively, but obviously would be cool and generalizable beyond square grids)
+ For both algorithms, 
+ + Keep track of rejection rate
+ + Keep track of number of new districts discovered as a function of non-rejected iteration (so we’re distinguishing rejection of illegal district from discovery of an already known district)
+ Visualize?
