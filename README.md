# PINN-Based Dual Stage Model for Efficient CFD Predictions

A Physics-Informed Neural Network (PINN) based dual-stage deep learning framework designed to accelerate and improve Computational Fluid Dynamics (CFD) predictions by integrating physical laws directly into the neural network training process.

---

## 📌 Project Overview

Traditional Computational Fluid Dynamics (CFD) simulations are computationally intensive and time-consuming due to high-resolution meshing and iterative solvers. This project proposes a **Dual-Stage Physics-Informed Neural Network (PINN)** model to efficiently approximate CFD solutions while preserving governing physical laws.

The key objective is to reduce computational cost while maintaining high prediction accuracy for fluid flow fields such as velocity and pressure distributions.

---

## 🧠 Key Concepts

### 🔹 Physics-Informed Neural Networks (PINNs)
PINNs incorporate governing Partial Differential Equations (PDEs), such as the Navier-Stokes equations, directly into the loss function of the neural network. This ensures that predictions satisfy physical constraints rather than relying purely on data-driven learning.

### 🔹 Dual-Stage Architecture
The model is structured in two stages:

1. **Stage 1 – Physics-Constrained Approximation**
   - Learns a coarse solution guided by PDE residuals.
   - Ensures physical consistency.

2. **Stage 2 – Refinement Network**
   - Improves prediction accuracy.
   - Reduces residual errors.
   - Enhances stability and convergence.

This structured approach improves generalization and reduces training instability often seen in standard PINNs.

---

## 🎯 Objectives

- Reduce computational burden of traditional CFD solvers.
- Maintain physical consistency in predicted flow fields.
- Improve convergence speed using staged training.
- Provide a scalable AI-based CFD alternative.

---

## 📁 Repository Contents

- `AMAN_UGP_Report.pdf` – Complete project report including methodology, equations, experiments, and results.
- `UGP.pptx` – Project presentation slides.
---

## ⚙️ Methodology

1. Formulate governing equations (e.g., Navier-Stokes).
2. Construct neural network architecture.
3. Define composite loss:
   - Data loss
   - PDE residual loss
   - Boundary condition loss
4. Train Stage 1 network.
5. Use refined outputs in Stage 2.
6. Evaluate performance against reference CFD solutions.

---

## 📊 Expected Benefits

- Faster predictions compared to full CFD simulations.
- Reduced dependency on large labeled datasets.
- Physics-consistent outputs.
- Improved stability compared to single-stage PINNs.

---

## 🛠️ Tools & Technologies

- Python
- Deep Learning Framework (PyTorch / TensorFlow)
- NumPy
- SciPy
- Matplotlib
- Physics-Informed Neural Networks (PINNs)

---
