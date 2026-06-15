# Secure Message Transmission with Superdense Coding

## 🔬 Project Overview
This project implements the quantum superdense coding protocol, allowing the transmission of two classical bits of information between a sender (Alice) and a receiver (Bob) through the physical transmission of only a single qubit. This demonstrates how quantum entanglement enables data compression ratios impossible in classical IT infrastructure.

## 🛠️ Methodology
- Entanglement: A maximally entangled Bell state is generated and shared between Alice and Bob using a Hadamard and a CNOT gate.

- Encoding: Alice applies specific local Pauli operations to her qubit depending on the 2-bit message ($I$ for '00', $X$ for '01', $Z$ for '10', and $ZX$ for '11').

- Decoding: Bob receives Alice's qubit and applies a CNOT gate followed by a Hadamard gate to reverse the entanglement and safely extract the classical bits via measurement.

## 📊 Key Results
- The superdense coding protocol achieved a fully deterministic success probability across all possible target messages.

- The protocol successfully doubled the effective channel capacity limit (transmitting 2 bits of information per 1 transmitted qubit), validating the theoretical advantage of quantum data compression.