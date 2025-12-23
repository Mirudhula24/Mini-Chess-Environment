# Mini-Chess-Environment
Project Overview

This project implements a Dynamic Programming–based Reinforcement Learning solution for a simplified 4×4 Mini-Chess environment.
The environment is modeled as a Markov Decision Process (MDP) where an agent (White) must optimally promote a pawn while avoiding capture by an opponent (Black King).

## Objectives

Model a real-world sequential decision problem as an MDP
Implement Value Iteration to compute optimal state values
Implement Policy Iteration to derive an optimal policy
Simulate agent behavior using the learned value function
Visualize optimal state values using a heatmap

## Environment Description

Board Size: 4×4 (as per assignment requirement)

Agents:

White: King + Pawn (learning agent)
Black: King (adversary)

State Representation:
(White King Position, White Pawn Position, Black King Position, Turn)

Actions:

White: Move King or Pawn
Black: Move King

Rewards:

+10 for Pawn promotion
−10 for Pawn capture
0 for intermediate states

## Algorithms Implemented

Value Iteration
Iteratively updates state values until convergence
Policy Iteration
Alternates between policy evaluation and improvement
Both algorithms compute optimal strategies under deterministic transitions.

## Visualization

A heatmap is generated to visualize the optimal value function V*(s)
The visualization shows how White King positions affect expected rewards when Pawn and Black King positions are fixed

## How to Run

Open the provided Jupyter Notebook
Run all cells sequentially

Observe:

State space size
Convergence of Value Iteration
Policy Iteration output
Board simulation
Value function heatmap

## Libraries Used

NumPy
Matplotlib
itertools
(No high-level RL or ML libraries are used, as per assignment constraints.)

## Conclusion

This project demonstrates how optimal decision-making can be achieved using planning-based Reinforcement Learning techniques without relying on data-driven learning.
It highlights the effectiveness of Dynamic Programming methods for small, fully known environments.

