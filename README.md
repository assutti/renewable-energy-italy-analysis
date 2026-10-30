# Renewable Energy in Italy — Regional and Temporal Analysis

This project analyzes renewable electricity production in Italy, focusing on temporal trends, regional differences, and the contribution of different renewable energy sources.

The project uses public data provided by Terna.
## Project Objectives

The main objectives of this project are to:

- Analyze the evolution of renewable electricity production in Italy from 2000 to 2024.
- Compare renewable energy production across Italian regions.
- Examine the contribution of different renewable energy sources.
- Identify long-term trends using statistical analysis.
- Apply a simple linear regression model to describe the historical production trend.
- Build an interactive Power BI dashboard to communicate the main findings.

## Data Source

The analysis is based on public electricity production data provided by **Terna**, the Italian transmission system operator.

The dataset covers the period **2000–2024** and includes information on:

- Year
- Italian region
- Renewable energy source
- Electricity production (GWh)

The raw data is collected and processed in the first notebook, producing a cleaned dataset used throughout the subsequent analysis.

## Project Workflow

The project follows a complete data analysis workflow:

1. **Data Collection** — acquisition and preparation of renewable electricity production data from Terna.
2. **Exploratory Data Analysis** — exploration of temporal, regional, and energy-source patterns.
3. **Data Visualization** — creation of visualizations to highlight the main trends in renewable production.
4. **Statistical Analysis** — calculation of descriptive statistics and long-term growth indicators.
5. **Machine Learning** — application of linear regression to model the historical trend in renewable electricity production.
6. **Power BI Dashboard** — development of an interactive dashboard summarizing the main results and analytical insights.


## Technologies & Tools

- **Python** — data collection, cleaning, analysis, visualization, and machine learning
- **Pandas** — data manipulation and transformation
- **NumPy** — numerical analysis
- **Matplotlib & Seaborn** — exploratory data visualization
- **Scikit-learn** — linear regression and model evaluation
- **Power BI** — interactive dashboard development and DAX measures
- **Jupyter Notebook** — analytical workflow and documentation
- **Git & GitHub** — version control and project repository management

## Key Findings

- Renewable electricity production in Italy increased from approximately **50.98 TWh in 2000** to **134.36 TWh in 2024**.
- This corresponds to an overall growth of approximately **163.56%** between 2000 and 2024.
- The compound annual growth rate (**CAGR**) over the period was approximately **4.12%**.
- Average annual renewable production was approximately **86.01 TWh**.
- The historical trend shows an estimated linear increase of approximately **3.77 TWh per year**.
- The linear regression model achieved an **R² of approximately 0.85**, indicating that the long-term linear trend explains a substantial share of the historical variation.
- The model's **RMSE was approximately 11.41 TWh**.

## Power BI Dashboard

The project includes a two-page interactive Power BI dashboard designed to communicate the main analytical results.

### Overview

The first page provides a high-level view of renewable electricity production in Italy, including:

- Production in 2000 and 2024
- Overall growth between 2000 and 2024
- Historical production trend
- Production by renewable energy source
- Top regions by renewable production
- Top regions by production growth

### Statistics & ML

The second page focuses on statistical and machine learning results, including:

- CAGR
- Average annual production
- Annual production standard deviation
- Linear trend coefficient
- R²
- RMSE
- Comparison between actual production and the fitted linear regression trend

The Power BI file is available in the `powerbi/` directory.

## Repository Structure

renewable-energy-italy-analysis/
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
│   ├── 01_data_collection.ipynb
│   ├── 02_exploratory_analysis.ipynb
│   ├── 03_visualization.ipynb
│   ├── 04_statistical_analysis.ipynb
│   └── 05_machine_learning.ipynb
├── powerbi/
│   └── Renewable_Energy_Italy_Dashboard.pbix
├── src/
├── .gitignore
└── README.md


## Machine Learning

A simple linear regression model was applied to annual renewable electricity production from 2000 to 2024.

The model was used to quantify and visualize the long-term historical trend rather than to produce future forecasts.

Main model results:

- **Trend coefficient:** approximately 3,768 GWh/year
- **R²:** approximately 0.85
- **RMSE:** approximately 11,415 GWh

The complete machine learning workflow is available in `notebooks/05_machine_learning.ipynb`.