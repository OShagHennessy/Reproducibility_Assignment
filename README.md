 # Reproducibility_Assignment
This is the term assignment for the Artificial Intelligence (COMS7044A) module. We were tasked to reproduce the results of the paper: "Utilising Uncertainty for Efficient Learning of Likely-Admissible Heuristics".

# 15-Puzzle Solver using NN-WUNN Heuristic

This repository contains code for solving the 15-Puzzle problem using the Neural Network Weighted Upperbound Nearest Neighbor (NN-WUNN) heuristic combined with the Iterative Deepening A* (IDA*) search algorithm.

## How this works
A flow chart depicting the process.
```mermaid
graph LR;

FirstBlock["`**Set-Up**
15-PuzzleEnvironment
Search Algorithm (IDA*)`"]
Algorithm3["`GenerateTaskPrac`"]
Algorithm4["`LearnHeuristicPrac`"]
TrainingofNNs["`Training of NNs`"]
KorTasks["KorTasks"]
Output["Output"]

Algorithm3 --> Algorithm4 --NNs are trained simultaneously--> TrainingofNNs --> KorTasks --> Algorithm4 --> Output

subgraph **Set Up**
15-PuzzleEnvironment --> Neural Networks --> Search Algorithm (IDA*)
end
```
## Prerequisites

Before running the solver, ensure you have the following prerequisites installed:
- Python 3
- pip (Python package manager)
- NumPy
- TensorFlow
- scikit-learn
- scipy

## Overview

The 15-Puzzle problem is a classic sliding puzzle game where 15 tiles numbered from 1 to 15 are placed in a 4x4 grid with one empty space. The goal is to rearrange the tiles by sliding them into the empty space to achieve a specified goal configuration.

In this project, we employ the NN-WUNN heuristic, a neural network-based approach, to estimate the distance between a given state and the goal state. This heuristic guides the IDA* search algorithm to efficiently explore the state space and find optimal or near-optimal solutions.

## Setup and Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/OShagHennessy/Reproducibility_Assignment.git
   
## Contribution by
Lebohang Mosia
