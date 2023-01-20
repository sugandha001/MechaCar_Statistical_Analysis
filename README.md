# MechaCar_Statistical_Analysis

#### In this analysis we are helping the management of a the company AutosRUs’ as their newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. For this we need to -
- Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes.
- We will collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots.
- We will run t-tests to determine if the manufacturing lots are statistically different from the mean population.
- We will also design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. 

# Linear Regression to Predict MPG
![Screenshot (203)](https://user-images.githubusercontent.com/112904905/213593177-ec343b68-d91a-4e0c-af0c-aa20f9d92b02.png)

## This analysis will help us answer the following questions -

## 1. Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
As noted in the image above Vehicle length and ground clearance are unlikely to provide random amount of variance to the mpg values. These will have a significant impact on mpg.

## 2. Is the slope of the linear model considered to be zero? Why or why not?
Slope of the linear model is not zero since the p-value is less than 0.

## 3. Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
The mult5iple R-squared value is 0.7149. This means that 71% of all mpg predictions will be determined. This model will predict mpg of mechacar prototype effectively.

## Summary Statistics on Suspension Coils

## Lot Summary

![Screenshot (211)](https://user-images.githubusercontent.com/112904905/213595494-e3aeabb3-fb90-4197-ae6c-a9c7b0621fdc.png)

## Total Summary

![Screenshot (212)](https://user-images.githubusercontent.com/112904905/213595691-47834601-3d7d-48fa-b4e9-470fb665c1cf.png)


##Screenshots of total_summary and lot_summary dataframes addresses the following question:

### The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
Lot 1 has a variance on PSI of 1 and lot 2 has variance on PSI 7.4. Both these lots meet the design specification.
Lot 3 on the other hand has a variance on PSI of 170. So, it does not meet the design specification.
Together the variance on PSI is 62.29 which meets the design requirement.

## T-Tests on Suspension Coils
We performed t-tests to determine if all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds per square inch.

![Screenshot (206)](https://user-images.githubusercontent.com/112904905/213596547-047bc6c5-e8fe-4e1d-ad0e-1a692feb3b1c.png)

![Screenshot (205)](https://user-images.githubusercontent.com/112904905/213596676-6812fc8b-67d5-4693-a945-9c011938401a.png)

![Screenshot (204)](https://user-images.githubusercontent.com/112904905/213596776-c1be6ef8-b8a3-4da1-b736-de8e0dae1fa3.png)

NULL Hypothesis - There is no significant difference between the mean PSI of all manufacturing lots and individual lots with a polpulation mean of 1500 PSI.
Alternate Hypothesis - There is a significant difference between the mean PSI of all manufacturing lots and individual lots with a polpulation mean of 1500 PSI.

### Result  - 
Significance value - 0.05
The t-test results of the lots -
lot 1 - p - value is 1 - so we can say that there is not enough evidence to reject the null hypothesis and we can confirm our samples are not statistically different.
lot 2 - p- value is 0.60 - there is not enough evidence to reject the null hypothesis.
lot 3 - p-value is 0.04 - p- value is lower than 0.05 so we can reject the null hypothesis. the samples are not statistically different.

## Study Design: MechaCar vs Competition
Quantifying results based on statistical evaluation of different metrics that compare mechacar to it's competition.

### 1. What metric or metrics are you going to test?
- Fuel efficiency
- Cost of maintenance
- Resale value
- Engine - Electric/hybrid/gasoline

### 2. What is the null hypothesis or alternative hypothesis?
Fuel Efficiency
Null Hypothesis - Mechacar gives better gas average than it's competitor
Alternative hypothesis - Mechacar does not provide better gas average as compared to it's competitor

### 3. What statistical test would you use to test the hypothesis? And why?
Using p-value we can determine if mechacar is more fuel efficient than it's competitors.

### 4. What data is needed to run the statistical test?
We can collect sample data for the 2 cars and calculate mean and variance.
