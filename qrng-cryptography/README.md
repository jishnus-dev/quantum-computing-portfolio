# Quantum Random Number Generation (QRNG) for Cryptographic Key Distribution

## 🔬 Project Overview
This project leverages the probabilistic nature of quantum mechanics to build a Quantum Random Number Generator (QRNG) utilizing single-qubit measurements in superposition states. The objective is to demonstrate information-theoretic cybersecurity over the deterministic vulnerabilities inherent in classical Pseudo-Random Number Generators (PRNGs).

## 🛠️ Methodology
- Superposition: A Hadamard gate is applied to a qubit initialized in the ground state to create an equal superposition.

- Quantum Measurement: A projection operator collapses the state, yielding fundamentally unpredictable outcomes governed by the Born rule.

- Execution: The circuit was simulated over multiple shots using the StatevectorSampler to extract a raw bitstring for entropy analysis.

## 📊 Key Results
- The QRNG produced a nearly uniform distribution of zeros and ones, resulting in an empirical Shannon entropy that closely matches the theoretical maximum limit.

- The extracted quantum key was evaluated against a classical PCG64 PRNG.

- While statistical distributions were similar, the QRNG guarantees superior cryptographic security as it lacks a deterministic seed, making it immune to reverse-engineering attacks