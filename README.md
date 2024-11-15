# Brazil Demographics Data Mapping and Visualization

This project reads a dataset containing demographic data on Brazilian individuals, applies mappings to convert coded numbers into descriptive text, and prepares the data for analysis and visualization.

## Prerequisites

Ensure the following Python libraries are installed:

```bash
pip install pandas matplotlib seaborn
```

## Project Overview
The project follows these key steps:

Import Libraries: Use pandas for data manipulation, matplotlib.pyplot for plotting, and seaborn for enhanced data visualization.
Load Dataset: Load the dataset from a CSV file named brazil.csv using pandas.
Map Codes to Descriptive Text: Apply mappings to make the data more readable by replacing numeric codes with descriptive text labels.
Display Sample Data: Show the first 5 rows of the processed dataset for verification.
Code Details
1. Import Required Libraries
```
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
```
2. Read the CSV File
```
python
Code kopieren
df = pd.read_csv('brazil.csv')
```
