# Ebony Soap Inventory Management Simulation

## Introduction
This simulation project models the inventory management strategy of Ebony, a prominent manufacturer of bath soap, with the goal of controlling inventory costs. By evaluating the effectiveness of a specified production policy over a 52-week period with multiple replications, this model aids management decisions by providing insights into inventory-related costs and production adjustments.

## Project Context
Ebony faces the challenge of optimizing weekly production levels to balance inventory costs against the risk of stockouts, where unmet demand results in lost sales. This simulation assesses the cost implications of maintaining production levels based on current inventory, using historical demand data to model future scenarios.

## Data Overview
- Historical weekly demand data for soap, indicating a normal distribution with a mean demand of 118.932692 units and a standard deviation of 14.229077 units.
- Inventory holding cost: $30 per unit per week (1 unit = 1000 cases of soap).
- Production levels: 110, 120, or 130 units per week with a $3000 cost for changing production levels.
- Current inventory: 60 units; last week's production: 120 units.

## Production Policy
- Thresholds: Produce 130 units if inventory < 30 units; Produce 110 units if inventory > 80 units; Otherwise, continue at the previous week's production level.

## Simulation Model
The simulation runs for 52 weeks with 1000 replications to provide a robust estimation of expected costs and credible intervals.

## Random Variables
- Weekly Demand _x_: Modeled as a random variable with distribution parameters derived from historical data.

## Objective
The aim is to determine the expected cost and the 95% credible interval for each upper threshold value _U_ for inventory, ranging from 30 to 80 in increments of 10.

## Alternative Production Policies
Additional policies for Ebony to consider include dynamic threshold adjustments, stochastic demand forecasting, adaptive production levels, alternative cost structures, and policies to manage excess demand.

## Implementation Details
The implementation is provided in a Python Jupyter Notebook file (Assign_3a_(EBONY) (1) (1).ipynb), demonstrating the simulation model and results analysis.

## Expected Results and Analysis
The simulation results include the expected cost and credible intervals for each production level, which will guide Ebony in optimizing their production strategy to minimize costs while meeting demand.

## Conclusion
The simulation findings will inform Ebony's management about the most cost-efficient inventory level to maintain, considering the trade-offs between holding costs and lost sales due to stockouts.

