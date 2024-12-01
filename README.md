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



## About Dataset
This dataset contains data from 2020 on more than 20,000 Brazilian individuals and their characteristics.

Categorical Data: Gender(male female)
Ordinal Data Education levels (No education, Primary, Secondary, Higher)
Continuous Data: Age

### Meaning of Dataset Variables:

- **woman**:  
  - `1` - Female  
  - `0` - Male  

- **age**:  
  Person's age  

- **education**:  
  - `1` - No education and less than 1 year of study  
  - `2` - Incomplete elementary or equivalent  
  - `3` - Complete fundamental or equivalent  
  - `4` - Incomplete secondary or equivalent  
  - `5` - Complete secondary or equivalent  
  - `6` - Incomplete higher or equivalent  
  - `7` - Superior complete  

- **work**:  
  - `1` - Agriculture, livestock, forestry, fisheries, and aquaculture  
  - `2` - General industry  
  - `3` - Construction  
  - `4` - Trade, repair of motor vehicles and motorcycles  
  - `5` - Transport, storage, and mail  
  - `6` - Accommodation and food  
  - `7` - Information, communication, financial, real estate, professional, and administrative services  
  - `8` - Public administration, defense, and social security  
  - `9` - Education, human health, and social services  
  - `10` - Other services  
  - `11` - Home services  
  - `12` - Ill-defined activities  

- **metropolitan_area**:  
  - `1` - Lives in a metropolitan region  
  - `0` - Does not live in a metropolitan region  

- **non_white**:  
  - `1` - Not white (includes black, brown, yellow, and indigenous)  
  - `0` - White  

- **urban**:  
  - `1` - Lives in urban areas  
  - `0` - Lives in rural areas  

- **work_permit**:  
  - `0` - Does not have a work permit  
  - `1` - Has a work permit  
  - `2` - Other situations (e.g., employer, civil servant)  

- **poverty**:  
  Individuals who received less than BRL 457 in 2020.  
  - `1` - Was poor in the 2020 interview  
  - `0` - Was not poor in the 2020 interview  







