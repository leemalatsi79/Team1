# Vegetable Price Analysis Project

**A data analysis project that focuses on analyzing vegetable prices and identifying trends from a historical dataset. The project leverages Python and data visualization tools to explore seasonal price fluctuations and correlations between vegetable prices.**

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Analysis](#analysis)
- [Requirements](#requirements)
- [License](#license)
- [Acknowledgements](#acknowledgements)

---

## Overview

This project analyzes historical vegetable price data. The dataset contains prices for various vegetables over a specific period, allowing us to perform statistical analysis and visualize price trends. By aggregating and visualizing data, we gain insights into price fluctuations, correlations, and seasonal trends for each vegetable.

**Dataset Source**: (https://www.kaggle.com/datasets/ksamiksha19/vegetable-prices)

---

## Features

- **Data Cleaning & Preprocessing**: Cleans and formats the dataset for analysis by removing missing values and converting columns to appropriate types.
- **Statistical Analysis**: Calculates various statistics, such as the mean, median, and price trends, for each vegetable.
- **Visualization**: Includes various plots (e.g., histograms, boxplots, and line plots) to visualize the distribution and trends in vegetable prices.
- **Correlation Analysis**: Investigates relationships between prices of different vegetables.
- **Outlier Detection**: Identifies outliers in the dataset and handles them appropriately for more accurate analysis.

---

## Installation

### Requirements

Before you begin, ensure you have the following installed:

- Python 3.x
- [Jupyter Notebook](https://jupyter.org/install) or [Google Colab](https://colab.research.google.com/) for running the code.
- Required Python packages (listed in `requirements.txt`).

### Steps to Install

1. Clone the repository:
   ```bash
   git clone https://github.com/maylouhw/Team1.git
   ```

2. Navigate to the project directory:
   ```bash
   cd vegetable-price-analysis
   ```

3. Create a virtual environment (optional but recommended):
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # Linux/macOS
   venv\Scripts\activate  # Windows
   ```

4. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```

---

## Usage

### Running the Analysis

1. Upload the dataset `prices.csv` to your project directory (ensure the file path is correct).
2. Open the Jupyter Notebook or Google Colab file and run each cell step-by-step.
3. The notebook will load the data, clean it, perform analysis, and visualize the results.

### Example Code:

```python
# Load dataset
import pandas as pd
data = pd.read_csv('prices.csv')

# Perform basic data analysis
average_prices = data.mean()
print(average_prices)

# Plotting the price distribution of each vegetable
import matplotlib.pyplot as plt
data.drop(columns=['Total Price']).plot(kind='box', vert=False)
plt.title('Box Plot of Vegetable Prices')
plt.show()
```

---

## Analysis

### 1. Data Cleaning & Preprocessing
The dataset undergoes initial cleaning to remove any missing or irrelevant data. Non-numeric columns are removed, and missing values are handled by imputation or removal.

### 2. Price Distribution
We calculate and visualize the distribution of prices for each vegetable. Histograms and box plots are used to show the spread of prices and identify outliers.

### 3. Price Trends
We look at monthly price fluctuations for each vegetable and identify any seasonal trends. Line plots are used to visualize how vegetable prices change month over month.

### 4. Correlation Analysis
By calculating the correlation matrix, we investigate how the prices of one vegetable are related to others. This helps in understanding if price changes for one vegetable influence the prices of others.

### 5. Summary Statistics
We calculate summary statistics for each vegetable's price, such as:
- Mean
- Median
- Standard Deviation
- Maximum and Minimum Prices

---

## Requirements

This project requires the following Python libraries:

- **pandas**: For data manipulation and analysis.
- **matplotlib**: For creating visualizations (plots and graphs).
- **seaborn**: For statistical data visualizations.
- **numpy**: For numerical operations.

To install these libraries, simply run:

```bash
pip install -r requirements.txt
```

Make sure that your environment is activated when you run the above command.
