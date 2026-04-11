# Quantum Computation and Optimization

A demonstration of Quantum Computing Advantage using the BERNSTEIN-VAZIRANI Algorithm to achieve an optimized constant O(1) time complexity, over a Classical Computing Technique which takes O(n) time complexity.

This project has been independently attempted, designed and implemented by me as a self-initiated study project.

It has been developed as part of my independent learning journey in quantum methodologies, how they becoming superior to classical methods in solving many complex problems in much optimized form. 

# Tools used and Design procedure
1. Python as the programming language, using Matplotlib and Qiskit.
2. Google Colab as the execution platform.

The project follows these steps:

1. We define a classical query model.
2. Then implement quantum style search logic.
3. Compare query complexities and performance between classical and quantum approaches.
4. Generate circuit representation.
5. Finally, generate a well defined technical report.

# Supporting Theory

The superiority of the quantum model over the classical approach arises from the unique properties of quantum states. In quantum computation, a system can exist in a superposition of multiple basis states simultaneously, allowing parallel evaluation of all possible inputs within a single computational step.
When the oracle operation is applied, information about the hidden function is encoded into the phase of the quantum state. Subsequent transformations exploit constructive and destructive interference to amplify the probability of the correct solution while suppressing incorrect alternatives.
Constructive interference reinforces the amplitudes corresponding to valid computational outcomes, whereas destructive interference cancels amplitudes associated with invalid states. This interference-based filtering mechanism enables the extraction of global information about the system using significantly fewer computational steps than required in classical models.
Thus, the combination of superposition, phase encoding, and interference dynamics provides an efficient computational mechanism fundamentally unavailable in classical computation, establishing the quantum model as much superior for this class of problems.

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



