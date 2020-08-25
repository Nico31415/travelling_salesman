# travelling_salesman

Implementation of different algorithms used to solve the Travelling Salesman Problem (PST).

The TSP asks the following question: "Given a list of cities and the distances between each pair of cities, what is the shortest possible route that visits each city exactly once and returns to the origin city?" 

The most intuitive solution would be to check every possible path. However, this takes O(n!) time.

Another algorithm that comes to mind is the Nearest Neighbour (NN), which each city to its closest neighbour. This sounds like a good idea but can be catastrophic if you have to reach to a really far away city at the end of the path.

Here is an example of why the NN can go wrong. 
