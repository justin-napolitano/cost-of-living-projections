---
slug: github-cost-of-living-projections-writing-overview
id: github-cost-of-living-projections-writing-overview
title: 'Cost of Living Projections: Simulating the Future'
repo: justin-napolitano/cost-of-living-projections
githubUrl: https://github.com/justin-napolitano/cost-of-living-projections
generatedAt: '2025-11-24T17:12:57.149Z'
source: github-auto
summary: >-
  I built the **cost-of-living-projections** repository to tackle some pressing
  questions about living expenses and carbon logistics, particularly in major
  U.S. cities. This project combines Monte Carlo simulations to produce reliable
  projections of living costs in Houston and New York City, as well as explores
  the economic impact of shipping carbon dioxide across the Atlantic. The aim is
  to unpack complex data into actionable insights using reproducible analysis.
tags: []
seoPrimaryKeyword: ''
seoSecondaryKeywords: []
seoOptimized: false
topicFamily: null
topicFamilyConfidence: null
kind: writing
entryLayout: writing
showInProjects: false
showInNotes: false
showInWriting: true
showInLogs: false
---

I built the **cost-of-living-projections** repository to tackle some pressing questions about living expenses and carbon logistics, particularly in major U.S. cities. This project combines Monte Carlo simulations to produce reliable projections of living costs in Houston and New York City, as well as explores the economic impact of shipping carbon dioxide across the Atlantic. The aim is to unpack complex data into actionable insights using reproducible analysis.

## Why This Project?

Why did I start this? Real-world financial planning isn’t simply about setting a budget; it involves anticipating future costs that can fluctuate wildly. Cities like Houston and NYC have dramatically different living expenses that can shift year-to-year. Simultaneously, as we grapple with climate change, understanding the cost of transporting CO₂ from Europe to U.S. ports is crucial for informed policy-making. 

The core goal is transparency. By using Monte Carlo simulations, we can account for uncertainties in these projections, making them not just guesses but informed estimates based on statistical sampling.

## Key Design Decisions

When I was sketching out the architecture of this project, a few decisions stood out:

- **Simulation-Based Approach:** Monte Carlo simulations allow me to create a range of potential outcomes based on varying inputs. This flexibility provides a richer understanding of possible futures than static forecasts.
  
- **Reproducibility:** I opted for Jupyter notebooks combined with Markdown documentation to ensure that anyone can trace the paths I took in reaching conclusions. After all, good data deserves good documentation.

- **Focus Areas:** I concentrated on two major cost areas – living expenses in Houston and NYC, and the economics of carbon shipping. This emphasis helps keep the project focused but also relevant across different fields of interest.

## Tech Stack

Here's what I’m using to make this all happen:

- **Python 3:** As a language that’s great for data science, it’s the backbone of my notebooks.
- **Jupyter Notebooks:** They let me present data and analysis interactively, making it easier to share findings.
- **NumPy:** Essential for numerical calculations and statistical operations; I rely on it heavily for sampling distributions.
- **Markdown:** Clear, straightforward documentation that aligns with the notebook structure.

## Getting Started

If you want to dive into the analysis, here’s how to get started:

### Prerequisites

Make sure you have Python 3 and Jupyter Notebook installed. Using a virtual environment is highly recommended to keep dependencies tidy.

### Installation

```bash
# Clone the repository
$ git clone https://github.com/justin-napolitano/cost-of-living-projections.git
$ cd cost-of-living-projections

# (Optional) Create and activate a virtual environment
$ python3 -m venv venv
$ source venv/bin/activate  # On Windows use `venv\Scripts\activate`

# Install dependencies
$ pip install numpy jupyter
```

### Running the Notebooks

Launch Jupyter Notebook with the command:

```bash
$ jupyter notebook
```

Then, check these key notebooks:

- `cost_of_living_monte_carlo.ipynb`: Monte Carlo models focusing on Houston and NYC living costs.
- `shipping_projections.ipynb`: Simulation of CO₂ shipping costs — not just a dry economic analysis.
- `carbon-storage-projects.ipynb`: Examines carbon storage initiatives, tying climate policies to fiscal realities.
- `europe_ports.ipynb`: Analyzes available data related to European ports involved in the shipping logistics.

## Project Structure

The files are thoughtfully organized for easy navigation:

```
├── carbon-storage-projects.ipynb       # Analysis of carbon storage projects
├── cost_of_living_monte_carlo.ipynb     # Monte Carlo models for living costs
├── cost_of_living_monte_carlo.md         # Markdown report on projections
├── cost_of_living_monte_carlo_files/     # Supporting files for living cost notebooks
├── europe_ports.ipynb                     # Data and analysis on European ports 
├── nyc-housing.csv                       # Housing data specific to NYC
├── README.md                            # Project overview
├── shipping_carbon_feasibility.md       # Analysis of shipping carbon feasibility
├── shipping_carbon_feasibility_files/   # Supporting files for feasibility report
├── shipping_projections.ipynb           # Monte Carlo simulation of shipping costs
├── shipping_projections.md               # Report on shipping projections
├── shipping_projections_files/           # Supporting files for shipping projections
```

## Future Work / Roadmap

The project is live, but there's always room for improvements. Here’s what’s on my list:

- **Data Updates:** I want to refresh the cost of living data for Houston and find more granular sources for accuracy.
- **Model Refinement:** It’s essential to use better input distributions based on recent data. Making the models more precise is a top priority.
- **Expand Shipping Models:** Additional variables, like infrastructure and operations, will provide a more detailed economic picture.
- **Automated Data Scraping:** I aim to streamline the data collection process to keep projections fresh without manual intervention.
- **Documentation & Testing:** More detailed documentation and strengthening tests will enhance reproducibility, which is a pillar of this project.

## Staying Updated

I often share updates about this project and others on my social channels. If you're into this kind of work, follow along on Mastodon, Bluesky, or Twitter/X for the latest developments and discussions.

In closing, the **cost-of-living-projections** project is my attempt to blend data science with real-world application. I invite you to explore, contribute, and watch this project evolve.
