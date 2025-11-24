---
slug: github-cost-of-living-projections-note-technical-overview
id: github-cost-of-living-projections-note-technical-overview
title: Cost of Living Projections
repo: justin-napolitano/cost-of-living-projections
githubUrl: https://github.com/justin-napolitano/cost-of-living-projections
generatedAt: '2025-11-24T18:33:37.091Z'
source: github-auto
summary: >-
  This repo runs Monte Carlo simulations for projecting living expenses in major
  US cities and calculates the annual cost of CO2 shipping from Europe to the
  US. It offers Jupyter notebooks, reports, and data files for easy
  reproducibility.
tags: []
seoPrimaryKeyword: ''
seoSecondaryKeywords: []
seoOptimized: false
topicFamily: null
topicFamilyConfidence: null
kind: note
entryLayout: note
showInProjects: false
showInNotes: true
showInWriting: false
showInLogs: false
---

This repo runs Monte Carlo simulations for projecting living expenses in major US cities and calculates the annual cost of CO2 shipping from Europe to the US. It offers Jupyter notebooks, reports, and data files for easy reproducibility.

## Key Features
- Simulations for living costs in Houston and NYC.
- Economic modeling for shipping supercritical CO2.
- Clear Jupyter notebooks for analysis and modeling.
- Markdown reports detailing methods and findings.

## Tech Stack
- Python 3
- Jupyter Notebooks
- NumPy for sampling

## Getting Started
Ensure you have Python 3 and Jupyter. Use a virtual environment if possible.

### Installation
```bash
$ git clone https://github.com/justin-napolitano/cost-of-living-projections.git
$ cd cost-of-living-projections
$ python3 -m venv venv
$ source venv/bin/activate  # Or venv\Scripts\activate on Windows
$ pip install numpy jupyter
```

### Run the Notebooks
Launch Jupyter Notebook:
```bash
$ jupyter notebook
```
Open:
- `cost_of_living_monte_carlo.ipynb`
- `shipping_projections.ipynb` 

Note: Keep an eye on data updates and model refinements.
