# C-AHP and C-AHP++
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

> † End-to-end learning is feasible when the position of $\max_{m} t_{im}$ remains fixed during training (i.e., decision topology is stable).

