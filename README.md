# Restaurant Tips Analysis & Prediction
**Author:** Denise Aoko Owino  
**Context:** Technical assessment for Data Specialist Role.

## Project Overview
This analysis explores the relationship between total bills and tip amounts using a Linear Regression model to identify key drivers of tip outcomes.

## Technical Requirements
The analysis was conducted within a **Jupyter Notebook** environment to ensure reproducibility and transparency. The following Python libraries were utilized for the end-to-end data lifecycle:
*   **Pandas & NumPy:** For data wrangling, cleaning, and type conversion.
*   **Scikit-Learn:** For data splitting (Train/Test) and the implementation of the Linear Regression model.
*   **Matplotlib & Seaborn:** For exploratory data analysis (EDA) and generating executive-ready visualizations.

## Run Instructions
To replicate this analysis, follow the steps below using the Anaconda distribution:

1. Environment: Ensure you have the latest version of Anaconda installed.

2. Launch: Open the Anaconda Navigator and launch Jupyter Notebook.

3. Navigation: Browse to the project root directory and open Analysis_Notebook.ipynb.

4. Execution: From the top menu, select Cell > Run All to generate the regression model results and performance metrics (RMSE/R²).

## Key Findings
### Model Performance
The predictive model was evaluated using standard statistical metrics to ensure analytical rigor:
*   **R-squared (R²):** [0.52] — This indicates that the model explains approximately [52%] of the variance in tip amounts.
*   **RMSE:** [1.08] — On average, the model's predictions deviate from actual tips by [$1.08].
*   The coefficient for Size (0.27) is numerically higher than Total Bill (0.08), the Total Bill remains the most influential factor due to its higher scale of variance. Specifically, the model predicts an 8-cent tip increase per dollar spent, versus a 27-cent increase per additional person. This indicates that while larger groups tip slightly more per head, the sheer volume of the bill is the primary driver of the final tip amount.

### Strategic Insights
*   **Most Influential Variable:** The **Total Bill** was identified as the primary driver of tip outcomes. For every additional dollar spent on the bill, the tip increases by approximately [$0.08].
*   **Temporal Trends:** Exploratory analysis via box plots highlighted that **Sundays** and **Fridays** show higher median tips and **Saturdays** show greater variance(outliers), suggesting weekend service as a key strategic focal point for maximizing outcomes.
