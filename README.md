# Do Lower-Income Adults Have Higher Obesity Rates?
### A Public Health Data Analysis Using CDC Surveillance Data

## Project Overview

This project examines the relationship between income and adult obesity prevalence in the United States using publicly available data from the Centers for Disease Control and Prevention (CDC).

The goal was to investigate whether obesity prevalence differs across income groups and explore how socioeconomic factors relate to public health outcomes.

## Research Question

Do adults in lower-income groups experience higher obesity rates than adults in higher-income groups?

**Hypothesis:** Adults in lower-income brackets will have higher obesity prevalence than adults in higher-income brackets.

## Dataset

- **Source:** CDC Nutrition, Physical Activity, and Obesity – Behavioral Risk Factor Surveillance System (BRFSS)
- **Access:** [CDC Open Data Portal](https://data.cdc.gov/api/views/hn4x-zwk7/rows.csv?accessType=DOWNLOAD)
- **Population:** U.S. adults aged 18 and older
- **Key variables:** Obesity prevalence, income category, year, and geographic location

The analysis uses national estimates stratified by income, as well as overall estimates for examining trends over time and differences across states.

## Tools & Technologies

- Python
- Pandas
- NumPy
- SciPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Methods

**1. Data Cleaning and Preparation**
- Imported CDC surveillance data using Pandas.
- Filtered records to focus on adult obesity prevalence.
- Converted obesity estimates to numeric values and handled missing observations.
- Organized records by income group, year, and geographic location.

**2. Exploratory Data Analysis**
Created visualizations to examine:
- National adult obesity trends over time.
- Obesity prevalence across U.S. states in the latest available year.
- Obesity prevalence across income categories.

Used Kernel Density Estimation (KDE) curves to explore the distributions of obesity estimates.

**3. Statistical Analysis**
- Calculated descriptive statistics, including means, medians, ranges, and standard deviations.
- Conducted a one-way ANOVA to examine differences in mean obesity estimates across income groups.
- Performed a chi-square test to examine the relationship between combined income tiers and binary obesity categories.

## Key Findings

**Obesity Prevalence Across Income Groups**

The descriptive analysis showed an inverse pattern between income and obesity prevalence:

- Less than $15,000: 35.8%
- $15,000–$24,999: 34.7%
- $25,000–$34,999: 33.2%
- $35,000–$49,999: 32.6%
- $50,000–$74,999: 32.1%
- $75,000 or greater: 28.0%

The difference between the lowest and highest income groups was approximately 7.8 percentage points.

**One-Way ANOVA**

- F-statistic: 20.9856
- P-value: less than 0.001
- Result: Statistically significant differences in mean obesity estimates across income groups.

**Chi-Square Test**

- Chi-square statistic: 2.3810
- Degrees of freedom: 1
- P-value: 0.1228
- Result: The association was not statistically significant using the combined income and obesity categories in this test.

Together, these results suggest differences across the full income categories, although the binary comparison did not reach statistical significance.

## Public Health Implications

The findings highlight the importance of examining socioeconomic factors when studying obesity and population health. Differences in income may reflect broader disparities in access to nutritious food, healthcare, and opportunities for physical activity.

Understanding these patterns can help inform public health research and interventions addressing health inequalities.

## Limitations

- The analysis uses observational surveillance estimates and cannot establish causation.
- Income categories are broad and may not capture differences within income groups.
- The analysis includes a "Data not reported" category in the descriptive statistics.
- Self-reported BMI data may introduce measurement error.
- The statistical tests are based on grouped surveillance estimates, not individual-level participant records. Their assumptions and interpretation should be considered when drawing conclusions.

## Project Files

- `income_analysis.ipynb` – Jupyter Notebook containing data preparation, exploratory analysis, visualizations, and statistical testing.

## Skills Demonstrated

- Public health data analysis
- Data cleaning and preprocessing
- Exploratory data analysis
- Statistical hypothesis testing
- Data visualization
- Python programming
- Interpretation of population health data

---

**Author:** Bella MacPherson  
**Institution:** The George Washington University  
**Program:** B.S. in Health Data Science
