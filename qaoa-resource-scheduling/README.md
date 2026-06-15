# Optimizing Simple Scheduling Problems with QAOA

## 🔬 Project Overview
This project implements the Quantum Approximate Optimization Algorithm (QAOA) to solve a combinatorial resource allocation problem. The scenario models the assignment of discrete tasks to workers to ensure a perfectly balanced workload without violating physical constraints.

## 🛠️ Methodology
- QUBO Formulation: The scheduling problem was mathematically defined as a Quadratic Unconstrained Binary Optimization (QUBO) model.

- Constraint Handling: A penalty multiplier was introduced to heavily penalize invalid quantum states (e.g., assigning one task to multiple workers), steering the optimizer toward valid assignments.

- Ansatz Depth Study: The QAOA circuit was executed and analyzed across multiple variational layers to evaluate expressibility and convergence behavior.

## 📊 Key Results
- The quantum algorithm successfully navigated the expanded Hilbert space to isolate the valid physical configurations.

- The deepest ansatz successfully achieved the exact theoretical minimum cost, discovering the perfectly balanced task assignment.

- This implementation proves the theoretical mechanics required to map human constraints into an Ising Hamiltonian for scaling to complex IT and logistics networks.