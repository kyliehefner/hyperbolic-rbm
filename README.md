# Hyperbolic Restricted Boltzmann Machine

**Implementation of standard Bernoulli and prototype Hyperbolic Restricted Boltzmann Machines for learning and reconstructing hierarchical WordNet data.**

---

## Features

- **Data Extraction**  
  - Use NLTK to pull synset hierarchies from WordNet (e.g. `animal.n.01`, `dog.n.01`, `pug.n.01`).
  - Convert hypernym/hyponym trees into binary feature matrices.

- **Models**  
  - **Bernoulli RBM**  
    - Built with scikit-learn’s `BernoulliRBM`.  
  - **Hyperbolic RBM**  
    - Prototype implementation using hyperbolic numbers (`j² = +1`) for weights & biases.  
    - Custom hyperbolic arithmetic, activation, sampling, and contrastive divergence.

- **Evaluation & Visualization**  
  - Reconstruction error (direct & extended layers).  
  - Weight heatmaps, activation histograms.  
  - Tree-structured graph visualizations with NetworkX + Graphviz.  
  - Two-layer neighborhood highlighting around test nodes (e.g. `pug.n.01`).
