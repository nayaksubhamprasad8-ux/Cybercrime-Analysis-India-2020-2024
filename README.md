# Cybercrime Trends and State-wise Analysis in India (2020–2024)

## Overview

This project analyzes registered cybercrime cases in India from 2020 to 2024 using Python. It explores yearly trends, compares state and Union Territory (UT) case counts, and examines changes across different cybercrime heads.

The objective is to identify patterns in the available data through data cleaning, exploratory data analysis (EDA), and visualization.

## Objectives

- Analyze the year-wise trend in registered cybercrime cases across India.
- Identify states and UTs with the highest registered case counts.
- Compare state-wise case counts between 2020 and 2024.
- Calculate absolute and percentage changes in registered cases.
- Identify crime heads with high case counts and substantial changes over time.
- Visualize trends using Matplotlib and Seaborn.
- Present data-driven findings while acknowledging the limitations of the dataset.

## Dataset

The project uses an Excel workbook containing two sheets:

### 1. State/UT-wise Data

Contains registered cybercrime cases for individual states and Union Territories from 2020 to 2024, along with summary rows for states, UTs, and all India.

### 2. Crime-head-wise Data

Contains yearly case counts for individual crime heads and aggregate categories for the same period.

**Time period:** 2020–2024  
**Geographical coverage:** Indian states and Union Territories  
**Data format:** Excel (`.xlsx`)

The analysis uses the provided dataset and does not independently verify the underlying records.

## Tools and Technologies

- **Python** — analysis and scripting
- **Pandas** — data loading, cleaning, transformation, and tabular analysis
- **NumPy** — numerical calculations
- **Matplotlib** — data visualization
- **Seaborn** — statistical charts and visual comparisons
- **OpenPyXL** — Excel file support
- **Jupyter Notebook** — interactive analysis and documentation

## Project Structure

```text
cybercrime-analysis-india-2020-2024/
├── Data/
│   └── Cybercrime_Annexure_Data.xlsx
├── cybercrime_analysis.ipynb
└── README.md
```

## Analysis Performed

### 1. Data Loading and Validation

- Loaded both sheets from the Excel workbook using Pandas.
- Separated individual states and UTs from summary rows.
- Checked for duplicate region names and missing values.
- Validated that the sum of state and UT counts matched the reported all-India totals for each year.

### 2. National Trend Analysis

- Calculated yearly totals.
- Measured year-on-year absolute changes and percentage growth.
- Visualized the national trend from 2020 to 2024.

### 3. State-wise Analysis

- Ranked states and UTs by registered cases in 2024.
- Compared case counts between 2020 and 2024.
- Calculated absolute and percentage changes.
- Identified regions with the largest increases and decreases.

### 4. Crime-head Analysis

- Ranked individual crime heads by registered cases in 2024.
- Calculated their share of the national total.
- Compared crime-head counts between 2020 and 2024.
- Visualized trends for selected major crime heads.

### 5. Data Visualization

The project uses line charts and bar charts to communicate yearly trends, state-wise comparisons, and changes in individual crime heads.

## Key Findings

Based on the provided dataset:

- Total registered cybercrime cases increased from **50,035 in 2020 to 101,928 in 2024**, an increase of approximately **103.71%**.
- The highest year-on-year growth rate occurred in **2023**, at approximately **31.15%**.
- **Telangana** recorded the highest number of cases in 2024, with **27,230**, followed by **Karnataka**, with **21,993**.
- Telangana recorded the largest absolute increase between 2020 and 2024, rising by **22,206 cases**.
- The crime-head data can be used to investigate the contributions of categories such as fraud, cheating, and computer-related offences.

These findings describe registered case counts in the supplied dataset. They should not be interpreted as proof of the underlying causes of changes in cybercrime.

## Limitations

- The analysis is limited to the provided data for 2020–2024.
- Registered cases do not necessarily represent the total incidence of cybercrime.
- The dataset does not independently establish why registered cases increased or decreased.
- Population size, internet usage, digital payment adoption, reporting practices, and enforcement changes are not included as explanatory variables.
- Percentage changes can be misleading when the baseline count is small or zero.
- Individual crime heads and aggregate categories may overlap. Summary rows must be excluded when ranking individual crime heads to avoid double-counting.
- The analysis identifies associations and trends; it does not establish causation.


### 1. Install dependencies

```bash
python -m pip install pandas numpy matplotlib seaborn openpyxl jupyter
```

### 2. Launch Jupyter Notebook

```bash
python -m jupyter notebook
```

### 3. Run the analysis

Open `cybercrime_analysis.ipynb` and execute the notebook cells in order.

Ensure that `Cybercrime_Annexure_Data.xlsx` is located at the path expected by the notebook.

## Future Improvements

- Add population-adjusted case rates to enable fairer comparisons between states.
- Incorporate internet penetration and digital payment adoption data to explore possible explanatory factors.
- Improve visualizations with clearer annotations and consistent formatting.
- Add automated data-quality checks and reproducible analysis scripts.
- Develop an interactive dashboard for exploring state-wise and year-wise trends.

## Conclusion

This project demonstrates how Python-based data analysis can be used to clean, validate, explore, and visualize registered cybercrime data. It provides a foundation for further research into geographical patterns and changes in recorded cybercrime cases in India.

---

## Reference 
Data :- https://www.pib.gov.in/PressReleasePage.aspx?PRID=2287039&utm_source=chatgpt.com&reg=48&lang=2

**Author:** Subham Prasad Nayak

**Project:** Cybercrime Trends and State-wise Analysis in India (2020–2024)
