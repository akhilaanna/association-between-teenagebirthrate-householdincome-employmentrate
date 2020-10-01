# Correlation Between Teenage Birth Rate, Household Income, and Employment Rate in Baltimore City, Maryland 

## Background Information 
Baltimore City is a metropolitan area in Maryland known for its rich cultural history and diverse neighborhoods. Being a major city in the United States, it has its share of economic struggles, faced by both the city government as a whole and by the residents that occupy it. Employment rate is a crucial indicator of a city's economic stability, but it is not only affected by the economy. Employment rate is also impacted by public health factors such as teenage birth rate. In this data analysis, I assess the relationship between a social factor (teenage birth rate) and an economic factor (household income) on the city's employment rate. 

## Business Question 
How do social and economic factors make an impact on Baltimore City's employment rate? 

## Data Question 
What is the correlation between teenage birth rate and employment rate using a simple linear regression model? What is the correlation between teenage birth rate, household income, and employment rate using a multiple linear regression model? 

Metrics used: teenage birth rate, household income, employment rate in Baltimore City, MD 
Data retrieved from: Opportunity Atlas https://www.opportunityatlas.org/. 

## Data Analysis Process 

**1) Simple Linear Regression: Relationship between Teenage Birth Rate and Employment Rate** 
	
*Slope*: -0.141178494 --> The negative slope indicates that as teenage birth rate increases, employment rate decreases. The absolute value of the slope is a very small number (less than 1), so the trendline is relatively flat. This means that as the teenage birth rate rises, the employment decreases only a little bit. 		

*Intercept*: 0.773863032 --> When the teenage birth rate is 0, the employment rate is 0.774. 					

*R-squared*: 0.071476839 --> 7.15% of the data can be explained by the linear regression line (trendline). This is very low. Based on the chart, it seems that it should be higher; however, the arithmetic shows that the R-squared value is very small, meaning that the trendline does not explain the data very well. 

*Standard Error*: 0.08476408 --> On average, the predicted value is 0.085 units away from the actual value. 						

Employment Rate = -0.1412(Teenage Birth Rate) + 0.7739					

Employment Rate for the average teenage birth rate (0.307) is predicted to be 0.73, or 73%. 

(simple lin regression visualization.png)

**2) Multiple Linear Regression: Relationship between Teenage Birth Rate, Household Income, and Employment Rate**

*R-squared*: 0.496771549 --> 49.7% of the data can be explained by the linear regression line (trendline). This is relatively high compared to the R-squared value from the simple linear regression conducted before. This means that the equation accurately explains almost half the data.  

*Standard Error*: 0.039538306 --> On average, the predicted value is 0.04 units away from the actual value. This is a low number, meaning that there is less difference between the predicted and actual values than if the standard error were higher. 

*Coefficients*:	3.08E-06 (household income), 0.009663745 (teenage birth rate) --> The coefficient for household income is extremely low (3.08E-06), but this doesn't necessarily mean that the effect of household income on employment rate is small. Since the household income values are large (in tens of thousands), the coefficient ends up being smaller to compensate for those large values. Though the value is small, it is still positive, meaning that there is a positive correlation between household income and employment rate (as income increases, employment rate by a little bit.) 

The coefficient for teenage birth rate is also low, but not as low as the coefficient for household income. Though low, it is positive, so in this model, as teenage birth rate increases, employment rate increases a little bit. This contrasts the results from the simple linear regression, so further research may be necessary to reach a consistent conclusion. 

*Significance F*: 1.00426E-51 --> Significance F is the probability that the household income and teenage birth rate don't actually make a meaningful contribution to predicting employment rate. The signifcance F for this model is very low, which means that the variables do matter and do correlate with employment rate. 

*P-values*: 1.82983E-12 (household income), 0.774784043 (teenage birth rate) --> P-values smaller than 0.05 indicate that the null hypothesis can be rejected. The null hypothesis is that there is no statistically significant impact of the independent variables on the dependent variable, so rejecting it would mean that there is an impact. The p-value of the household income is very small, meaning that the variable has significant effects. The p-value of the teenage birth rate, however, is larger than 0.05, so the variable does not have a statistically significant effect. The significance F value suggests that overall the variables do matter, but when considered individually, the data shows that the teenage birth rate cannot be concluded to have a significant impact on emplyoment rate.

## Business Answer 

Social factors and economic factors can both make an impact on employment rate. The data from the simple linear regression showed that teenage birth rate can make an impact, but did not show significant results in the multiple linear regression. Household income was only used for the multiple linear regression, and the results from it showed that it does have an impact. 

## Recommendations 

For the simple linear regression model, it was interesting to see the negative correlation between teenage birth rate and employment. Intuitively, this makes sense; if women are having children as teens, it is very hard to keep up with school and career, especially in under-resourced communities. From a public health perspective, Baltimore City can take preventative measures and develop programs to support teenage mothers, perhaps by providing them with a way to get their education and a job while they balance the work that comes with taking care of their baby. They can even develop programs that don't specifically aim to achieve graduation/employment, but rather have a mission to emotionally support teenage mothers so that they feel less stressed when it comes to school and work. Teenage birth rates themselves can be decreased by improving sex education, increasing access to contraceptives, among much more.  

Ultimately, these models are only predictions, and the equations generated from them can only explain so much about the relationships between the variables. The R-squared value for the simple linear regression was very small (7%) so that equation does not lead to much confidence in the predictions. The R-squared value for the multiple linear regression was about 50%, which is significantly higher, but still is not 100% accurate in predicting employment rate values. 

## Further Research 

For further research, I am interested in assessing other factors that affect employment rate, such as social policies regarding housing, education, and discrimination.  


