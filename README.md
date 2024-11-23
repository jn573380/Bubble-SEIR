This repository contains two R scripts to simulate an epidemic using a stochastic Bubbled SEIR model.
The function Bubbled_SEIR implements a stochastic SEIR model with Bubble Strategies.
The function organized_data simulates multiple epidemics and processes the result. It converts simulation results into daily statistics for comparison and records final size and duration for each epidemic.

Here is how to run the simulation for 1000 iterations with 5 bubbles:
results <- organized_data(k = 5, beta = 1.32, kappa = 0.25, gamma = 1/1.61, r = 0.01, S0 = 19, E0 = 0, I0 = 1, R0 = 0, N = 100, Nsim = 1000)

Modify parameters such as: 
k: Number of bubbles;
beta: Infection rate;
kappa: Latency rate;
gamma: Recovery rate;
r: Movement rate;
S0, E0, I0, R0: Initial compartment sizes within each bubble.
