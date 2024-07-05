# Shortest path algorithms in graphs
A simple code to find shortest paths in graphs using some algorithms.

Graph Algorithms Implementation
This repository contains a C program that allows the user to work with graph representations and execute various graph algorithms through a command-line interface. The supported algorithms include Floyd-Warshall, Bellman-Ford, and Dijkstra's algorithm. The program allows for initialization and manipulation of an adjacency matrix representation of a graph.

# Features

Initialize Matrix: Set the order of the adjacency matrix.
Print Matrix: Display the current state of the adjacency matrix.
Insert Value in Matrix: Add or update a non-negative value in the matrix at a specified position.
Insert Negative Value in Matrix: Add or update a negative value in the matrix at a specified position.
Insert Predefined Values in Matrix: Fill the matrix with a set of predefined values for testing purposes.
Traverse Matrix: Perform a depth-first traversal of the graph from a given origin to a destination.
Floyd-Warshall Algorithm: Compute the shortest paths between all pairs of vertices.
Bellman-Ford Algorithm: Compute the shortest paths from a given source vertex, handling negative weights and detecting negative cycles.
Dijkstra's Algorithm: Compute the shortest paths from a given source vertex, assuming all edge weights are non-negative.
Exit Program: Terminate the program.

# Usage
Upon running the program, the user is presented with a menu to choose from the above-listed features. The adjacency matrix can be manipulated and analyzed using the provided options.

# Example

To compile and run the program, use a C compiler such as gcc:

sh

gcc -o graph_algorithms graph_algorithms.c
./graph_algorithms

Follow the on-screen instructions to interact with the program.

# Implementation Details

The adjacency matrix is represented by a 2D array matriz[101][101], with support for matrices up to 100x100.
The Menu function handles user input and displays the available options.
Various utility functions are implemented for matrix manipulation and graph traversal.
Each graph algorithm function (Floyd-Warshall, Bellman-Ford, Dijkstra) includes checks for appropriate conditions (e.g., non-negative weights for Dijkstra).
The program supports detecting and handling negative cycles using the Bellman-Ford algorithm.

# Notes

Ensure that the input for the matrix dimensions does not exceed 100.
The adjacency matrix is initialized with zeroes, and diagonal elements (self-loops) are ignored during insertion.
For convenience, the predefined matrix values can be used to quickly test the graph algorithms.
