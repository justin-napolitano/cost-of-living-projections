# cost-of-living-projections

This repository contains Monte Carlo simulation models focused on projecting costs related to living expenses in major US cities and the annual economic cost of shipping carbon dioxide from Europe to US ports. It includes Jupyter notebooks, markdown reports, and supporting data files for reproducible analysis.

---

## Features

- Monte Carlo simulations for cost of living projections in Houston and New York City.
- Monte Carlo modeling of the annual cost of shipping supercritical CO2 across the Atlantic.
- Transparent, reproducible computational notebooks combining data analysis and domain-specific modeling.
- Markdown reports documenting methodology, findings, and revisions.

---

## Tech Stack

- Python 3 (Jupyter Notebooks)
- NumPy (for statistical sampling and distributions)
- Markdown for documentation

---

## Getting Started

### Prerequisites

Ensure Python 3 and Jupyter Notebook are installed. Recommended to use a virtual environment.

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

Launch Jupyter Notebook:

```bash
$ jupyter notebook
```

Open and run the following notebooks:
- `cost_of_living_monte_carlo.ipynb` — Monte Carlo models for Houston and NYC cost of living.
- `shipping_projections.ipynb` — Monte Carlo simulation of CO2 shipping costs.
- `carbon-storage-projects.ipynb` — Related analysis on carbon storage projects.
- `europe_ports.ipynb` — Data and analysis related to European ports.

---

## Project Structure

```
├── carbon-storage-projects.ipynb       # Analysis of carbon storage projects
├── cost_of_living_monte_carlo.ipynb     # Monte Carlo models for cost of living
├── cost_of_living_monte_carlo.md         # Markdown report for cost of living projections
├── cost_of_living_monte_carlo_files/     # Supporting files for the above notebook
├── europe_ports.ipynb                     # Data and analysis on European ports
├── histogram.png                         # Visualization image
├── nyc-housing.csv                       # Dataset used for NYC housing cost modeling
├── shipping_carbon_feasibility.md       # Feasibility report on shipping carbon
├── shipping_carbon_feasibility_files/   # Supporting files for feasibility report
├── shipping_projections.ipynb           # Monte Carlo simulation of shipping costs
├── shipping_projections.md               # Markdown report for shipping projections
└── shipping_projections_files/           # Supporting files for shipping projections
```

---

## Future Work / Roadmap

- Update cost of living models with more recent and granular data, especially for NYC and Houston.
- Improve shipping cost model by incorporating dynamic cost of transport distributions.
- Extend the shipping model to include additional ports and shipping routes.
- Automate data scraping pipelines for housing and shipping cost data.
- Enhance visualization and reporting for clearer communication of uncertainty and results.

---

*Note: This project emphasizes transparency and reproducibility. All analyses are published with code to ensure rigor.*
