---
layout: page
title: Physics-guided deep learning for nanofluid viscosity
description: A Physics Guided Deep Neural Network (PGDNN) that fuses theoretical viscosity models with data-driven learning to predict nanofluid viscosity.
img: assets/img/JC_TOC.png
importance: 5
category: work
related_publications: true
---

Predicting nanofluid viscosity is hard because purely theoretical models miss the physics that data can capture, while purely data-driven black-box models tend to overfit and generalize poorly beyond their training data. This project develops a Physics Guided Deep Neural Network (PGDNN) that folds physics-based theoretical models directly into the network's loss function, so the model is nudged toward physically consistent predictions rather than fitting the data blindly.

Trained and tested on roughly 9,000 experimental and simulated data points spanning spherical Al2O3, CuO, SiO2, and TiO2 nanoparticles, the PGDNN outperformed traditional theoretical and computational models on unseen data (R² = 0.9961, RMSE = 0.0312) while avoiding the overfitting that plagues black-box approaches. A sensitivity analysis further showed that particle volume fraction is the dominant factor controlling nanofluid viscosity, with base-fluid viscosity a close second — a useful physical checkpoint on top of the raw predictive accuracy.

{% cite bhaumik2023unique %}
