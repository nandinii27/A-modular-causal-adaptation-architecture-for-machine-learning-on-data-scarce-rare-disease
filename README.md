# Where does a rare disease enter the network?

A patient-derived line carrying a rare lesion will never be screened at the scale data-hungry models need.
Given a handful of observations from such an unseen context, can a model name the gene through which the
disease enters?

This repository models the disease as a rank-one deviation `u v^T` from a frozen structural causal model
of general biology. Only the deviation is learned, and `argmax u` names the entry node. A bootstrap ensemble
supplies uncertainty, and active acquisition picks the next experiment.

**Paper:** *A modular causal adaptation architecture for machine learning on data-scarce rare disease*,
Nandini Gantayat. Women in Machine Learning (WiML) @ NeurIPS 2026, poster.

## Data

Simulated networks are generated inside the notebook. The Sachs et al. (2005) protein-signalling data
(7,466 cells, 11 proteins, nine conditions) are downloaded by the first cell from the `cdt` package on PyPI.

## Licence

MIT
