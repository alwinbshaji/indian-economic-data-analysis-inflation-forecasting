# Indian Economic Data Analysis & Inflation Forecasting

## Project Overview

This project analyses Indian economic data, focusing on Consumer Price Index (CPI), inflation trends and Reserve Bank of India (RBI) monetary policy rates.

The project uses Python for data cleaning, exploratory data analysis, data visualization, statistical analysis and basic machine learning. It also explores the relationship between CPI inflation and the RBI Repo Rate and develops a simple Linear Regression model to forecast future CPI index values.

The objective is to understand inflation patterns in India and gain practical experience working with official economic datasets.

## Objectives

- Analyse Consumer Price Index (CPI) trends in India.
- Study monthly changes in CPI.
- Compare inflation between Rural and Urban sectors.
- Analyse division-wise CPI trends.
- Explore historical RBI monetary policy rates.
- Examine the relationship between CPI inflation and the Repo Rate.
- Build a basic Linear Regression model for CPI index forecasting.

## Datasets Used

### 1. Consumer Price Index (CPI)

- Source: Ministry of Statistics and Programme Implementation (MoSPI), Government of India.
- Data period: January 2025 – October 2026.
- Original dataset dimensions: 31,460 rows and 15 columns.
- Filtered dataset: All India, Combined sector, CPI (General).
- Selected analysis variables: Date, CPI Index and Inflation.

### 2. RBI Policy Rates

- Source: Reserve Bank of India (RBI).
- Dataset contains historical monetary policy rates.
- Variables include:
  - Bank Rate
  - Repo Rate
  - Reverse Repo Rate
  - Standing Deposit Facility (SDF)
  - Marginal Standing Facility (MSF)
  - Cash Reserve Ratio (CRR)
  - Statutory Liquidity Ratio (SLR)

## Technologies and Libraries

- Python
- Google Colab
- Pandas – Data manipulation and cleaning
- NumPy – Numerical operations
- Matplotlib – Data visualization
- Seaborn – Statistical visualization
- Scikit-learn – Machine learning and model evaluation
- OpenPyXL – Excel file handling

## Project Workflow

### 1. Data Collection and Cleaning

- Imported CPI and RBI policy-rate datasets.
- Inspected dataset structure, columns and data types.
- Checked missing values and duplicate records.
- Converted date columns into datetime format.
- Converted economic variables into numeric format.
- Handled missing policy-rate entries using forward filling.
- Filtered CPI data for All India, Combined sector and CPI (General).

### 2. CPI Exploratory Data Analysis

- Analysed CPI index movements over time.
- Calculated monthly percentage changes.
- Studied inflation trends.
- Identified higher and lower monthly changes.
- Visualized CPI trends using line charts.

### 3. Division-wise CPI Analysis

- Examined CPI movements across different divisions.
- Calculated monthly percentage changes for each division.
- Compared average monthly changes.
- Identified divisions with higher and lower changes.
- Studied variation in division-wise CPI movements.

### 4. Rural vs Urban Inflation Analysis

Compared CPI and inflation trends across Rural, Urban and Combined sectors.

Key observations for October 2026:

| Indicator | Value |
|---|---:|
| Rural CPI Index | 110.73 |
| Urban CPI Index | 109.22 |
| Combined CPI Index | 110.05 |
| Rural Inflation | 6.63% |
| Urban Inflation | 5.41% |
| Combined Inflation | 6.09% |

The analysis showed higher inflation in the Rural sector than in the Urban sector for October 2026.

### 5. RBI Monetary Policy Rate Analysis

- Examined historical RBI policy-rate movements.
- Calculated descriptive statistics such as mean, standard deviation, minimum and maximum.
- Visualized changes in major interest rates.
- Analysed Repo Rate movements.
- Identified increases and decreases in the Repo Rate.

The downloaded RBI dataset contained 70 recorded Repo Rate changes, including 35 increases and 35 decreases.

### 6. CPI Inflation and Repo Rate Correlation

Merged monthly CPI inflation data with RBI Repo Rate data using the latest effective policy rate available on or before each month's end.

Calculated the Pearson correlation coefficient to explore the relationship between CPI inflation and the Repo Rate.

**Correlation coefficient: 0.622**

This indicates a moderate positive correlation in the selected observations. However, correlation does not imply causation.

The analysis uses only 10 observations because year-on-year inflation values were unavailable for the first 12 months.

### 7. CPI Index Forecasting Using Linear Regression

Developed a basic Linear Regression model to analyse the CPI index trend and generate short-term exploratory forecasts.

**Model approach:**

- Independent variable: Numerical time sequence.
- Dependent variable: CPI Index.
- Total observations: 22 months.
- Training dataset: First 18 months.
- Testing dataset: Last 4 months.
- Forecast horizon: Next 3 months.

**Model equation:**

CPI Index = Intercept + (Coefficient × Time)

The model was evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)

After evaluation, the model was trained again using all 22 observations to forecast the next three months.

The forecast is a simple trend-based estimate and is not an official CPI prediction.

## Key Findings

- The Combined CPI Index reached 110.05 in October 2026.
- Combined inflation reached 6.09% in October 2026.
- Rural inflation (6.63%) was higher than Urban inflation (5.41%) in October 2026.
- The correlation between CPI inflation and the Repo Rate was 0.622.
- A Linear Regression model was developed to study the CPI index trend and generate three-month exploratory forecasts.

## Limitations

- The CPI analysis is based on only 22 monthly observations.
- Year-on-year inflation data is available for only 10 observations.
- The correlation analysis has a limited sample size.
- Simple Linear Regression does not account for seasonality, external economic factors or complex inflation dynamics.
- The forecast results should not be considered official economic predictions.
- The monthly alignment of CPI and RBI policy rates is a simplified analytical approach.

## Skills Demonstrated

- Data Collection and Preprocessing
- Data Cleaning
- Exploratory Data Analysis (EDA)
- Statistical Analysis
- Data Visualization
- Time-Series Trend Analysis
- Correlation Analysis
- Linear Regression
- Model Evaluation
- Working with Government Economic Data

## Project Structure

```text
Indian-Economic-Data-Analysis/
│
├── Data_collection.ipynb
├── README.md
```

## How to Run the Project

1. Clone or download this repository.
2. Open Google Colab.
3. Upload `Data_collection.ipynb`.
4. Upload the required CPI and RBI Excel datasets to your Google Drive.
5. Update the dataset file paths in the notebook if necessary.
6. Run the notebook cells sequentially.

## Conclusion

This project provided practical experience in analysing Indian economic data using Python. It explored CPI and inflation trends, compared Rural and Urban inflation, examined RBI monetary policy rates and investigated their relationship with CPI inflation.

A basic Linear Regression model was also implemented to study CPI index trends and generate short-term exploratory forecasts.

The project helped develop practical skills in data preprocessing, exploratory data analysis, statistical analysis, visualization and introductory machine learning while improving understanding of Indian economic indicators.

---

**Project Category:** Data Science | Economic Data Analysis | Machine Learning

**Developed using:** Python and Google Colab
