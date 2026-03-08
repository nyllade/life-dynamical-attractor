# Life as a Dynamical Attractor

This project explores how simple nonlinear feedback systems can produce
persistent activity states that resemble life-like dynamical attractors.

Using a minimal mathematical model, we study how positive feedback,
environmental support, and degradation interact to determine whether
activity collapses or persists.

The notebook demonstrates how persistent dynamical behavior can emerge
from simple nonlinear interactions.

---

# Model

The activity variable \(x(t)\) evolves according to:

```math
\frac{dx}{dt} =
\alpha \frac{x^n}{K^n + x^n}\left(1-\frac{x}{K_c}\right)
- \delta x + I
```

Where:

- \(x\) — activity level
- \(\alpha\) — feedback strength
- \(n\) — Hill coefficient (nonlinearity)
- \(K\) — feedback saturation constant
- \(K_c\) — carrying capacity
- \(\delta\) — degradation rate
- \(I\) — environmental input

The model combines three competing processes:

1. nonlinear autocatalytic feedback
2. degradation / loss
3. environmental support

This minimal framework is used to study when sustained activity can
emerge as a dynamical attractor.

---

# Notebook Structure

The main notebook `attractor_model.ipynb` contains the following analyses:

### 1. Time-Series Dynamics
Simulates activity trajectories over time to show how the system evolves
from small initial conditions.

### 2. Persistence Classification
Determines whether the system converges to collapse or persistent activity.

### 3. Effect of Feedback Strength
Shows how increasing positive feedback changes activation dynamics.

### 4. Steady-State Activity vs Feedback Strength
Analyzes how equilibrium activity depends on feedback strength.

### 5. Persistence Regime Maps
Explores environmental parameter space to determine where activity
can persist.

### 6. Three-State Regime Map
Identifies regions of:
- collapse
- bistability
- persistent activity

### 7. Phase-Line Analysis
Examines fixed points and stability structure of the system.

### 8. Bifurcation Diagram
Shows how steady states change as degradation rate varies.

### 9. Basin of Attraction
Analyzes how initial conditions determine which attractor the system
converges to.

### 10. Perturbation Recovery
Tests resilience of persistent activity under perturbations.

### 11. Chirality Extension
Extends the model to two interacting species (L and R) to explore
symmetry breaking and the emergence of enantiomeric excess.

---

# Installation

Install dependencies before running the notebook:

```bash
pip install -r requirements.txt