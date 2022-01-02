# Logical-Classical-Planning-Agents

Note: Code is kept private. Attributed to UC Berkeley (http://ai.berkeley.edu)

This project implements 2 frameworks:
1. Pacman agent logically plans its way to goal

Given Pacman's position represented as (x,y), a time t, and positions of walls, a successor state axiom is returned for Pacman's position being (x,y) at time t.    This is the conjunction of Pacman being in an adjacent square at time t-1 and Pacman moving to (x,y) at time t-1. At each time step, expressions that represent the Pacman game logic are created. A model that satisfies the logical expression is then found, and this represents the sequence of actions that take Pacman to the goal state.
  
2. Pacman agent uses GraphPlan to find its way to the goal.

Unlike logic-based planning, there is no explicit representation of time. Instead, propositions are added and deleted in the state to enumerate the possible state propositions at each level of the planning graph and those levels represent time. The algorithm then searches for the first level when all goal propositions are present and not mutually exclusive.
