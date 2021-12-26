# MechaCar_Statistical_Analysis

## Overview of Project
A few weeks after starting his new role, Jeremy is approached by upper management about a special project. AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team.

In this challenge, you’ll help Jeremy and the data analytics team do the following:

1. Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
2. Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
3. Run t-tests to determine if the manufacturing lots are statistically different from the mean population
4. Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.

## Linear Regression to Predict MPG
![lm](https://user-images.githubusercontent.com/83085800/147395195-afa8b479-5f76-43bd-9c6a-af3963cce5d7.png)
As you can see in the above formula the vehical length and ground clearance have a significant impact on miles per gallon (mpg). While the vehicle weight, spoiler angle, All Wheel Drive (AWD) have p-values that indicate random amount of variance. The p-valu for this model is 5.35e-11 which is less than the 95% confidence level. There is sufficient eveidence to rejct the null hypothesis. With that being said the r-squared value is 71% of all mpg predictions. The regression model effectively predicts mpg of MechaCar.

## Summary Statistics on Suspension Coils
### Total Summary
![total_summary](https://user-images.githubusercontent.com/83085800/147395438-4916e233-d6aa-4d19-9b81-5ae5d0722bb0.png)
### Lot Summary
![lot_summary](https://user-images.githubusercontent.com/83085800/147395458-0c276649-b94e-4a63-b3df-e6c2a11bc6f7.png)
The variance of the coils is 62.29 for the variance and is well within the 100 PSI variance requrirement. Lot 1 and 2 are well within the 100 PSI requirement, but lot 3 with a variance of 170.29 is proportionately above the 100 PSI requirement.

## T-Test on Suspension Coils
![mechacoilPSI](https://user-images.githubusercontent.com/83085800/147395514-bf875bc7-429a-47d7-94e5-d13e3ab99896.png)
With a p-value of 0.06, which is greater than 0.05 significance level, there is NOT enough evidence to reject the null hypothesis. With that being said the lots is statisically similar to the population mean of 1500.
![Lot PSI](https://user-images.githubusercontent.com/83085800/147395534-442ddd4b-592c-4383-a74a-1fd1fc33b99e.png)
1. For lot 1 we can not reject the null hypothesis with a p-value of 1 which is greater than 0.06 significance level.
2. For lot 2 we can not reject the null hypothesis with a p-value of 0.61 which is grater than the significance level of 0.05, stating the sample mean and population mean or similar.
3. Lot 3 we will reject the null hypothesis with a p-value of 0.05 which is less than 0.05 significance level, stating the sample and population are not similar.
## Study Design: MechaCar vs Competition

### Variables
Variables to analyze acroos multiple manufacuters:
1. Engine type
2. MPG
3. Current Price
4. Amount of cars sold annually
### Hypothesis: Null and Alt
1. Null: MechaCar is priced correctly based on its success rate of cars sold annually compared to its competitors.
2. MechaCar is NOT priced correctly based om its success rate of cars sold annually compared to its competitors.
### Statistical Test
Since we are testing mutliple variables we would use a Multiple Linear Regression to test our hypothesis.





