# Computational Drug Formulation Toolkit with DeepChem

A toolkit for predicting key molecular properties relevant to drug formulation using DeepChem.

## Overview

It demonstrates how computational predictions can guide formulation scientists, reducing trial-and-error approaches in pharmaceutical development. This project showcases the use of DeepChem to predict properties that impact drug formulation decisions.

## Key Features

- **Property Prediction Models** for:
  - Solubility (ESOL dataset)
  - Lipophilicity (Lipophilicity dataset)
  - Blood-Brain Barrier Permeability (BBBP dataset)
  - Toxicity (Tox21 dataset)
  - Hydration Free Energy (FreeSolv dataset)
- **Molecular Visualization** tools to inspect compounds
- **Integrated Formulation Strategy** connecting predictions to practical decisions

## Getting Started

### Installation

```bash
# Clone the repository
git clone https://github.com/heilcheng/pharma-pred.git
cd pharma-pred

# Install dependencies
pip install -r requirements.txt
```

### Running the Tutorials

The notebooks directory contains comprehensive tutorials on predicting properties relevant to drug formulation.

If using Jupyter:
```bash
jupyter notebook notebooks/Tutorial_v1.ipynb
```

If using Google Colab, you can upload the notebook directly to Colab.

## Tutorial Content

The tutorial demonstrates:

1. **Setup and Imports**: Installing and importing necessary libraries
2. **Solubility Prediction**: Using the ESOL dataset to predict aqueous solubility
3. **Lipophilicity Prediction**: Understanding distribution and membrane permeability
4. **BBB Permeability**: Classifying compounds that can cross the blood-brain barrier
5. **Toxicity Prediction**: Early assessment of potential toxicity issues
6. **Hydration Free Energy**: Understanding water interactions for stability
7. **Custom Dataset Example**: Implementing a specialized prediction model

## Key Challenges in Drug Formulation Addressed

- **Solubility and Bioavailability:** Predicting aqueous solubility (logS) helps select solubility-enhancing techniques.
- **Distribution and Permeability:** Predicting lipophilicity (logD/logP) helps understand drug distribution. Blood-Brain Barrier (BBB) permeability predictions are crucial for CNS drugs.
- **Toxicity:** Predicting toxicity avoids harmful formulations early.
- **Stability:** Predicting properties like hydration free energy informs stability and interactions.

## Integrated Approach

By combining these predictions, formulators can build a more complete profile of a drug candidate early on:
* **Identify Challenges:** Is the drug poorly soluble? Highly lipophilic? Potentially toxic? Likely to cross the BBB unexpectedly?
* **Select Excipients & Technologies:** Predictions guide the choice of solubilizers, stabilizers, permeation enhancers, and formulation types (e.g., solid dispersions, lipid systems, nanoparticles).
* **Reduce Experiments:** Computational screening focuses lab work on the most promising formulation strategies, saving time and resources.
* **Optimize Delivery:** Tailor formulations for specific needs (e.g., ensuring CNS penetration or designing extended-release for rapidly cleared drugs).

While *in silico* models don't replace experiments, they provide valuable guidance, enabling more rational, efficient, and successful drug formulation development.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- The DeepChem team for their powerful cheminformatics framework
- MoleculeNet for well-curated pharmaceutical datasets
- RDKit for cheminformatics capabilities