# travelling_salesman

Implementation of different algorithms used to solve the Travelling Salesman Problem (PST).

The TSP asks the following question: "Given a list of cities and the distances between each pair of cities, what is the shortest possible route that visits each city exactly once and returns to the origin city?" 

The most intuitive solution would be to check every possible path. However, this takes O(n!) time.

Another algorithm that comes to mind is the Nearest Neighbour (NN), which each city to its closest neighbour. This sounds like a good idea but can be catastrophic if you have to reach to a really far away city at the end of the path.

Here is an example of why the NN can go wrong. 

![nearest_neighbour](https://user-images.githubusercontent.com/20355467/91210591-64c97b00-e705-11ea-81bf-6d461f22a7ed.png)
![held_karp](https://user-images.githubusercontent.com/20355467/91210698-8591d080-e705-11ea-93ba-9a087eeb2b41.png)

One of the open problems in Computer Science is to find an algorithm for TSP with polynomial time. Using dinamic programming and memoisation, The Held-Karp algorithm does much better than brute force, with O(2^n*n^2), but not quite as good as polinomial time.

This is a logarithmic graph comparing the times for Brute Force (blue) and Held Karp (orange)

![TSP](https://user-images.githubusercontent.com/20355467/91210969-ec16ee80-e705-11ea-8382-2f28c1d30ffe.png)

To learn more about this problem, please see:

https://en.wikipedia.org/wiki/Travelling_salesman_problem
https://medium.com/basecs/speeding-up-the-traveling-salesman-using-dynamic-programming-b76d7552e8dd
