# Shetti-AI: Precise prediction of protein sequence mutational landscapes to accelerate functional assays

## Status 
> **Manuscript is under revision.**
> 
> This repository contains the Phase 1 computational pipeline. For inquiries regarding Phase 2 modules or collaboration, please contact the author directly via GitHub.

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
**Sobhy. Shetti-AI: Precise prediction of protein sequence mutational landscapes to accelerate functional assays (Under Revision).**

---

## Author & Contact
Haitham Sobhy 
GitHub: (https://github.com/hsobhy)

---

## References 
* **Sobhy H.** — A tool to parse, manipulate large datasets of sequences — *Microbial Genomics* 2015; [PMID: 28348820](https://pubmed.ncbi.nlm.nih.gov/28348820/)
* **Sobhy H.** — A bioinformatics pipeline to search functional motifs within whole-proteome. *V. Genes* 2017; [PMID: 28000080](https://pubmed.ncbi.nlm.nih.gov/28000080/)
* **Sobhy H.** — A review of functional motifs utilized by viruses — *Proteomes* 2016; [PMID: 28248213](https://pubmed.ncbi.nlm.nih.gov/28248213/)
* **Sobhy H.** — The potential functions of protein domains during COVID Infection. *COVID J.* 2021; DOI: [10.3390/covid1010032](https://doi.org/10.3390/covid1010032)

---

# 🔒 Copyright & Usage Restrictions
**Copyright (c) 2026 Haitham Sobhy. All Rights Reserved.**

This notebook and associated code are provided **solely for non-profit academic research and peer-review evaluation**.

- **Citation Requirement:** If you use, reference, or evaluate this work, you must cite:
  > **Shetti-AI: Precise prediction of protein sequence mutational landscapes to accelerate functional assays (Under Revision)**
- **Corporate R&D & Commercial Restriction:** Any use, execution, or testing by commercial entities, for-profit corporations, or corporate R&D divisions is **STRICTLY PROHIBITED**.
- **Permissions:** No part of this codebase may be copied, redistributed, or modified without prior explicit written permission.
- **Contact:** `hsobhy at live dot com`




