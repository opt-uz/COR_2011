Description for files of Calvete, Galé, Oliveros's instances

First block of data is associated to the distribution from depots to retailers. It has been derived
from MDVRP benchmark problems provided by Cordeau et al.
 
This is the description for Files of Cordeau's Instances

The first line contains the following information:

type m n t

where

type   = 0 (VRP) 
    1 (PVRP) 
    2 (MDVRP) 
    3 (SDVRP) 
    4 (VRPTW) 
    5 (PVRPTW) 
    6 (MDVRPTW) 
    7 (SDVRPTW) 
m  = number of vehicles 
n  = number of customers 
t = number of depots (MDVRP) 

The next t lines contain, for each depot the following information:

D Q

where

D   = maximum duration of a route 
Q   = maximum load of a vehicle 

The next lines contain, for each customer, the following information:

i x y d q f a list e l

where

i  = customer number 
x  = x coordinate 
y  = y coordinate 
d  = service duration 
q  = demand 
f  = frequency of visit 
a  = number of possible visit combinations 
list  = list of all possible visit combinations 
e  = beginning of time window (earliest time for start of service), if any 
l  = end of time window (latest time for start of service), if any 

In the case of the MDVRP, the lines go from 1 to n + t and the last t entries correspond to the t depots.


The second block is associated to the production process.

The first line contains the number of production plants (p) and their capacities.

The next p lines contains t+1 values:

j v

where

j= plant number
v= t-vector, upper level objective function coefficient from plant j to depot (1 to t)


The next p lines contains t+1 values:

j w

where

j= plant number
w= t-vector, lower level objective function coefficient from plant j to depot (1 to t)

