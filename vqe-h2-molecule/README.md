# Hybrid Quantum-Classical VQE for Molecule Energy Estimation

## 🔬 Project Overview
This project implements a Variational Quantum Eigensolver (VQE) to estimate the ground state energy of the hydrogen molecule (H2). This implementation combines a parameterized quantum circuit to prepare trial molecular states with a classical optimizer that iteratively minimizes the measured energy.

## 🛠️ Methodology
- Hamiltonian Mapping: The electronic structure of the molecule was transformed into qubit operators using the Jordan-Wigner mapping technique.

- Quantum Ansatz: A hardware-efficient TwoLocal ansatz was utilized, incorporating RY and RZ rotation gates alongside linear CX entanglement to ensure a shallow circuit depth suitable for NISQ devices.

- Classical Optimization: The COBYLA optimizer was selected for parameter updates due to its stable convergence with small VQE systems.

## 📊 Key Results
- The exact classical ground state energy was calculated to establish a comparative baseline.

- The VQE algorithm successfully converged to an estimated total energy, resulting in a highly accurate energy error margin when compared to the exact solver.

- Runtime execution on the Statevector simulator completed efficiently, validating the hybrid quantum-classical feedback loop.