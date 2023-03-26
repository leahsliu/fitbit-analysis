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

Provided more time, I would have also made some predictions and found relationships between the data (i.e. chi squared tests).

### Conclusions
Based on my exploratory analysis, there is a strong positive correlation between the steps I take and the calories burned. By using heat maps, I was also able to explore the relationship between the days of the week and my sleep quality. These heat maps showed that I get more deep sleep and REM sleep later in the week.

Lastly, I built a linear regression model with 4 features that predicts the calories burned with an R2 of 0.889. Since R2 tells us the goodness of fit of a logistic regression, I wanted to see if the FitBit data I collected could be used to create a better predictive algorithm. Thus a larger R-squared value of 0.889 meant that my data would fit the linear regression model better. To my surprise, there is a slightly negative correlation between the calories burned and my step count as seen by the -0.0299 relationship between calories burned and steps. However, we also know that the p-value is 0.239, which is really high. Thus we cannot make any conclusion about the relationship between steps and calories burned if we have a significance level of 5%.

### Visuals Explained
#### Line Plots of Steps vs. Time:
I used lineplots to show the relationship between steps and time despite a continuous relationship to show the dramatic effect in the steps I take everyday. The reason why I created 2 plots-- one with average monthly steps and one with daily steps is to show that there aren't many outliers that are causing the general trend of my steps to be different between graphs.

#### Regression and Line Plots of Carlories Burned vs. Steps:
The next graph is a regression plot. I used this graph to see more clearly the linear relationship between calories burned and steps. I also knew the seaborn regplot function also features a confidence interval that can show us if there is high confidence or low confidence in the parameters' relationship.

To see the relationship between steps and calories burned better, I plotted them against one another to reveal a positive relationship between the two.

#### Correlation Matrix:
The correlation matrix further emphasizes that there is a strong correlation between the 2 parameters-- presenting a value of 0.932225 correlation between calories burned and steps.

#### Heat Maps:
I plotted some heat maps to visualize the relationship between parameters based on cell color changes. I noticed patterns in how much deep sleep I get vs. the days of the week and also patterns in the number of steps I took vs. the days of the week.

#### Logistic Regression:
The 4 features I used were 'Steps', 'Distance', 'sq_Steps', 'sq_Distance'. The last 2 features, 'sq_Steps', 'sq_Distance', are the product of squaring a pre-existing feature. Other ways I could have made new indiciates was by computing indicator functions (a function that is 1 when the old feature is in a particular set and 0 when it isn’t), and multiplying features together.

To see my other annotations and code, please refer to my Jupyter Notebook: https://github.com/leahsliu/fitbit-analysis/blob/main/fitbit_data_analysis.ipynb

### Sources Cited:
https://seaborn.pydata.org/generated/seaborn.heatmap.html
