# Matlab Learning and AI

## Getting started

To define a matrix:

```matlab
A = [1, 2, 3; 4, 5, 6, 7, 8, 9]
```

To stagger matrix:

```matlab
rref(A)
```

# Custom Data Type Optimization Using the Genetic Algorithm

This example shows how to use the genetic algorithm to minimize a function using a custom data type. The genetic algorithm is customized to solve the traveling salesman problem.

### Traveling Salesman Problem

The traveling salesman problem is an optimization problem where there is a finite number of cities, and the cost of travel between each city is known. The goal is to find an ordered set of all the cities for the salesman to visit such that the cost is minimized. To solve the traveling salesman problem, we need a list of city locations and distances, or cost, between each of them.

Our salesman is visiting cities in the United States. The file usborder.mat contains a map of the United States in the variables x and y, and a geometrically simplified version of the same map in the variables xx and yy.

```matlab
load('usborder.mat','x','y','xx','yy');
plot(x,y,'Color','red'); hold on;
```

<img src="https://github.com/RonnyldoSilva/Matlab-Learning/blob/master/Images/traveling_salesman_demo_01.png">
