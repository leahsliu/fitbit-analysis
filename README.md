# Analyzing FitBit Data
In this project, I analyzed my own FitBit data that was recovered from the FitBit database. I referred to the site for instructions on how to export my data here: https://help.fitbit.com/articles/en_US/Help_article/1133.htm

Please refer to my fitbit_data_analysis.ipynb file to see my data analysis.
File: https://github.com/leahsliu/fitbit-analysis/blob/main/fitbit_data_analysis.ipynb

### Data Analysis Process
The steps I followed were:
1. Exporting data
2. Cleaning data
3. Forming exploratory analysis questions
4. Performing data analysis/ creating visualizations

Provided more time, I would have also made some predictions and found relationships between the data (i.e. logistic regressions and chi squared tests).

### Visuals Explained
I used lineplots to show the relationship between steps and time despite a continuous relationship to show the dramatic effect in the steps I take everyday. The reason why I created 2 plots-- one with average monthly steps and one with daily steps is to show that there aren't many outliers that are causing the general trend of my steps to be different between graphs.

The next graph is a regression plot. I used this graph to see more clearly the linear relationship between calories burned and steps. I also knew the seaborn regplot function also features a confidence interval that can show us if there is high confidence or low confidence in the parameters' relationship.

The correlation matrix further emphasizes that there is a strong correlation between the 2 parameters-- presenting a value of 0.932225 correlation between calories burned and steps.

Lastly, I plotted some heat maps to visualize the relationship between parameters based on cell color changes. I noticed patterns in how much deep sleep I get vs. the days of the week and also patterns in the number of steps I took vs. the days of the week.

To see my other annotations and code, please refer to my Jupyter Notebook: https://github.com/leahsliu/fitbit-analysis/blob/main/fitbit_data_analysis.ipynb

### Sources Cited:
https://seaborn.pydata.org/generated/seaborn.heatmap.html