---
layout: page
title: research
permalink: /research/
description: A closer look at a few research threads, beyond the publication list.
nav: true
nav_order: 3
horizontal: false
---

#### Research Experience

- **Shell Technology Centre (STC), Bangalore** — *Unsteady-State Microkinetic Modeling of
  Electrochemical CO₂ Reduction* (Apr 2023 – Oct 2024)
  Co-advisors: Dr. Amardeep Pathak, Dr. Nishant Sinha, Prof. Ananth Govind Rajan
  - Developed and tested a wrapper for MKMCXX, optimizing it for electrochemical CO₂
    reduction simulations
  - Built microkinetic models for reaction pathways and evaluated catalyst performance

- **Malaviya National Institute of Technology, Jaipur** — *Development of a Bio-Adsorbent
  for Arsenic Removal Using a Hydrothermal Process* (Aug 2021 – Mar 2022)
  Advisor: Dr. Madhu Agarwal
  - Developed orange peel–based bio-adsorbents for arsenic removal from potable water in
    rural India
  - Conducted adsorption studies and characterized material performance

- **IASc–INSA–NASI Summer Research Fellowship Programme** (Remote) — *Analyzing COVID-19
  Spread in Chest X-rays Using CNNs* (Jun 2020 – Jul 2020)
  Advisor: Dr. Venkadachalam Ramesh, Central University of Tamil Nadu
  - Designed a CNN-based X-ray analysis model to predict COVID-19 with 96.9% precision
    and 91.7% recall
  - Utilized ResNet with transfer learning for rapid and cost-effective disease detection

- **Institute of Technology & Management, Salt Lake** (Remote) — *Predicting the Viscosity
  of Various Nanofluids Using Artificial Neural Networks* (Aug 2020 – Feb 2021)
  Supervisor: Dr. Satyasaran Changdar
  - Explored a physics-guided neural network framework to develop a generalized model for
    predicting nanofluid viscosity with high accuracy

#### Selected Research Projects

<!-- pages/projects.md -->
<div class="projects">
  {% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_projects = site.projects | where: "category", category %}
  {% assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
      {% for project in sorted_projects %} {% include projects_horizontal.liquid %}
      {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %} {% include projects.liquid %} {% endfor %}
  </div>
  {% endif %} {% endfor %} {% else %}
  <!-- Display projects without categories -->
  {% assign sorted_projects = site.projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
      {% for project in sorted_projects %} {% include projects_horizontal.liquid %}
      {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %} {% include projects.liquid %} {% endfor %}
  </div>
  {% endif %} {% endif %}
</div>
