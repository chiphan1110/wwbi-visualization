# 📊 Data Visualization - Bureaucracy, Budgets, and the Gender Gap: A Global and Local Perspective

## Overview
This project analyzes global trends in public sector wage spending and gender representation using the *Worldwide Bureaucracy Indicators (WWBI)* dataset curated by the TidyTuesday project.  
We explore two main questions:
- How has the proportion of GDP allocated to public wages changed over time across different world regions and income groups?
- How has the gap in female representation between high-skill and low-skill occupations evolved over time in Vietnam, and how does it differ between the public and private sectors?

The analysis is performed through data visualization techniques, using Python (Pandas, Matplotlib, Seaborn).

Further details on methodology, findings, and discussions are provided in the [proposal.md](proposal.md) and [presentation.pdf](presentation.pdf).

## Repository Structure
```
.
├── code/           # Jupyter notebooks for EDA and main analyses
│   ├── eda.ipynb   # Exploratory Data Analysis
│   ├── q1.ipynb    # Analysis for Question 1 (Public Wage Spending)
│   └── q2.ipynb    # Analysis for Question 2 (Gender Representation)
├── data/           # Dataset files and metadata
│   ├── README.md   # Metadata and codebook for the dataset
│   ├── WWBI-Codebook-v3.1.pdf  # Original data dictionary
│   ├── wwbi_country.csv
│   ├── wwbi_data.csv
│   └── wwbi_series.csv
├── figure/         # Generated figures for the final report and presentation
│   ├── female_occupation_gap_combined.png
│   ├── female_occupation_lollipop.png
│   └── wage_bill_as_gdp.png
├── peer_review/    # Peer review feedback documents
│   ├── group2.md
│   └── group6.md
├── presentation.pdf  # Project presentation slides
└── proposal.md       # Detailed project proposal and report
```

## Getting Started
1. Clone this repository.
2. Install required Python libraries (see inside the notebooks).
3. Open the Jupyter notebooks in the `code/` directory to reproduce the analysis.

## Dataset
- **Source**: World Bank’s Bureaucracy Lab, curated by [TidyTuesday](https://github.com/rfordatascience/tidytuesday/blob/main/data/2024/2024-04-30)
- **Details**: See [data/README.md](data/README.md) for dataset provenance, structure, and codebook.

## Acknowledgement
This project is conducted during the course COMP4010-Data Visualization at VinUniversity. We would like to express our gratitude for the course instructor Prof. Mo El-Haj and TA Kieu Hai Dang for their supportive guidance and feedback. 

---