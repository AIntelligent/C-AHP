# Experimental Materials for "Multi-Criteria Decision Making through the Fusion of Quantitative and Qualitative Information: A Triadic Information Fusion Model and an Innovative Approach in AHP"

C-AHP and C-AHP++ are two improved versions of the AHP method. In this repository, you will find experimental results of these new methods and their application to a real problem such as *"Car Selection"*.

> Kartal, Hakan Emre [hek@nula.com.tr](hek@nula.com.tr) [0000-0002-3952-7235](https://orcid.org/0000-0002-3952-7235)
> **DOI**: [pending](https://doi.org/)

## C-AHP and C-AHP++
**Contextual and Enhanced-Contextual Analytic Hierarchy Process**  
(Extensions of the classical AHP framework)

| Feature | Classical AHP | C-AHP | C-AHP++ |
| :--- | :--- | :--- | :--- |
| **Decision Basis** | Pairwise subjective judgments only | Fusion of subjective judgments with global context | Fusion of subjective judgments with alternative-specific context |
| **Input Requirements** | Pairwise judgments only | Judgments + global alternative ($\alpha_i$) and criteria ($\omega_j$) weights | Judgments + alternative-specific contextual weights ($\alpha_i$, $\omega_{ij}$) |
| **Subjectivity Issue** | Vulnerable (“Super Subjectivity Paradox”: all weights entirely subjective) | **Resolved via global subjective–objective fusion** | **Resolved via contextualized reweighting (alternative-specific)** |
| **Flexibility** | Static (no context awareness) | Moderate (global context-aware) | High (alternative-specific context-aware) |
| **Contextual Weight Structure** | None | Global vector ($\omega_j$): one weight vector shared across all alternatives | Alternative-specific matrix ($\omega_{ij}$): contextualized per alternative and criterion |
| **Main Limitation** | Risk of detachment from reality | Uniform evaluation across alternatives | Requires larger data and stronger domain expertise to parameterize $\omega_{ij}$ |
| **Gradient-Based Learning** | ❌ No | ✅ Yes † | ✅ Yes † |
| **Differentiability** | ❌ No | ⚠️ Partially differentiable (piecewise due to $\max$) | ⚠️ Partially differentiable (piecewise due to $\max$) |
| **Entropy Control ($\tau$)** | ❌ No | ✅ Yes (temperature parameter $\tau$ tunes subjectivity–objectivity balance) | ✅ Yes (same as C-AHP, extended to contextual weights) |
> † End-to-end gradient learning is possible provided the $\max$-based decision topology remains constant during training.

## Files
- `HBB.zip`: All the ingredients required for *Hemoglobin-β (HBB)*.
  - `P68871.fasta`: This a bioinformatics file in FASTA fmat containing the *Hemoglobin-β* protein sequence from the **UniProt (Universal Protein Resource)** database.
  - `last_alignment_data.txt`, `final_alignment_used.txt` and `final_alignment.clustal`: This is a *Hemoglobin-β* protein alignment file created in Clustal format.
  - `C-Softmax_HBB_Notebook_v2_en.ipynb - Colab.pdf`: Results of HBB tests.
  - `C_Softmax_HBB_Notebook_v2_en.ipynb`: Interactive Jupyter Notebook (compatible with Google Colab).
  - `blosum62.txt`:

## Direct Download
[![DOI](https://zenodo.org/badge/1034360450.svg)](https://doi.org/10.5281/zenodo.16881842)

