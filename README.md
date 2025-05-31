Zombie Outbreak Simulation: Cellular Automata & PDE Solver
A computational physics project implementing zombie outbreak dynamics through cellular automata and partial differential equations, showcasing advanced numerical methods and visualization techniques.
🧟‍♂️ Project Overview
This project implements the zombie outbreak model from the famous "When Zombies Attack!" paper by Munz et al., extending it from a simple ODE system to a sophisticated spatial cellular automaton simulation. The implementation demonstrates the evolution from theoretical mathematical models to practical computational physics applications.
Mathematical Foundation
The project is based on the SIZR (Susceptible-Infected-Zombie-Removed) epidemiological model:
dS/dt = Π - βSZ - δS
dI/dt = βSZ - ρI - δI  
dZ/dt = ρI + ζR - αSZ
dR/dt = δS + δI + αSZ - ζR
Where:

S: Susceptible population
I: Infected population
Z: Zombie population
R: Removed population
β: Transmission rate
ρ: Zombification rate
α: Zombie destruction rate
ζ: Resurrection rate
δ: Natural death rate
Π: Birth rate

Computational Physics Connection
This project showcases several advanced computational physics techniques:
1. Spatial Discretization & Cellular Automata

Transformed the original ODE system into a 2D spatial grid-based cellular automaton
Implemented Moore neighborhood interactions for realistic spatial propagation
Developed efficient state transition algorithms with probabilistic rules

2. Multi-Scale Modeling

Single City Simulation: High-resolution local dynamics
Multi-City Network: Large-scale regional outbreak modeling with intercity migration
Heterogeneous parameter distributions across different urban environments

3. Numerical Optimization

JIT Compilation: Used Numba for 10x+ performance improvements
Vectorized Operations: Leveraged NumPy for efficient array computations
Memory-Efficient Storage: Sparse frame saving for large-scale simulations
