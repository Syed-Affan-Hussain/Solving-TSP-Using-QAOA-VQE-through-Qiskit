# Solving-TSP-Using-QAOA-VQE-through-Qiskit
This repository provides an implementation of solving the Traveling Salesman Problem (TSP) using the Quantum Approximate Optimization Algorithm (QAOA) and the Variational Quantum Eigensolver (VQE) through Qiskit.  

This code implements the solution to the Traveling Salesman Problem (TSP) using the Quantum Approximate Optimization Algorithm (QAOA) and the Variational Quantum Eigensolver (VQE) through Qiskit.

## Note

Please run this code on IBM Quantum LAB.

## Issue on GitHub

There are errors in the results, likely due to compatibility issues between Qiskit QAOA and the TSP function. I have submitted an issue on GitHub to address this problem.

## Graph Visualization

The `draw_graph` function is used to visualize the TSP graph.

## TSP Solution Visualization

The `draw_tsp_solution` function is used to visualize the solution to the TSP problem. It takes the TSP graph, the order of cities in the solution, colors, and positions of nodes as inputs.

## Generating TSP Instance

A TSP instance with `n` cities is randomly generated.

## Creating TSP Hamiltonian

A random TSP Hamiltonian is created by converting the TSP instance to a quadratic program and then to a QUBO.

## Solving the Problem with QAOA

The TSP problem is solved using the QAOA algorithm. The QAOA object is instantiated with a sampler and an optimizer. The `compute_minimum_eigenvalue` method is used to find the minimum eigenvalue.

## Results

The results of the QAOA computation are printed, including the lowest energy value, the TSP objective value, the execution time, the best sample, and the solution. The solution objective value is also computed.

## Solving the Problem with VQE

The TSP problem is also solved using the VQE algorithm. The VQE object is instantiated with a sampler, an ansatz, and an optimizer. The `compute_minimum_eigenvalue` method is used to find the minimum eigenvalue.

## Results

The results of the VQE computation are printed, including the lowest energy value, the execution time, the feasibility of the solution, the solution, and the solution objective value.

## TSP Solution Visualization

The `draw_tsp_solution` function is used to visualize the solution to the TSP problem obtained from VQE.

