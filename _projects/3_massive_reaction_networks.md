---
layout: page
title: Data-driven massive reaction networks
description: Combining DFT, machine learning, and automated reaction enumeration to build the largest known kinetic network for CO₂ hydrogenation on copper.
img: assets/img/ARE_TOC.png
importance: 3
category: work
related_publications: true
---

Real catalytic mechanisms rarely reduce to the few dozen elementary steps typically hand-picked for a microkinetic model — but enumerating all of them by hand doesn't scale either. This project pairs extensive DFT calculations with machine-learned activation-barrier prediction and automated reaction enumeration to build kinetic networks far larger than what human intuition alone would construct.

Applied to CO₂ hydrogenation on copper, the approach starts from a curated set of 152 elementary reactions and expands it to 9,389, cutting the human bias baked into manually curated networks. The resulting model predicts roughly 40-fold higher CO₂ conversion than smaller networks, tracking experimental trends in methanol and CO production, and points to intermolecular hydrogen transfer and molecular-hydrogen-mediated hydrogenation as underappreciated steps — a mechanistic detail the ML-guided search surfaced rather than one we set out looking for.

<span style="display:none">{% cite verma2025data %}</span>
[(Verma and Chaturvedi et al., 2025)](https://chemrxiv.org/engage/chemrxiv/article-details/6751cc927be152b1d00e55c6)
