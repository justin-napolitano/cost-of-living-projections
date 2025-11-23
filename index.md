---
slug: "github-cost-of-living-projections"
title: "cost-of-living-projections"
repo: "justin-napolitano/cost-of-living-projections"
githubUrl: "https://github.com/justin-napolitano/cost-of-living-projections"
generatedAt: "2025-11-23T08:30:05.244306Z"
source: "github-auto"
---


# Technical Overview of the cost-of-living-projections Repository

## Motivation

This repository addresses two distinct but related economic modeling challenges: projecting annual living costs in major US cities and estimating the annual cost of shipping carbon dioxide from Europe to US ports. Both problems involve uncertainty and variability in input parameters, making Monte Carlo simulation an appropriate methodology.

The cost of living models aim to provide transparent, data-driven estimates to support salary negotiations and financial planning, while the shipping cost models contribute to understanding the economic feasibility of carbon transport infrastructure, a topic of growing importance in climate mitigation strategies.

## Problem Statement

1. **Cost of Living Projection**: Determine the annual housing and living expenses in Houston and New York City using probabilistic modeling to capture variability in rent and food costs. The goal is to estimate a salary threshold sufficient to meet typical landlord income requirements.

2. **Shipping Carbon Cost Projection**: Model the annual economic cost of shipping supercritical CO2 from European ports to US ports. This involves accounting for variable shipping distances, capacities, port selections, and round-trip durations, incorporating uncertainty in these parameters.

## Implementation Details

### Monte Carlo Simulation Approach

The core technique employed is Monte Carlo simulation, where uncertain variables are modeled as random draws from probability distributions (primarily normal distributions bounded by minima and maxima). This approach allows quantification of uncertainty and the generation of confidence intervals for cost estimates.

### Cost of Living Models

- Data Sources: NYC housing data from 2018 and an estimate for Houston based on current rental conditions.
- Variables Modeled: Monthly rent and food costs.
- Methodology: For each variable, define a normal distribution with specified mean and standard deviation based on observed or estimated bounds. Sample repeatedly to simulate annual costs.
- Output: Confidence intervals for annual rent and living expenses, used to infer adequate salary levels (e.g., $90,000 annual salary sufficient for qualifying for median NYC rent).

### Shipping Cost Models

- Variables: Shipping distances, tanker capacities, ports of origin and destination, round-trip durations, and cost per ton of transport.
- Data Handling: Distances between ports and capacities are sampled from distributions reflecting variability. Fixed variables like cost per ton are currently static but planned for conversion to distributions.
- Correction of Errors: A prior decimal conversion error in distance units was identified and corrected, demonstrating the importance of transparency and code publication.
- Modeling Infrastructure: Includes referencing external research on LNG shipping capacities and adapting those to supercritical CO2.

### Documentation and Transparency

- Markdown reports accompany notebooks to document methodology, revisions, and findings.
- The author emphasizes transparency to avoid unintentional misinformation, as evidenced by the public correction of earlier errors.

## Practical Considerations

- The models rely on somewhat dated or estimated data; updates and more granular data scraping are planned to improve accuracy.
- The Monte Carlo approach provides probabilistic insights rather than deterministic answers, which is crucial for decision-making under uncertainty.
- The modular structure allows for extension, such as adding more ports or refining cost parameters.

## Summary

This project exemplifies the use of probabilistic modeling to address real-world economic questions with inherent uncertainty. It combines domain knowledge in urban economics and carbon shipping logistics with computational methods to produce transparent, reproducible analyses. The emphasis on code publication and error correction underscores a commitment to rigor and reliability in modeling.

When returning to this work, focus on the data sources for distributions, the assumptions behind fixed vs. variable parameters, and the integration of domain-specific knowledge into the Monte Carlo framework.