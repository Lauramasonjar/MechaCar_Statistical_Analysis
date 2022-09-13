# MechaCar_Statistical_Analysis
MechaCar_Statistical_Analysis

## Project Overview
AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management wants to review the production data for insights that may help the manufacturing team.

## Purpose

In this challenge, we need to perform the following points on the basis of statistics: 

- Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes.
- Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots.
- Run t-tests to determine if the manufacturing lots are statistically different from the mean population.
- Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. 
- For each statistical analysis, you’ll write a summary interpretation of the findings.


## Requirements

- Linear Regression to Predict MPG
- Summary Statistics on Suspension Coils
- T-Test on Suspension Coils
- Design a Study Comparing the MechaCar to the Competition


## Resources
Data Source: 
-	[MechaCar_mpg.csv](Data/MechaCar_mpg.csv)
-	[Suspension_Coil.csv](Data/Suspension_Coil.csv)

## Software: 
- RStudio
- Languages: **R**

## Results & Analysis

### Linear Regression to Predict MPG 

With the multiple linear regression model, we are identifying which variables (vehicle weight, spoiler angle, ground clearance, AWD and vehicle length) in the dataset predict the mpg of MechaCar prototypes. Basically, we are asking if there is a relationship between variables and mpg of MechaCar prototypes. 

**Null hypothesis and Alternative hypothesis for linear regression**

For the multiple linear regression model, the following hypothesis will help to understand the significant linear relationship between values:

**H0:** The slope of the linear model is zero, or m = 0 (If there is no significant linear relationship, each dependent value would be determined by random chance and error. Therefore, our linear model would be a flat line with a slope of 0).

**Ha:** The slope of the linear model is not zero, or m ≠ 0 (If there is significant linear relationship, each dependent value would not be determined by random chance and error. Therefore, our linear model would not be a flat line with a slope greater or lesser than 0).

![MechaCar_Statistical_Analysis](https://github.com/Lauramasonjar/MechaCar_Statistical_Analysis/blob/main/Images/Linear%20Regression%20Results.png)
#

**1. Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?**

- To determine which variables provide a non-random amount of variance to the mpg value we have to look at their individual **p-value**. 
- If the p-value is below 0.05 it is statistically unlikely to provide random amounts of variance to the linear model, meaning that those variables have a significant impact on mpg. 
- According to our results *(Figure 1)* **ground clearance** (p-value = 5.21 x 10-8), **vehicle length** (p-value = 2.60 x 10-12), as well as **intercept** (p-value = 5.08 x 10-8) provided a non-random amount of variance to the mpg values in the dataset.
- When an intercept is statistically significant, it means there are other variables and factors that contribute to the variation in mpg that have not been included in the model. 
- These variables may or may not be within our dataset and may still need to be collected or observed.


**2. Is the slope of the linear model considered to be zero? Why or why not?**

- Based on our results in the image above, p-value is 5.35 x 10-11, which is much smaller than our assumed significance level of 0.05%. 
  Therefore,
- We can state that there is sufficient evidence to reject our null hypothesis. 
- The slope of our linear model is not zero, meaning that there is significant linear relationship between variables and mpg of MechaCar prototype.


**3. Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?**

- To determine if this linear model predict mpg of MechaCar prototypes effectively we need to look at its **r-squared** and **p-value**.
- According to our results in the image above, r-squared is 0.7149 and indicates a strong positive linear relationship, therefore, we can confirm that this linear model effectively predicts mpg of MechaCar prototypes.

### Summary Statistics on Suspension Coils

**The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?**

**Suspension Coil(total_summary)**

The current manufacturing data meet this design specification for all manufacturing lots in total. According to the results below, variance is 62.29 PSI and that is within requirements of not exceeding variance 100 PSI.

![MechaCar_Statistical_Analysis](https://github.com/Lauramasonjar/MechaCar_Statistical_Analysis/blob/main/Images/total_summary.png)


**Suspension Coil(lot_summary)**

The current manufacturing data partially meet this design specification for each lot separately. According to the results below, it shows that Lot 1 and Lot 2 meet the design specification with a variance of 0.9795918 and 7.4693878 PSI respectively, and it is within requirements of not exceeding variance 100 PSI. Lot 3 does not meet the design specification because of its variance of 170.286122 PSI which exceeds the requirements variance of 100 PSI.

![MechaCar_Statistical_Analysis](https://github.com/Lauramasonjar/MechaCar_Statistical_Analysis/blob/main/Images/lot_summary.png)


