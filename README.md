# Excel-Business-Analysis-project-for-Amazon-using-synthetic-and-openly-available-data
In this Excel file, I performed data cleaning, handled missing values, bootstrapping using percentiles at 0.975, conditional formatting for annual income and purchase amount, anomaly detection using Z-scores, binning and Min-Max transformation for annual income stratification, and finally performed hypothesis testing and visualisations.

Visualisations
Scatter plot for Annual Income and purchase amount. I chose this type of graph as it would show the correlation between two numerical variables, as this would show if annual income influenced the purchase amount of these customers. However, there was no correlation as all data points were dispersed.  

Histogram for distribution of PurchaseAmount. This chart would allow visualization of the distribution of my continuous numerical data. This way I created purchasing ranges in 7 bins to distinguish which purchase ranges were more common, and which less as this can help the business identify customer behaviour. 

Most purchases are between £272.97 and £1485.57, and specifically most common purchase amount was between £879.27 and £1,081.37. The reason behind the low number of purchases under £272.97 and after £1485.57, could be investigated further. Maybe there was an additional delivery fee which caused customers to only order higher purchases, and maybe the demographic ordering at this shop isn’t buying expensive items or in bulk. 

Warehouse location bar chart to view difference in delivery times. The bar chart was used to allow comparison for the categorical data. 

As seen from the data, some cities performed faster delivery times such as Newcastle, and Glasgow, this could indicate that there is better logistics in these cities, or that there are less orders or more customers. Also, large delivery times were seen in Coventry and Southampton, therefore these cities could be investigated further to find new methods to speed up the logistics process. 

Boxplot to compare the annual income distribution across genders. I chose this chart as it provides identification of tendencies, spread of data, and variability.  
It was seen that females had the highest range (indicated by the interquartile ranges of the salaries extending from £20854.35 (lowest salary) to £200000 (highest salary), this could suggest women from all incomes like to shop at this company. The interquartile ranges were largest for females, followed by men, and then lowest for the “other” category.  

The median annual income was slightly lower for males when compared to females and other. The range of income showed a narrower range for the “other” category, so this shows lower variability and could indicate the need of more targeted marketing to this group. Also, no outliers were seen so I can assume my data cleaning was successful. 
Values from 6 number summary confirmed with Descriptive statistics 

Bar chart for gender distribution of data collected. I chose the bar chart, for visual comparison of categorical variable (gender). 

As seen, more male’s data was included in the dataset, and then followed by women. The other group should be analysed further to encourage data ethics methods to allow equity and fairness for all genders. Also, in addition to the previous boxplot, this bar chart would suggest the females in the group were from more varied backgrounds than men, as men had lower interquartile ranges, but as seen here, there were more in count. 

Pie chart for category popularity. I chose this chart as it would allow visualization of the whole data (categorical data). 
I found categories B, C and E were most popular, I also found that category D was the least popular, therefore in terms of logistics, it would be good to investigate why this product is less popular.  

Statistics

Hypothesis: Age and gender do not significantly influence the final purchase amount. H0: μA = μ0   

Alternative hypothesis: Age and/or gender significantly influence the final purchase amount. H1: μA  ≠ μ0 (This is a two-sided test) 

Correlation analysis 

No correlation between these variables was found, as no values greater than 0.5.  

T-tests for each of the variables.

As both t-tests showed a p-value (1.984) > 0.05, we reject the null hypothesis, so there’s no significant difference in purchase amounts depending on age or gender. 

T- test for the 3 variables. The T-stat was so close to 0, which shows the difference between the variables has no statistical significance, therefore reject the null hypothesis. (James, G, 2021).  

Regression  
Regression line equation: y= 691.758 + 1.485x1 + 0.566x2.  

When age is 0 and the age in binary is 0 (male), the purchase amount is £691.758. Each unit increase in age, will increase the purchase amount by 1.485. Each unit increase in gender binary (0 for male, 1 for female, 2 for other) will cause an increase in purchase amount by 0.566. 

R-Square: 0.0032 so no significant impact, indicating that the model explains only 0.32% of the variation in Purchase Amount, model is not a good fit. This suggests that other variables may cause the variation, but not age, or gender.  

Standard Error values are high for purchase amount, and then moderately high for gender. This would suggest this regression model is a poor fit. 

Both p-values are over alpha (0.05) at 0.5796 for age x1, and 0.9920 for x2 gender in binary (0.992), this suggests the variables have no statistical significance.  

The value of 0 is contained in both confidence intervals for x1 and x2, therefore, these indicate no correlation between the variables. 

As seen the predicted and revised values don’t fit on top of eachother, this suggests this model is a not a good fit. 

The gender in binary residual plot, fails the linear regression model as values are largely positive or negative and shows a pattern. The age residual plot has values away from 0 due to large error in our model, so both plots show the model didn’t fit. (Moore, D. et al, 2021) 
