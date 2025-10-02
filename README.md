# C-AHP and C-AHP++
Contextual and Enhanced-Contextual Analytic Hiyerarchy Process (AHP)

| Feature | Classical AHP | C-AHP | C-AHP++ |
| :--- | :--- | :--- | :--- |
| **Decision Basis** | Purely subjective | Subjective + global objective | Subjective + contextual objective |
| **Input Requirements** | Pairwise judgments only | Judgments + global weights ($\alpha_i$, $\omega_j$) | Judgments + alternative-specific weights ($\alpha_i$, $\omega_{ij}$) |
| **Subjectivity Issue** | Vulnerable ("Super Subjectivity Paradox") | Mitigated via balancing | Resolved via contextual reweighting |
| **Flexibility** | None (static) | Moderate (global context-aware) | High (alternative-specific context-aware) |
| **Contextual Weight Structure** | None | Global vector ($\omega_j$) | Alternative-specific matrix ($\omega_{ij}$) |
| **Main Limitation** | Risk of detachment from reality | Uniform evaluation across alternatives | Requires more data and domain expertise |
| **Gradient-Based Learning** | ❌ No | ✅ Yes $\dagger$ | ✅ Yes $\dagger$ |
| **Differentiability** | ❌ No | ⚠️ Partial (due to $\max$ operator) | ⚠️ Partial (due to $$\max$$ operator) |
| **Entropy Control ($\tau$)** | ❌ No | ✅ Yes | ✅ Yes |

> $\dagger$ End-to-end learning is feasible when the position of $\max_{m} t_{im}$ remains fixed during training (i.e., decision topology is stable).

