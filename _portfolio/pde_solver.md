---
title: "Neural Network PDE Solver"
collection: portfolio
permalink: /portfolio/pde-solver
date: 2025-09-01
excerpt: "A physics-informed neural network project for solving PDEs. <br/><img src='/images/PINN_structure.png'>"
tags:
  - Machine Learning
  - Physics-Informed AI
  - PDEs
---

Partial differential equations (PDEs) underpin models across science and engineering, yet analytical solutions are atypical and classical mesh-based solvers can be costly in high dimensions. This dissertation presents a unified comparison of three mesh-free neural PDE solvers, physics-informed neural networks (PINNs), the deep Ritz method (DRM), and weak adversarial networks (WANs), on Poisson problems (up to 5D) and the time-independent Schr\"odinger equation in 1D/2D (infinite well and harmonic oscillator), and extends the study to a laser-driven case of Schrödinger's equation via the Kramers-Henneberger (KH) transformation.

Under a common protocol, all methods achieve low $L_2$ errors ($10^{-6}$-$10^{-9}$) when paired with forced boundary conditions (FBCs), forced nodes (FNs), and orthogonality regularization (OG). Across tasks, PINNs are the most reliable for accuracy and recovery of excited spectra; DRM offers the best accuracy-runtime trade-off on stationary problems; WAN is more sensitive but competitive when weak-form constraints and FN/OG are used effectively. Sensitivity analyses show that FBC removes boundary-loss tuning, network width matters more than depth for single-network solvers, and most gains occur within 5000-10,000 epochs. The same toolkit solves the KH case, indicating transfer beyond canonical benchmarks.

We provide practical guidelines for method selection and outline the following extensions: time-dependent formulations for DRM and WAN, adaptive residual-driven sampling, parallel multi-state training, and neural domain decomposition. These results support physics-guided neural solvers as credible, scalable tools for solving complex PDEs. 

👉 [View on GitHub](https://github.com/JiakangC/Neural-Network-Based-PDE-Solver.git)

📄  [Read Full Dissertation (PDF)](/files/msc-dissertation.pdf)
