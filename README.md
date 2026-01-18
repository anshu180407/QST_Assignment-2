# Density Matrix Reconstruction using Track 1

This project focuses on building and training a machine learning model that can reconstruct a quantum density matrix ρ from given measurement data. The approach ensures that the reconstructed state satisfies all required physical constraints, including Hermiticity, positive semi-definiteness, and unit trace.

## Overview
- Track: 1 (Transformer-based model):
  Objective:Estimate the density matrix ρ from Pauli measurement expectation values
- Constraint Enforcement:Cholesky decomposition:  
  ρ = (L L†) / Tr(L L†)
- Quantum System:2-qubit system

## Project Structure
- src/ : Core source code (data generation, model, training)
- docs/ : Documentation files
- outputs/ : Saved model checkpoints

## Quick Start

- Install dependencies:
  pip install numpy torch scipy

- Train the model:
  python src/train.py

-The best trained model will be saved in the 'outputs/' directory.

## Design and Documentation
- Model architecture and mathematical logic are explained in 'docs/model_working.md'
- Steps to reproduce the results are provided in 'docs/replication_guide.md'

## Results

On the test set, the model achieves a mean quantum fidelity of approximately 0.97 and a mean trace distance of around 
0.079. The average inference latency is approximately 2.846 ms per density matrix reconstruction on CPU. Due to random dataset generation and training initialization, results may vary slightly across runs.


