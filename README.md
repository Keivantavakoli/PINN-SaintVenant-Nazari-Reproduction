# Reproduced PINN Architectures for Saint-Venant Equations

This repository reproduces the **Physics-Informed Neural Network (PINN)** architectures presented in *Nazari et al. (2024)* for modeling 1D Saint-Venant equations.

---

## 📘 Overview
The goal of this project is to **replicate and analyze** the three architectures (A, B, and C) proposed by Nazari, focusing on:
- Parameter learning stability for *S₀* and *n*  
- The effects of noisy derivative data on inverse prediction  
- The impact of MAP regularization and loss weighting  

---

## 🧠 Architectures Implemented
1. **Architecture A (Data-Assisted)** — Uses forward-difference derivatives and learns parameters jointly.  
2. **Architecture B (Pure AD)** — Relies entirely on automatic differentiation for gradient computation.  
3. **Architecture C (MAP Regularization)** — Incorporates a Maximum A Posteriori prior to stabilize parameter learning.

---

## 🧩 Model Description
- **Governing equations:** 1D Saint-Venant (shallow water) equations  
- **Parameters learned:** Channel slope (*S₀*) and Manning’s coefficient (*n*)  
- **Loss components:**  
  - Data Loss (MSE between predicted and reference flow variables)  
  - PDE Loss (MSE of continuity and momentum residuals)  
  - Regularization (optional MAP prior)  

---

## 💬 Comments and Collaboration
This repository was created to **reproduce and verify** the results of *Nazari et al. (2024)* and to encourage open discussion.  
Feel free to:
- Open an **Issue** with questions or feedback  
- Submit **Pull Requests** for improvements  
- Share insights on architecture performance or training stability  

---

## 📚 Citation
If you use or build upon this work, please cite the original study:

> Nazari, M., et al. (2024). *Physics-Informed Neural Networks for Modeling Water Flows in a River Channel*. Journal of Hydrology.

---

## ⚖️ License
This project is released under the **MIT License**, allowing reuse and modification with proper attribution.
