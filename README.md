# Autolysis - Automated Dataset Analysis

## Introduction

**Autolysis** is a Python-based automation script designed to analyze CSV datasets and generate both visual and textual reports. The script leverages GPT-4o-Mini via AI Proxy to narrate insightful stories about the data, complemented by several data visualizations using Seaborn and Matplotlib.

## How it Works

1. Load the dataset using `pd.read_csv()`.
2. Perform generic data analysis including:
   - Summary statistics
   - Missing data analysis
   - Principal component analysis (PCA)
   - Correlation analysis
   - Scatter plots between numeric columns
3. Use GPT-4o-Mini via AI Proxy to generate a narrative that explains the findings.
4. Automatically create:
   - A **README.md** file containing the story of the data analysis.
   - Several **PNG charts** visualizing important aspects of the dataset.

## Installation

### Prerequisites

- Python 3.x
- Required libraries (install using `pip`):
  ```bash
  pip install pandas seaborn matplotlib scikit-learn requests python-dotenv
  ```
### Running the Script
- To run the script, use the command line and pass the CSV dataset as an argument:
  ```bash
  uv run autolysis.py dataset.csv
  ```
