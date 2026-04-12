# Quantum Computation and Optimization

A demonstration of Quantum Computing Advantage using the BERNSTEIN-VAZIRANI Algorithm to achieve an optimized constant O(1) time complexity, over a Classical Computing Technique which takes O(n) time complexity.

The Bernstein–Vazirani algorithm demonstrates a quantum advantage in the query model for identifying a hidden bit string 
𝑠∈{0,1}^𝑛, given an oracle function:

𝑓(𝑥) = 𝑠⋅𝑥 (mod 2)

This project has been independently attempted, designed, and implemented by me as an independent self-initiated study project. It has been developed as part of my independent learning journey in quantum methodologies, focusing on how they are becoming superior to classical methods in solving complex, unstructured problems in a much more optimized form, combining algorithmic computations, and mathematical and physical analysis.

# Tools used and Design procedure

1. Python as the programming language, using Matplotlib and Qiskit.
2. Google Colab as the execution platform.
3. Quantum circuit generated using Qiskit.

The project follows these steps:

1. We define a classical query model.
2. Then implement quantum style search logic.
3. Compare query complexities and performance between classical and quantum approaches.
4. Generate circuit representation : Visualize quantum circuit using Qiskit.
5. Finally, generate a well defined technical report.

# Supporting Theory

The superiority of the quantum model over the classical approach arises from the unique properties of quantum states. In quantum computation, a system can exist in a superposition of multiple basis states simultaneously, allowing parallel evaluation of all possible inputs within a single computational step.

The quantum system is initialized into a uniform superposition:

(1/(2^(𝑛/2)))* ∑ 𝑥∈{0,1}^𝑛 ∣𝑥⟩

When the oracle operation is applied, information about the hidden function is encoded into the phase of the quantum state.

The oracle acts as a phase-kickback transformation:

∣x⟩ to (-1)^(s.x) ∣x⟩


This operation encodes global information about the hidden string s into the relative phase structure of the quantum state, without collapsing the superposition.

Applying Hadamard transforms before and after the oracle causes the phase information to interfere constructively on the computational basis state ∣𝑠⟩, while all other basis states undergo destructive interference.

Constructive interference reinforces the amplitudes corresponding to valid computational outcomes, whereas destructive interference cancels amplitudes associated with invalid states. This interference-based filtering mechanism enables the extraction of global information about the system using significantly fewer computational steps than required in classical models.

Thus, the combination of superposition, phase encoding, and interference dynamics provides an efficient computational mechanism fundamentally unavailable in classical computation, establishing the quantum model as much superior for this class of problems, and as a result, the final measurement yields the exact hidden string 𝑠 with probability 1 after a single oracle query.

# Results and Observations

1. The implementation and results demonstrate the efficiency advantage of the quantum based Bernstein–Vazirani algorithm in determining a hidden binary string.
2. In the classical attempt scenario, identifying the hidden string requires multiple queries equal to the length of the string.
3. In contrast, the quantum implementation determines the entire hidden string using only a single query to the oracle.
4. The output results verify that the measured quantum state correctly reconstructs the hidden bit string, demonstrating the computational advantage of the quantum approach.

# Author 
Sayan Pramanik.

# Quantum Solver Project

Click below to open and run the required code directly in Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/SynPmk/Quantum_Computation_and_Optimization/blob/main/quantum_algorithm.ipynb)



