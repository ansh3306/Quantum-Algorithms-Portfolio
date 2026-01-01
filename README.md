# Quantum Algorithms & Simulation Portfolio

**Author:** Ansh Droch
**Affiliation:** National Institute of Science Education and Research (NISER)
**Standing:** DISHA Scholar, Integrated M.Sc. in Mathematics (Minor in CS)
**Contact:** ansh.droch@niser.ac.in

## 🚀 Overview
This repository contains implementations of quantum algorithms and simulations using **Qiskit**, focusing on Quantum Walks, Variational Algorithms (VQE), and Error Correction. These projects demonstrate a bridge between abstract mathematical theory (Group Theory, Linear Algebra) and practical implementation on NISQ devices.

---

## 🔹 Module 1: Quantum Walks (Dynamics & Noise)
*Focus: Simulating coherent quantum transport and analyzing environmental effects.*

### 1. Discrete-Time Quantum Walk (DTQW)
📄 **File:** `Qiskit_Discrete_Time_Quantum_Walk.ipynb`
- **Objective:** Simulate a coined quantum walk on a cycle graph.
- **Key Implementation:**
  - Constructed the **Shift** and **Coin** (Hadamard/Grover) operators.
  - Demonstrated **ballistic spreading** ($\sigma^2 \propto t^2$) compared to classical diffusive random walks ($\sigma^2 \propto t$).
  - Visualized probability distributions showing constructive/destructive interference peaks.

### 2. Noisy Quantum Walk & Error Mitigation
📄 **File:** `Quantum Walk with Noise & Error Mitigation.ipynb`
- **Objective:** Analyze the fragility of quantum interference under realistic hardware noise.
- **Key Implementation:**
  - Applied custom **Noise Models** (Depolarizing and Thermal Relaxation channels) to the walk circuit.
  - Quantified the transition from quantum ballistic spread to classical-like diffusion due to decoherence.
  - Implemented error mitigation strategies to recover signal fidelity.

---

## 🔹 Module 2: Variational Quantum Algorithms (VQE)
*Focus: Hybrid quantum-classical optimization for Hamiltonian simulation.*

### 3. VQE for Molecular Ground State ($H_2$)
📄 **File:** `Variational Quantum Eigensolver (VQE) for H₂ipynb`
- **Objective:** Calculate the ground state energy of the Hydrogen molecule.
- **Key Implementation:**
  - Mapped the fermionic Hamiltonian to qubits using **Parity/Jordan-Wigner mapping**.
  - Utilized a hardware-efficient ansatz (`EfficientSU2`) and classical optimizers (COBYLA/SPSA).
  - Achieved **chemical accuracy** consistent with Full Configuration Interaction (FCI) benchmarks.

---

## 🔹 Module 3: Quantum Information & Error Correction
*Focus: Fundamental tests of quantum mechanics and preserving quantum states.*

### 4. Quantum Error Correction (3-Qubit Bit Flip Code)
📄 **File:** `3-Qubit Bit Flip Code.ipynb`
- **Objective:** Protect a logical qubit against $X$-error (bit-flip) noise.
- **Key Implementation:**
  - Designed the encoding circuit using entangled ancilla qubits.
  - Implemented **Syndrome Measurement** to detect errors without collapsing the logical state.
  - Demonstrated successful state recovery using dynamic correction gates.

### 5. CHSH Inequality Violation
📄 **File:** `CHSH Inequality Violation & Finite-Size Statistics.ipynb`
- **Objective:** Experimental verification of non-locality (Bell's Theorem).
- **Key Implementation:**
  - Prepared entangled Bell pairs ($|\Phi^+\rangle$).
  - Measured correlations across different measurement bases.
  - Calculated the CHSH parameter $S$, observing violation of the classical bound ($S > 2$), validating quantum non-locality.

---

## 🛠 Tools & Frameworks
- **SDK:** Qiskit (IBM Quantum)
- **Languages:** Python (NumPy, SciPy, Matplotlib)
- **Concepts:** Linear Algebra, Group Theory, Open Quantum Systems
