# Water Quality Data Analysis Project

## Overview
This project analyzes water quality data collected from various locations in Andhra Pradesh, India. The dataset includes parameters such as temperature, dissolved oxygen (D.O.), pH levels, conductivity, biochemical oxygen demand (B.O.D.), and coliform counts. The goal is to assess water quality and identify significant trends or issues.

## Dataset
The dataset used in this project is a CSV file containing the following columns:

- **STATION CODE**: Unique identifier for each sampling station.
- **LOCATIONS**: Names of the locations where samples were collected.
- **STATE**: The state where the sampling took place.
- **TEMPERATURE (°C)**: Minimum, maximum, and mean temperatures recorded.
- **D.O. (mg/l)**: Minimum, maximum, and mean dissolved oxygen levels.
- **pH**: Minimum, maximum, and mean pH levels.
- **CONDUCTIVITY (µmhos/cm)**: Minimum, maximum, and mean conductivity measurements.
- **B.O.D. (mg/l)**: Minimum, maximum, and mean biochemical oxygen demand.
- **NITRATE-N + NITRITE-N (mg/l)**: Minimum, maximum, and mean values for nitrate and nitrite levels.
- **FECAL COLIFORM (MPN/100ml)**: Minimum, maximum, and mean fecal coliform counts.
- **TOTAL COLIFORM (MPN/100ml)**: Minimum, maximum, and mean total coliform counts.

## Features
The notebook includes the following key features:

1. **Data Loading**: Load the dataset using Pandas for analysis.
2. **Data Exploration**: Initial exploration of the dataset to understand its structure and contents.
3. **Feature Engineering**:
   - Creation of rolling averages for temperature to smooth out fluctuations.
   - Interaction features between pH levels and D.O. concentrations to explore relationships.
   - Binning of temperature values into categorical ranges for better analysis.
   - Lag features to capture temporal dependencies in D.O. levels.
   - Normalization of conductivity values to ensure uniform scaling across features.

4. **Visualization**: Utilize Plotly for interactive visualizations of water quality parameters.

## Requirements
To run this notebook successfully, ensure you have the following Python libraries installed:

- `pandas`
- `numpy`
- `plotly`

You can install these libraries using pip:

```bash
pip install pandas numpy plotly
