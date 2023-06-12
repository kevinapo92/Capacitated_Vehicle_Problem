# Capacitated_Vehicle_Problem

## Introduction

This repository provides an implementation of a capacitated Vehicle Routing Problem (VRP) solver. The VRP is a well-known optimization problem that involves finding the optimal set of routes for a fleet of vehicles to pick up and deliver goods to a given set of customers. In this particular implementation, we focus on the capacitated VRP, where each vehicle has a limited carrying capacity.

The solver is designed to minimize the total distance traveled by the vehicles while satisfying the demand of each customer. We calculate distances between locations (nodes) using the Manhattan distance metric. The problem is formulated as an Integer Programming (IP) problem, with the VRP generalizing the famous Traveling Salesman Problem (TSP), which is a VRP with a single vehicle.

**Features** 
* Support for up to 16 customers and 4 vehicles starting from the depot node.
* Each vehicle has a capacity of 15 units for carrying goods.
* Input file provides the coordinates of the depot and customers, along with their respective demands.

## Formulation 
A two index formulation was used to solve the problme, a binary decision variable xij asumes the value 1 if and only if there is a route that goes from customers i to j directly, with these parameters and decision variables the two-index flow formulation of the CVRP if given by:

![image](https://github.com/kevinapo92/Capacitated_Vehicle_Problem/assets/96119396/5a59b2d3-9a75-4ea2-9881-796209470583)


## Technologies Used
* Solve the capacitated VRP using the Cplex and Pandas libraries for optimization.
* Utilize the SciPy library for additional functionality.
* Python
* Jupyter Notebook

## Data
[CVRP_Data](https://github.com/kevinapo92/Capacitated_Vehicle_Problem/blob/main/CVRP_input.xlsx)

## Analysis and Results
[CVRP_two_index](https://github.com/kevinapo92/Capacitated_Vehicle_Problem/blob/main/CVRP%20model.ipynb)



