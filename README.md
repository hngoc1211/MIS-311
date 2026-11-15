# Life Expectancy – Exploratory Data Analysis

## 1. Project Overview

This project explores life expectancy and mortality indicators across countries using Exploratory Data Analysis (EDA).

The main purpose is to identify patterns, relationships, and regional differences in life expectancy and understand how mortality indicators are associated with population health.

### Objectives

- Understand the dataset structure and variables.
- Identify and handle missing values.
- Detect and remove duplicate records.
- Calculate descriptive statistics.
- Compare average life expectancy across regions.
- Examine the relationship between adult mortality and life expectancy.
- Develop two key insights supported by data and visualizations.

## 2. Dataset Description

- **Dataset:** Life Expectancy
- **Initial observations:** 182
- **Observations after duplicate removal:** 179
- **Number of columns:** 6
- **Source:** Dataset provided by the lecturer for MIS 311, Eastern International University. The original source is not stated in the supplied file.

### Variables

| Variable | Description |
|---|---|
| Country | Name of the country |
| Region | Geographical region |
| Infant_deaths | Infant mortality indicator |
| Under_five_deaths | Under-five mortality indicator |
| Adult_mortality | Adult mortality indicator |
| Life_expectancy | Average life expectancy (years) |

## 3. Data Cleaning and Preparation

Before conducting the analysis, I examined the dataset for missing values and duplicate records using Microsoft Excel.

### Duplicate Records

I identified 3 duplicate rows associated with Albania, Brunei Darussalam, and Colombia.

After removing these duplicates, the dataset decreased from 182 to 179 unique country observations.

### Missing Values

I identified 3 missing values:

- Bangladesh: Under_five_deaths
- Ghana: Adult_mortality
- Iraq: Adult_mortality

I retained these countries and left the missing cells blank instead of deleting the entire rows. This preserves the available information for analysis.

Blank cells are excluded from calculations that require numerical values. Therefore, the valid observation count differs across variables.

## 4. Descriptive Statistics

I calculated descriptive statistics for the four numerical variables using Microsoft Excel.

| Statistic | Infant_deaths | Under_five_deaths | Adult_mortality | Life_expectancy |
|---|---:|---:|---:|---:|
| Mean | 30.36 | 42.85 | 191.91 | 68.86 |
| Median | 19.37 | 23.01 | 162.59 | 71.51 |
| Standard Deviation | 26.73 | 43.02 | 112.12 | 9.20 |
| Minimum | 2.38 | 3.00 | 57.71 | 45.61 |
| Maximum | 115.72 | 178.73 | 572.97 | 82.46 |
| Count | 179 | 178 | 177 | 179 |

The mean life expectancy (68.86 years) is lower than the median (71.51 years). This suggests that some countries with relatively low life expectancy pull the overall average downward.

## 5. Data Visualizations

### 5.1 Average Life Expectancy by Region

This column chart compares average life expectancy across nine geographical regions.

Africa has the lowest average life expectancy, while North America and the European Union have the highest averages.

![Average Life Expectancy by Region](Average%20Life%20Expectancy%20by%20Region..png)

### 5.2 Adult Mortality vs. Life Expectancy

This scatter plot illustrates the relationship between adult mortality and life expectancy across countries.

The downward pattern indicates that countries with higher adult mortality tend to have lower life expectancy.

![Adult Mortality vs. Life Expectancy](Relationship%20between%20Adult%20Mortality%20and%20Life%20Expectancy..png)

## 6. Key Insights

### Insight 1: Significant Regional Differences in Life Expectancy

North America has the highest average life expectancy at 77.84 years (n = 3), closely followed by the European Union at 77.72 years (n = 27), while Africa has the lowest at 57.85 years (n = 51), an approximately 20-year gap. These differences may reflect variations in healthcare access, economic development, and living conditions. Regions with lower life expectancy may therefore need greater priority when allocating public health resources.

### Insight 2: Strong Negative Relationship Between Adult Mortality and Life Expectancy

The Pearson correlation coefficient between adult mortality and life expectancy is -0.94757 (approximately -0.95), based on 177 countries with complete data, indicating a very strong negative relationship. Adult mortality can therefore serve as an important indicator when examining population health. However, correlation does not establish causation, as factors such as income and healthcare quality may influence both variables.

## 7. Conclusion

This analysis reveals two important findings. First, average life expectancy differs substantially across geographical regions, with an approximately 20-year gap between Africa and North America. Second, adult mortality has a very strong negative relationship with life expectancy.

The regional averages should be interpreted with caution, particularly for regions with small sample sizes, such as North America (n = 3).

Through this project, I developed practical experience in data cleaning, descriptive statistics, PivotTables, data visualization, and interpreting analytical results using Microsoft Excel.

## 8. Tools and Techniques

- Microsoft Excel
- PivotTables
- Descriptive Statistics
- Excel Column Charts
- Scatter Plots
- Pearson Correlation

## 9. Files in This Repository

| File | Description |
|---|---|
| `05_Life Expectancy.xlsx` | Original dataset provided by the lecturer |
| `05_Life Expectancy_clean.xlsx` | Workbook containing cleaned data and analysis |
| `Average Life Expectancy by Region..png` | Average life expectancy by region |
| `Relationship between Adult Mortality and Life Expectancy..png` | Adult mortality vs. life expectancy |

## Author

**Hồng Ngọc**

Business Administration Student – Business Analytics  
Eastern International University (EIU)

[GitHub Profile](https://github.com/hngoc1211)
