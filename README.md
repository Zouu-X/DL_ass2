# Deep Learning Assignment 2

This project demonstrates how to analyze and generate molecular data with deep learning. It contains three major tasks:

1. **SMILES-based energy prediction** – character embeddings and an LSTM are used to predict formation energies from SMILES strings.
2. **Geometry-based energy prediction** – a SchNet model predicts formation energies from atomic coordinates and types.
3. **Molecule generation** – an autoregressive LSTM generates SMILES strings and evaluates their validity, uniqueness, and novelty.

## Repository layout

```
ass2_data/            # Raw coordinates, atom types, SMILES, and energies
clean_data/           # Preprocessed coordinate and atom type data
models/               # Trained model weights
ass2_skeleton.ipynb   # Notebook with the full workflow and sample code
Deep_learning_assignment_2.pdf  # Background and assignment description
```

## Dependencies

- Python 3.10+
- PyTorch
- torch-geometric
- RDKit

It is recommended to create a `conda` environment and install these packages there.

## Quick start

1. Open `ass2_skeleton.ipynb` and follow the steps to load data, train models, and evaluate generation results.
2. If needed, extract core components from the notebook into scripts or libraries for reuse.

## Further study

- Read the code comments on data processing and training routines to deepen your understanding of PyTorch and graph neural networks.
- Try replacing or extending the existing models (e.g., with Transformers or other GNN architectures).
- Write unit tests and visualization tools to improve engineering quality.

