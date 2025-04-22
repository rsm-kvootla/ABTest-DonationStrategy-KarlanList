# Donation Experiment Analysis

This repository contains an analysis of the Karlan and List (2007) field experiment, which investigates the effectiveness of different fundraising treatments on donation behavior.

## Overview
The analysis focuses on exploring how different ask strategies, match ratios, and other socio-economic and demographic characteristics influence the probability and amount of donations.

## Data
- Source: `karlan_list_2007.dta`
- Dataset includes variables such as `treatment`, `donation amount`, `household income`, `education level`, `gender`, and other relevant features.

## Files
- `index.qmd`: Quarto markdown document containing code and narrative.
- `karlanlist.ipynb`: Jupyter notebook, outlining the code.

## Approach and Steps
1. **Data Loading and Cleaning**
   - Load the `.dta` file using pandas.
   - Inspect variable types, handle missing values, and perform necessary transformations.

2. **Exploratory Data Analysis (EDA)**
   - Plot histograms and bar charts for continuous and categorical variables to understand distributions.
   - Analyze donation behavior across demographic groups.

3. **Treatment Effect Analysis**
   - Compare the proportion of donors in the treatment and control groups.
   - Compare donation amounts (see `img4.png`) and calculate average treatment effect.

4. **Simulation and Statistical Validation**
   - Run simulations to demonstrate the Law of Large Numbers.
   - Illustrate the Central Limit Theorem by showing sampling distributions at various sample sizes.

5. **Summarize Key Findings**
   - Interpret the insights and effectiveness of the treatment strategies.
  
## Key Insights
- **Treatment Effects**: Treatment increased the donation rate slightly (2.2% vs 1.8%).
- **Donation Amounts**: Despite a higher response rate, the average donation in the treatment group was slightly lower than in the control group.
- **Simulations**:
  - Law of Large Numbers: Monte Carlo Simulation confirms convergence of sample means to the true treatment effect as sample size increases.
  - Central Limit Theorem: Shows how the distribution of sample means approaches normality with larger sample sizes.

## Requirements
- Python (with packages such as pandas, seaborn, matplotlib, statsmodels)
- Quarto for rendering `.qmd` files

## How to Reproduce
1. Open `index.qmd` in Quarto.
2. Ensure the dataset (`karlan_list_2007.dta`) is in the working directory.
3. Render the Quarto file or run cells to reproduce plots and analysis.

## References
Karlan, D., & List, J. A. (2007). Does Price Matter in Charitable Giving? Evidence from a Large-Scale Natural Field Experiment. *American Economic Review*, 97(5), 1774–1793.


