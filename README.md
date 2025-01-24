# MCM Contest Project: Analysis of Olympic Data

## Overview
This repository contains our work for the Mathematical Contest in Modeling (MCM) 2025. The project focuses on analyzing and modeling Olympic-related datasets to address the assigned problem.

## Project Structure
The repository is organized as follows:

```
- 2025_MCM_Problem_C.pdf       # Problem description and guidelines
- data_dictionary.csv          # Data dictionary for reference
- summerOly_athletes.csv       # Dataset containing athlete information
- summerOly_hosts.csv          # Dataset containing host city information
- summerOly_medal_counts.csv   # Dataset containing medal counts information
- summerOly_programs.csv       # Dataset containing event program details
- scratches/                   # Jupyter notebook and scratch files for data exploration
  - start_up.ipynb             # Initial data exploration and loading
```

## Datasets
### 1. **Athletes Data** (`summerOly_athletes.csv`)
Contains information about athletes, including:
- Name
- Sex
- Country (NOC)
- Year of participation
- City of participation
- Sport and Event
- Medal information

### 2. **Hosts Data** (`summerOly_hosts.csv`)
Contains details of Olympic host cities, including:
- Year of the games
- Host country and city

### 3. **Medal Counts Data** (`summerOly_medal_counts.csv`)
Contains data on the number of medals won by each country:
- Country (NOC)
- Gold, Silver, and Bronze medal counts

### 4. **Programs Data** (`summerOly_programs.csv`)
Contains details of Olympic events and programs:
- Year of the games
- Sport and Event details

## Initial Setup and Exploration
### Environment Setup
This project uses Python for data analysis and modeling. The following libraries are used:
- `pandas` for data manipulation
- (Optional) Libraries for visualization and modeling, such as `matplotlib`, `seaborn`, `scikit-learn`, etc.

### Instructions
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```
2. Install dependencies:
   ```bash
   pip install pandas matplotlib seaborn scikit-learn
   ```
3. Open the Jupyter notebook to explore the data:
   ```bash
   jupyter notebook scratches/start_up.ipynb
   ```

### Data Loading
The data files are loaded into dataframes as follows:
```python
import pandas as pd

# Load datasets
athletes_csv = pd.read_csv("2025_MCM_Problem_C_Data/summerOly_athletes.csv")
hosts_csv = pd.read_csv("2025_MCM_Problem_C_Data/summerOly_hosts.csv")
medal_counts_csv = pd.read_csv("2025_MCM_Problem_C_Data/summerOly_medal_counts.csv")
programs_csv = pd.read_csv("2025_MCM_Problem_C_Data/summerOly_programs.csv", encoding='windows-1252')
```

### Exploration
Preview the datasets using:
```python
# Print heads of each file
print("Athletes CSV Head:\n", athletes_csv.head())
print("Hosts CSV Head:\n", hosts_csv.head())
print("Medal Counts CSV Head:\n", medal_counts_csv.head())
print("Programs CSV Head:\n", programs_csv.head())
```

## Goals
1. **Data Cleaning:** Ensure data is properly formatted and consistent.
2. **Data Analysis:** Identify key trends and patterns.
3. **Modeling:** Build mathematical models to address the problem statement.
4. **Visualization:** Create clear and effective visuals to support the analysis.

## Team
Our team consists of motivated students passionate about mathematics and modeling. We will collaboratively explore the problem, analyze the data, and develop solutions.

## Contribution
If you have suggestions or improvements, feel free to fork the repository and create a pull request.

## License
This project is for educational and competition purposes. All rights to the data and problem statement belong to the MCM organizers.

---
Let's solve this problem and make our solution stand out in the contest!

