# Shetti-AI: Generative Intelligence for Protein Motif Engineering

## Status 
**Manuscript in Preparation.** 
 This repository contains the Phase 1 computational pipeline. For inquiries regarding Phase 2 modules or collaboration, please contact the author directly via GitHub.

---

## Overview
Shetti-AI is a generative AI project exploring how adversarial models can operate on structured biochemical representations.

This repository contains **Phase 1**, a proof-of-concept using a Wasserstein GAN (WGAN) to model amino acid feature distributions and generate motif perturbations.

---

## Phase 1 — WGAN Feature-Space Modeling

Phase 1 implements a WGAN trained on simplified amino acid biophysical vectors.  
The model learns the distribution of these features and applies **latent-space perturbations** to generate motif variants.

### Key Points
- Amino acids encoded as low-dimensional biophysical vectors  
- WGAN used for stable training and reduced mode collapse  
- Generator produces feature vectors approximating real amino acid space  
- Mutations performed via vector interpolation + nearest-neighbor mapping  

### Output
- Produces stochastic variations of input motifs  
- Operates purely in feature space 

### Limitations 
- Simplified representation  

---

## Install
```bash
pip install numpy torch biopython
```

---

## Citation & Usage
If you use this code or the associated methodology, please cite as:
**Sobhy. A High-Precision AI Framework for the Prediction of Functional Motif Mutation and Conservation (In Preparation).**

---

## Author & Contact
Sobhy H. 
Email: hsobhy@live.com 
GitHub: (https://github.com/hsobhy)

---

## References 
* **Sobhy H.** — A tool to parse, manipulate large datasets of sequences — *Microbial Genomics* 2015; [PMID: 28348820](https://pubmed.ncbi.nlm.nih.gov/28348820/)
* **Sobhy H.** — A bioinformatics pipeline to search functional motifs within whole-proteome. *V. Genes* 2017; [PMID: 28000080](https://pubmed.ncbi.nlm.nih.gov/28000080/)
* **Sobhy H.** — A review of functional motifs utilized by viruses — *Proteomes* 2016; [PMID: 28248213](https://pubmed.ncbi.nlm.nih.gov/28248213/)
* **Sobhy H.** — The potential functions of protein domains during COVID Infection. *COVID J.* 2021; DOI: [10.3390/covid1010032](https://doi.org/10.3390/covid1010032)

---

## License
This project is licensed under the **GNU Affero General Public License v3.0 (AGPL-3.0)**. 
*Note: This license requires that if you modify this software and run it on a network, you must make your modified source code available to your users. Non-commercial users should contact the author.*




