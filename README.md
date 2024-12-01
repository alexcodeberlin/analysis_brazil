# Brazil Demographics Data Mapping and Visualization

This project reads a dataset containing demographic data on Brazilian individuals. It prepares the data for analysis and visualization.<br> 
The following dataset is used https://www.kaggle.com/datasets/patrickgomes/determinants-of-poverty-in-brazil. For any further details please check out.
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
2. Read the CSV File - copy csv file into root folder 
```
python
Code kopieren
df = pd.read_csv('brazil.csv')
```

About Dataset
This dataset contains data from 2020 on more than 20,000 Brazilian individuals and their characteristic

Meaning of dataset variables:
woman:
1 - female
0 - male

age: person's age
education:
1 - No education and less than 1 year of study
2 - Incomplete elementary or equivalent
3 - Complete fundamental or equivalent
4 - Incomplete audio or equivalent
5 - Complete audio or equivalent
6 - Incomplete higher or equivalent
7 - Superior complete

work:
1 - Agriculture, livestock, forestry, fisheries and aquaculture
2 - General industry
3 - Construction
4 - Trade, repair of motor vehicles and motorcycles
5 - Transport, storage and mail
6 - Accommodation and food
7 - Information, communication and financial, real estate, professional and administrative
8 - Public administration, defense and social security
9 - Education, human health and social services
10 - Other Services
11 - Home Services
12 - Ill-defined activities

metropolitan_area
1 - lives in metropolitan region
0 - does not live in a metropolitan region

not_white
1 - not white (black, brown, yellow and indigenous)
0 - white

urban
1 -lives in urban areas
0 - I live in the countryside

work permit
0 - does not have a work permit
1 - has a work permit
2 - other situations, employer, civil servant

poverty: individuals who received less than BRL 457 in 2020
1 - was poor in 2020 interview
0 - not poor in 2020 interview
