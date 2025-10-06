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
  - `C-AHP_Experiments_v1.zip`: Package containing the problem to which the proposed methods are applied, the applied methods, all solution steps, data, results, result graphs, and outputs.
    - `Car_Selection_Decision.ods`: Open Office Calc (or Excel) file containing the step-by-step solution and formulations of the car selection problem using AHP, C-AHP, and C-AHP++ methods.
    - `Car_Selection_Decision_All_Results_Comparison_With_Graphs.pdf`: Output file comparing all method outputs with data and schematics.
    - `Car_Selection_Decision_C-AHP(Tau=0.5).pdf`: Output file containing all data sets and results for the $\tau = 0.5$ parameter of the C-AHP method.
    - `Car_Selection_Decision_C-AHP(Tau=1.0).pdf`: Output file containing all datasets and results for the $\tau = 1.0$ parameter of the C-AHP method.
    - `Car_Selection_Decision_C-AHP(Tau=2.0).pdf`: Output file containing all datasets and results for the $\tau = 2.0$ parameter of the C-AHP method.
    - `Car_Selection_Decision_C-AHP++(Tau=0.5).pdf`: Output file containing all datasets and results for the $\tau = 0.5$ parameter of the C-AHP++ method.
    - `Car_Selection_Decision_C-AHP++(Tau=1.0).pdf`: Output file containing all datasets and results for the $\tau = 1.0$ parameter of the C-AHP++ method.
    - `Car_Selection_Decision_C-AHP++(Tau=2.0).pdf`: Output file containing all datasets and results for the $\tau = 2.0$ parameter of the C-AHP++ method.
    - `C-AHP_Simple_Exams.zip`: A package containing all datasets, solutions, results, and result graphs for the example problems solved in the article.
      - `Choosing_A-Laptop_(Tau=0.5).pdf`: Output file containing all datasets and results for the $\tau = 0.5$ parameter of the laptop choice problem.
      - `Choosing_A-Laptop_(Tau=1.0).pdf`: Output file containing all datasets and results for the $\tau = 1.0$ parameter of the laptop choice problem.
      - `Choosing_A-Laptop_(Tau=2.0).pdf`: Output file containing all datasets and results for the $\tau = 2.0$ parameter of the laptop choice problem.
      - `Technology-Company-Investment-Decision_(Tau=0.5).pdf`: Output file containing all data sets and results for the technology company investment decision problem for $\tau = 0.5$.
      - `Technology-Company-Investment-Decision_(Tau=1.0).pdf`: Output file containing all data sets and results for the technology company investment decision problem for $\tau = 1.0$.
      - `Technology-Company-Investment-Decision_(Tau=2.0).pdf`: Output file containing all data sets and results for the technology company investment decision problem for $\tau = 2.0$.
 
## Direct Download
[![DOI](https://zenodo.org/badge/1034360450.svg)](https://doi.org/10.5281/zenodo.16881842)
