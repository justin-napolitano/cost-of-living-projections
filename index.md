---
slug: github-cost-of-living-projections
title: Monte Carlo Simulations for Cost of Living and CO2 Shipping Projections
repo: justin-napolitano/cost-of-living-projections
githubUrl: https://github.com/justin-napolitano/cost-of-living-projections
generatedAt: '2025-11-23T08:45:42.737151Z'
source: github-auto
summary: >-
  Technical overview of probabilistic models estimating US city living costs and transatlantic CO2
  shipping using Monte Carlo simulation methods.
tags:
  - monte-carlo
  - cost-of-living
  - carbon-shipping
  - python
  - simulation
  - data-analysis
seoPrimaryKeyword: monte carlo simulation
seoSecondaryKeywords:
  - cost of living projections
  - carbon shipping cost
  - probabilistic modeling
seoOptimized: true
---

# Technical Overview of cost-of-living-projections

## Motivation

This project aims to provide quantitative projections for two distinct but related domains: the cost of living in major US cities and the economic cost of shipping carbon dioxide across the Atlantic. Both analyses employ Monte Carlo simulations to model uncertainty and variability in key parameters, enabling probabilistic estimates rather than deterministic outputs.

The cost of living models focus on Houston and New York City, providing a data-driven basis for salary negotiation and financial planning. The shipping carbon models estimate the annual cost of transporting supercritical CO2 from European ports to US terminals, a relevant problem in the context of carbon capture and storage infrastructure.

## Problem Statement

1. **Cost of Living:** Estimating living expenses involves multiple uncertain variables such as rent, food, and other monthly costs. Static or point estimates fail to capture this variability, limiting their utility for informed financial decisions.

2. **Shipping Carbon:** The economic feasibility of shipping CO2 depends on complex factors including shipping distances, vessel capacities, and operational costs. Prior estimates contained errors due to unit conversion mistakes, underscoring the need for transparent and reproducible modeling.

## Project Components

### Monte Carlo Simulations

Monte Carlo methods are used extensively to model distributions of uncertain variables. For cost of living, parameters such as rent and food costs are sampled from normal distributions bounded by empirically derived minima and maxima. For shipping costs, variables include shipping distances, capacities, port selections, and round-trip durations, with fixed and variable parameters modeled probabilistically.

### Data Sources

- NYC housing data is included as a CSV file, likely used to parameterize rent distributions.
- Estimates for Houston living costs are based on personal experience and bounded by plausible ranges.
- Shipping data and port information appear to be drawn from academic sources and prior reports, with references to work from Università Bocconi.

### Notebooks and Reports

- `cost_of_living_monte_carlo.ipynb` contains the core Monte Carlo models for living expenses.
- `shipping_projections.ipynb` implements the shipping cost simulation.
- Markdown files document methodology, revisions, and findings, including corrections for earlier errors.

## Implementation Details

- Simulations rely on Python 3 and NumPy for statistical sampling.
- The Monte Carlo approach samples from normal distributions defined by median and standard deviation parameters.
- Shipping cost models include dynamic variables such as shipping distance and capacity, modeled with random sampling within defined bounds.
- Reports emphasize transparency and reproducibility, publishing code alongside results to facilitate verification and error correction.

## Practical Considerations

- The cost of living models currently use dated or approximate data; ongoing work aims to improve data quality through web scraping and updated sources.
- The shipping cost model was revised after discovering a unit conversion error that significantly inflated cost estimates, highlighting the importance of code transparency.
- The project structure separates notebooks, markdown reports, and supporting files for clarity and modularity.

## Summary

This repository serves as a computational toolkit for probabilistic cost projections in two domains with significant economic and policy relevance. It demonstrates the application of Monte Carlo methods to real-world problems, emphasizing reproducibility and iterative refinement. The work is technical and practical, intended as a reference for ongoing development and analysis rather than polished end-user software.

