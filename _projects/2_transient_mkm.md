---
layout: page
title: Unsteady-state microkinetic modeling
description: An automated framework for transient microkinetic modeling that captures the dynamics of CO reduction and oxygen evolution during potential sweeps.
img: assets/img/ADTS_TOC.png
importance: 2
category: work
related_publications: true
---

Most microkinetic models of electrochemical reactions assume steady state — a reasonable simplification, but not what actually happens during a voltammetry sweep. This project builds an unsteady-state microkinetic modeling (USS-MKM) framework that tracks surface coverages as the applied potential changes in real time, matching how linear sweep and staircase voltammetry experiments are actually run.

The framework initializes a clean surface, runs the microkinetic model at each potential step, carries the resulting coverages forward as the initial condition for the next step, and repeats across the full potential window — automated and scalable to large reaction networks. Applied to CO reduction and oxygen evolution, USS-MKM agrees well with prior steady-state results at long times and reproduces experimental CO reduction current densities, while also exposing transient behavior that steady-state models simply can't see.

<span style="display:none">{% cite chaturvedi2025transient %}</span>
[(Chaturvedi et al., 2025)](https://advanced.onlinelibrary.wiley.com/doi/10.1002/adts.202500799)
