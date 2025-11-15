# hardy-pme-adaptive
Adaptive solver for PME &amp; R-PME using Hardy inequalities and level-set refinement
**Hardy-Inequality Based Adaptive Algorithms for PME and R-PME**  
*November 3, 2025 | Demetrios A. Pliakis*

> **80–90% fewer grid points** | **Sharp free boundaries** | **Real estate dynamics**

An efficient, open-source Python implementation of adaptive numerical methods for the **Porous Medium Equation (PME)** and **Reaction-PME (R-PME)**.

### Key Features
- **Level-set-guided mesh refinement** using **Hardy inequality stability estimates**
- **Modified Stefan condition** for R-PME with source terms (e.g., logistic growth)
- **1D core solver** with implicit tridiagonal scheme and dynamic time-stepping
- **Higher-D framework** via **geodesic pixel decomposition**
- **Real estate applications**: gentrification waves, transit impact, market crashes

### Performance (1D)
| Method             | Mesh Points | Time Step | Free Boundary |
|--------------------|-------------|-----------|---------------|
| Uniform FDM        | 1000–5000   | ~10⁻⁶     | Diffuse       |
| **Hardy-Adaptive** | **100–600** | **~10⁻³** | **Sharp**     |

**Full Technical Report:** [docs/PME_R_PME.pdf](docs/PME_R_PME.pdf)  
**Live Examples:** `examples/barenblatt_1d.py`, `examples/gentrification_1d.py`  
**Cite:** [CITATION.cff](CITATION.cff)

---
