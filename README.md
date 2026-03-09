# Life as a Dynamical Attractor

This project explores a minimal dynamical model for the emergence of sustained activity in a prebiotic chemical network.  
The goal is to study how nonlinear feedback and environmental forcing can produce **stable dynamical attractors**, bistability, and symmetry breaking.

The central question is whether chemical activity collapses to zero or persists as a self-sustaining dynamical state.

---

# Model

The system is modeled by the nonlinear differential equation

$$
\frac{dx}{dt} = \alpha \frac{x^n}{K^n + x^n}\left(1 - \frac{x}{K_c}\right) - \delta x + I
$$

where

- $x$ — activity level of the chemical network  
- $\alpha$ — feedback strength  
- $n$ — Hill coefficient controlling nonlinearity  
- $K$ — saturation constant  
- $K_c$ — carrying capacity representing resource limitation  
- $\delta$ — degradation rate  
- $I$ — environmental input  

The equation combines four competing mechanisms:

1. nonlinear autocatalytic amplification  
2. feedback saturation through a Hill function  
3. logistic limitation due to finite resources  
4. degradation and external environmental forcing  

These interactions determine whether activity collapses or persists as a stable attractor.

---

# What This Notebook Investigates

The notebook analyzes the system using several tools from nonlinear dynamical systems:

- time evolution of activity
- persistence versus collapse
- bifurcation structure
- basin of attraction and robustness
- recovery from perturbations
- extension to chiral symmetry breaking

The goal is to understand **when life-like persistent dynamics can emerge from simple chemical feedback systems.**

---

# Notebook Structure

## Life as a Dynamical Attractor

- Model Equation  
- Baseline Parameters  
- Time Series Simulation  
- Persistence Classification  
- Effect of Feedback Strength  
- Steady-State Activity as a Function of Feedback Strength  
- Persistence Regime Maps (environmental viability)  
- Three-State Regime Map (Collapse / Bistable / Persistent)  
- Bistability and Attractor Structure  
- Phase-Line Diagram  
- Bifurcation Diagram  

These sections analyze how nonlinear feedback creates stable or unstable dynamical regimes.

---

## Basin of Attraction

- Locating a Bistable Environment  
- Interpretation of Candidate Bistable Points  
- Basin of Attraction at a Bistable Point  
- Basin Robustness Landscape  
- Recovery from Perturbations  

These analyses examine the robustness of the persistent state and how the system responds to perturbations.

---

## Chirality Effects

- Chirality and Persistence  
- Chirality Symmetry Breaking  
- Chiral Dynamics  
- Phase Portrait of the Chiral System  
- Quantifying Chirality: Enantiomeric Excess  
- Final Enantiomeric Excess Across Parameters  

The model is extended to two competing species $L$ and $R$ representing left- and right-handed molecular forms.  
This allows investigation of **spontaneous symmetry breaking and the emergence of homochirality**.

---

## Possible Extension

- Resource-Coupled Persistence  

This section outlines a possible extension where chemical activity is coupled to explicit resource dynamics.

---

# How to Run

Install dependencies:
pip install -r requirements.txt

Then run the notebook:
All figures and analyses will be generated automatically when the notebook cells are executed.

---

# License

This project is released under the MIT License.