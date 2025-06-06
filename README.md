# Health_Insurance_Project

**In this project we will find out which variable (smoking, gender, number of dependants, region) is the most correlated with high health insurance charges. **

We also create dashboards using Power BI which you can see a live version of by clicking on, 
*[Home Page](https://app.powerbi.com/view?r=eyJrIjoiNmEwOTEzNDItOWU3My00N2IyLWFjMzctYTkyMjZkMjQ0MzlmIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9&pageName=dd58060b08b5c0aba9ae)*\
*[Average charges Page](https://app.powerbi.com/view?r=eyJrIjoiNmEwOTEzNDItOWU3My00N2IyLWFjMzctYTkyMjZkMjQ0MzlmIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)*


Also, we did inferential statistics and reported our findings.


*First, we clean the dataset using Power query.*\
 <img width="755" alt="1" src="https://github.com/user-attachments/assets/1bf02e9f-b751-4f28-8686-de13551a5e83" />


*Then for each factor having multiple values such as BMI, Age, and charges we get their summary statistics, their outliers using Box and whiskers, and their distribution using Histogram.*\
1.\
*BMI is normally distributed with skewness being near to zero. Median and mean are almost identical. Although there are a few outliers, I chose not to remove them on purpose because I expect BMI to be one big dependent variable to effect charges. So in this case, outliers may say something critical.*\
 <img width="741" alt="2" src="https://github.com/user-attachments/assets/ed0ac452-1b58-4735-bacf-73256f28a375" />


2.\
*Age seems to have normal distribution with no outliers. Minimum and maximum values are 18 and 64, respectively. We have young adult to old-aged individuals in the dataset.*\
 <img width="763" alt="3" src="https://github.com/user-attachments/assets/57a7e0f6-fcbb-4a1a-862a-46cc0b58cea1" />

3.\
*Charges are heavily right-skewed. A value between −2 and +2 is generally considered acceptable, but we have a lot more here. We have lots of outliers on the larger side. This shows us that big chunk of charges are low, on the other hand, some particularly high charges cause right-skewness. This might cause a problem at decision making, but let’s always take this into consideration during exploratory analysis.*\
 <img width="714" alt="4" src="https://github.com/user-attachments/assets/2f6de366-b7ac-45fb-97cb-ddb7d7bb3b91" />

4.\
*We then group data into small categories according to scientific guidelines by simply using IF, AND functions. We group data for BMI and age variables.*\
 <img width="950" alt="5" src="https://github.com/user-attachments/assets/c12ee798-77e6-410d-8ea9-476aedc62b21" />

5.\
*We also create a smoker range and a sex range using IF condition so we do not have any non-numerical data in our correlation range.*
 <img width="842" alt="6" src="https://github.com/user-attachments/assets/37763fcf-4cfd-408e-8b52-da70bba447e3" />

6.\
*Then we create a correlation matrix and find that smoking has highest correlation with charges, followed by age and BMI.*
 <img width="466" alt="7" src="https://github.com/user-attachments/assets/9e480600-6c86-4ee6-ba21-7876074157d9" />

7.\
**Then to create dashboard we have used Power BI.**\
[Live Dashboard link](https://app.powerbi.com/view?r=eyJrIjoiNmEwOTEzNDItOWU3My00N2IyLWFjMzctYTkyMjZkMjQ0MzlmIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9&pageName=dd58060b08b5c0aba9ae)\
Customer Proportions Dashboard:
 <img width="653" alt="8" src="https://github.com/user-attachments/assets/8e54db5d-9c65-4b5c-a597-789777b26ebd" />

Average Charges Dashboard:
 <img width="652" alt="9" src="https://github.com/user-attachments/assets/46c40d71-564b-42e6-9b4e-8cdc34fefb79" />

9.\
**Then finally we have done some inferential statistics based on our findings.**

##From Dashboard 1 we find that.\
- [x] Even though we have very less smokers as customers compared to non-smokers. But still the charges being spent on smokers is 80% which is a very significant proportion. One can conclude that smokers incur majority of insurance charges even being a small proportion of the population.
- [x] When it comes to age, we have mostly adult customers followed by middle age, young adult, and old age respectively.
- [x] When it comes to BMI score, we have a majority of obese customers followed by overweight, healthy weight, and underweight.
- [x] BMI score also has a very linear relationship with average insurance charges. The obesity BMI incurs the most charges followed by Overweight, healthy weight, and underweight.

##From Dashboard 2 we find that.\
- [x] We found from correlation that smoking is the most correlated variable with charges which is again being reflected by our charts.
- [x] When it comes to age, Old age customers incur the greatest charges per customer, followed by middle age, adult, and young adult.
- [x] Family size paints an interesting picture, where we see an increase in charges as the size of dependants reaches from 0 to 3, and then there is a sudden decrease till 5. Minimum value here is 0 and maximum is 5.
- [x] Southeast as a region is incurring the most charges. On 2nd place is north east followed by northwest and southwest.
- [x] Majority of smokers come from southeast and southwest regions.
