# Health_Insurance_Project
##Health Insurance Project##
**In this project we will find out which variable (smoking, gender, number of dependants, region) is the most correlated with high health insurance charges. **

We also create dashboards using Power BI which you can see a live version of by clicking on, 
[Home Page] (https://app.powerbi.com/view?r=eyJrIjoiNmEwOTEzNDItOWU3My00N2IyLWFjMzctYTkyMjZkMjQ0MzlmIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9&pageName=dd58060b08b5c0aba9ae)
[Average charges Page] (https://app.powerbi.com/view?r=eyJrIjoiNmEwOTEzNDItOWU3My00N2IyLWFjMzctYTkyMjZkMjQ0MzlmIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)


Also, we did inferential statistics and reported our findings.

*First, we clean the dataset using Power query.*
 

*Then for each factor having multiple values such as BMI, Age, and charges we get their summary statistics, their outliers using Box and whiskers, and their distribution using Histogram.*
1.
*BMI is normally distributed with skewness being near to zero. Median and mean are almost identical. Although there are a few outliers, I chose not to remove them on purpose because I expect BMI to be one big dependent variable to effect charges. So in this case, outliers may say something critical.*
 

2.
*Age seems to have normal distribution with no outliers. Minimum and maximum values are 18 and 64, respectively. We have young adult to old-aged individuals in the dataset.*
 
3.
*Charges are heavily right-skewed. A value between −2 and +2 is generally considered acceptable, but we have a lot more here. We have lots of outliers on the larger side. This shows us that big chunk of charges are low, on the other hand, some particularly high charges cause right-skewness. This might cause a problem at decision making, but let’s always take this into consideration during exploratory analysis.*
 
5.
*We then group data into small categories according to scientific guidelines by simply using IF, AND functions. We group data for BMI and age variables.*
 
6.
*We also create a smoker range and a sex range using IF condition so we do not have any non-numerical data in our correlation range.*
 
7.
*Then we create a correlation matrix and find that smoking has highest correlation with charges, followed by age and BMI.*
 
8.
*Then to create dashboard we have used Power BI.*
[Live Dashboard link] (https://app.powerbi.com/view?r=eyJrIjoiNmEwOTEzNDItOWU3My00N2IyLWFjMzctYTkyMjZkMjQ0MzlmIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9&pageName=dd58060b08b5c0aba9ae)
Customer Proportions Dashboard:
 
Average Charges Dashboard:
 
9.
*Then finally we have done some inferential statistics based on our findings.*

##From Dashboard 1 we find that.
- [x] Even though we have very less smokers as customers compared to non-smokers. But still the charges being spent on smokers is 80% which is a very significant proportion. One can conclude that smokers incur majority of insurance charges even being a small proportion of the population.
- [x] When it comes to age, we have mostly adult customers followed by middle age, young adult, and old age respectively.
- [x] When it comes to BMI score, we have a majority of obese customers followed by overweight, healthy weight, and underweight.
- [x] BMI score also has a very linear relationship with average insurance charges. The obesity BMI incurs the most charges followed by Overweight, healthy weight, and underweight.

##From Dashboard 2 we find that.
- [x] We found from correlation that smoking is the most correlated variable with charges which is again being reflected by our charts.
- [x] When it comes to age, Old age customers incur the greatest charges per customer, followed by middle age, adult, and young adult.
- [x] Family size paints an interesting picture, where we see an increase in charges as the size of dependants reaches from 0 to 3, and then there is a sudden decrease till 5. Minimum value here is 0 and maximum is 5.
- [x] Southeast as a region is incurring the most charges. On 2nd place is north east followed by northwest and southwest.
- [x] Majority of smokers come from southeast and southwest regions.
