# CI2024_lab2
Second lab of the Computational Intelligence 2024 course. 
The goal of this lab is to implement a solution to the Traveling Salesman Problem (TSP) using a fast and approximate approach and a slow and exact approach.

## Greedy Solution

The greedy solution is based on the 2-opt algorithm. The algorithm starts by a NN (Nearest Neighbor) algorithm to generate a initial solution. Then, it iteratively tries to improve the solution by swapping two edges and checking if the new solution is better than the previous one. The algorithm stops when no improvement is found.

In the notebook `tsp_greedy.ipynb` you can find the implementation of the greedy solution as well as the tests and results.

## Evolutionary Algorithm Solution

For the EA solution I tried different configurations. Overall the EA characteristics are the following:

* Hyper-modern GA flow
* Representation: one-time items
* Parent selection: tournament selection
* Crossover: inver-over
* Mutation: can be chosen between insert mutation and inversion mutation
* Population model: can be chosen between generational and steady-state

In the notebook `tsp_ea.ipynb` you can find the implementation of the greedy solution as well as the tests and results.

## Results

Overall the greedy solution is faster and gives a good approximation of the optimal solution. The EA solution is slower but can give better results for the problems by tweaking the parameters. 

## Credits

* Thanks to [Daniel Bologna (s310582)](https://github.com/AbstractBorderStudio) who worked with me in the implementation of the EA solution and gave me the idea of using the inversion mutation.
* My work is based on the code provided by the professor Giovanni Squillero in the course.
* Here some resources that helped me come up with the greedy solution and with the visualization of the results:
    * https://en.wikipedia.org/wiki/2-opt
    * https://youtu.be/NG9CcLk7xNs?si=Iz7crSLu5yML1Nqz
    * https://networkx.org/documentation/stable/auto_examples/index.html
