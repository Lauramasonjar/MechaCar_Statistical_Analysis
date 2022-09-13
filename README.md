# MechaCar_Statistical_Analysis
MechaCar_Statistical_Analysis

## Project Overview
AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management wants to have to review the production data for insights that may help the manufacturing team.

## Purpose

In this challenge, we need to perform following points on basis of statistics: 

- Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes.
- Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots.
- Run t-tests to determine if the manufacturing lots are statistically different from the mean population.
- Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. 
- For each statistical analysis, you’ll write a - summary interpretation of the findings.


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

With multiple linear regression model, we are identifying which variables (vehicle weight, spoiler angle, ground clearance, AWD and vehicle length in our case) in the dataset predict the mpg of MechaCar prototypes. In simple words, we are asking if there is a relationship between variables and mpg of MechaCar prototypes. 

**Null hypothesis and Alternative hypothesis for linear regression**

For multiple linear regression model, following hypothesis will help to understand significant linear relationship between values:

**H0:** The slope of the linear model is zero, or m = 0 (If there is no significant linear relationship, each dependent value would be determined by random chance and error. Therefore, our linear model would be a flat line with a slope of 0).

**Ha:** The slope of the linear model is not zero, or m ≠ 0 (If there is significant linear relationship, each dependent value would not be determined by random chance and error. Therefore, our linear model would not be a flat line with a slope greater or lesser than 0).
