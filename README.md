# 🎯 Quantum Optimization: Marketing Budget Allocation with QAOA

This repository presents an integer quadratic programming problem for marketing budget allocation, solved using the **Quantum Approximate Optimization Algorithm (QAOA)** from Qiskit.  

We model a realistic scenario where a limited advertising budget must be allocated across three customer segments: **children/teens**, **single adults**, and **parents**. To **maximize total expected utility**, considering:
- The individual impact per segment,
- The saturation effect (diminishing returns),
- The interaction effects (synergies or cannibalization) between segments.

---

## ⚖️ Classical vs Quantum Comparison

Before applying QAOA, the problem was first solved using a **classical exact optimizer** to find the optimal solution and serve as a benchmark.  
This allows for a direct comparison between the classical and quantum-inspired solutions in terms of Accuracy of the solution.

---

## 📊 Problem Formulation

We solve the following quadratic integer optimization problem:

$$\begin{align}
\text{Maximize}\quad{} & f(x) = 6.5x_1 + 9.0x_2 + 7.8x_3 - (0.6x_1^2 + 0.9x_2^2 + 0.5x_3^2) + 0.3x_1x_2 - 0.4x_1x_3 + 0.7x_2x_3\\
\text{subject to}\quad{} & x_1 + x_2 + x_3 \leq 10   \\
                         & 0 \leq x_1 \leq 5         \\
                         & 0 \leq x_2 \leq 5         \\
                         & 0 \leq x_3 \leq 5         \\
\end{align}$$

---

## 🚀 Technologies Used

- 🧠 **Qiskit** – for quantum simulation and QAOA
- 💻 **Python** – Jupyter Notebook / Colab-friendly

---

## 📁 Files

| File | Description |
|------|-------------|
| `Quantum_Optimization_Marketing_Budget_Allocation.ipynb` | Main notebook with full model, classic and quantum approach, QAOA configuration, and results |

---

