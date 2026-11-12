# Quantum computing notebooks

Beginner notebooks in Qiskit and PennyLane, written while learning quantum computing. Everything runs on simulators. I have not used real quantum hardware.

| Notebook | What it covers |
|---|---|
| `01_quantum_basics.ipynb` | Statevectors, inner products, Pauli and Hadamard gates, a first circuit, tensor products, density matrices, partial trace, von Neumann entropy |
| `02_deutsch_jozsa.ipynb` | Deutsch (1 bit, four oracles) and Deutsch–Jozsa (n bits): deciding constant vs balanced with one query |
| `03_grover.ipynb` | Grover search over 4 qubits: oracle, diffuser, about 98% success on the target |
| `04_shor_order_finding.ipynb` | Quantum order-finding for N=15, a=7, plus the classical step that recovers the factors 3 and 5 |
| `05_variational_classifier.ipynb` | A 2-qubit variational classifier on Iris (setosa vs versicolor) with a train/test split |

## Limitations
- `04` is the order-finding core of Shor's algorithm with hard-coded modular multiplication for N=15. It does not scale to larger numbers.
- `05` is a toy model on two features of one small dataset, not a benchmark.

## Run
```
pip install qiskit qiskit-aer pennylane scikit-learn sympy matplotlib pylatexenc jupyter
jupyter notebook
```

## Credits
The modular-multiplication circuits in `04` follow the approach in the Qiskit textbook.
