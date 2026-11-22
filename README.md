# Indian Economic Data Analysis & Inflation Forecasting

## Project Overview

This project focuses on analysing Indian economic data, particularly the Consumer Price Index (CPI), to understand inflation trends and changes in the prices of different goods and services.

Using Python and Data Science techniques, the project explores CPI data, identifies monthly and yearly inflation patterns, compares price changes across different divisions, and visualizes important economic trends.

The project uses real-world CPI data published by the Ministry of Statistics and Programme Implementation (MoSPI), Government of India.

## Objectives

- Analyse Indian Consumer Price Index (CPI) data.
- Understand monthly and year-on-year inflation trends.
- Identify the highest and lowest CPI changes.
- Compare price index changes across different divisions.
- Study correlations between CPI variables.
- Visualize economic trends using charts and graphs.
- Explore the potential for inflation forecasting.

## Dataset Information

**Dataset:** Consumer Price Index (CPI), India

**Source:** Ministry of Statistics and Programme Implementation (MoSPI)

**Website:** https://esankhyiki.mospi.gov.in/catalogue-main/catalogue?product=CPI

**Base Year:** 2024 = 100

**Data Period:** January 2025 – October 2026

**Geographical Coverage:** All India

**Sector:** Combined (Rural + Urban)

The analysis focuses on the All India Combined CPI data.

## Technologies Used

- Python
- Google Colab
- Pandas – Data manipulation and analysis
- NumPy – Numerical calculations
- Matplotlib – Data visualization
- Seaborn – Statistical visualization

## Project Workflow

### 1. Data Collection
Collected CPI data from the official MoSPI eSankhyiki portal.

### 2. Data Cleaning and Preprocessing
- Inspected dataset structure and dimensions.
- Checked missing values.
- Checked duplicate records.
- Selected relevant columns.
- Filtered All India Combined CPI data.
- Converted month and year into datetime format.
- Sorted observations chronologically.

### 3. Exploratory Data Analysis (EDA)
- Examined descriptive statistics.
- Analysed CPI index trends.
- Studied monthly percentage changes.
- Calculated year-on-year CPI changes.
- Identified highest and lowest monthly movements.

### 4. Correlation Analysis
Examined relationships between:
- CPI Index
- Monthly Percentage Change
- Year-on-Year Change

Visualized the correlation matrix using a heatmap.

### 5. Inflation Validation
Calculated year-on-year CPI changes using a 12-month percentage change and compared them with officially published inflation figures.

The mean absolute difference between the calculated and published values was approximately 0.00423 percentage points for the available overlapping observations.

### 6. Division-Wise Analysis
Compared CPI trends across 12 divisions, including:

- Food and Beverages
- Clothing and Footwear
- Housing and Utilities
- Health
- Transport
- Education Services
- Restaurants and Accommodation
- Personal Care and Miscellaneous Services

Calculated average CPI index values and cumulative percentage changes for each division.

### 7. Data Visualization
Created visualizations to understand:
- CPI index trends
- Inflation trends
- Monthly percentage changes
- Correlation between CPI variables
- Division-wise CPI comparisons

## Key Findings

Based on the current dataset (January 2025 – October 2026):

- The All India Combined CPI index reached 110.05 in October 2026.
- Published CPI inflation reached 6.09% in October 2026.
- The highest monthly CPI percentage increase was approximately 1.03% in June 2026.
- The lowest monthly CPI percentage change was approximately -0.34% in February 2025.
- Personal care and miscellaneous services recorded the highest cumulative CPI index increase, approximately 20.84%.
- Information and communication recorded the lowest cumulative CPI index increase, approximately 3.30%.

These findings describe changes in the CPI index during the selected period and should not be interpreted as individual product price changes.

## Repository Structure

```text
indian-economic-data-analysis-inflation-forecasting/
│
├── Data_collection.ipynb
├── README.md
└── requirements.txt
```

## How to Run the Project

1. Clone this repository:

```bash
git clone https://github.com/alwinbshaji/indian-economic-data-analysis-inflation-forecasting.git
```

2. Open the project folder.

3. Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn openpyxl
```

4. Open `Data_collection.ipynb` using Google Colab or Jupyter Notebook.

5. Download the CPI dataset from the official MoSPI website.

6. Upload the dataset to your Google Drive and update the dataset file path in the notebook.

7. Run the notebook cells sequentially.

## Current Limitations

- The current dataset contains only 22 monthly observations.
- A longer historical dataset is needed for reliable time-series forecasting.
- Correlation does not establish causation.
- Monthly CPI percentage changes are different from official year-on-year inflation rates.

Forecasting is a planned extension of this project and should not be considered a validated prediction at the current stage.

## Future Improvements

- Include additional historical CPI data.
- Perform state-wise and rural-versus-urban comparisons.
- Explore time-series forecasting models.
- Evaluate forecasting performance using suitable metrics.
- Develop an interactive inflation dashboard.
- Incorporate additional Indian economic indicators.

## Author

**Alwin B Shaji**

B.Tech Computer Science and Engineering

GitHub: https://github.com/alwinbshaji

---

*This project is developed for learning and portfolio purposes to explore real-world economic data analysis using Python and Data Science.*
