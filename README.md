# MechaCar_Statistical_Analysis

## Overview

### Purpose

The purpose of this analysis was to review the produciton data for insights on some produciton troubles blocking the manufacturing team's progress on the MechaCar a new prototype by AutosRUs. The analysis included perfomring multiple linear regrssion analysis, collecting summary statistics, conducting t-tests to determine whether the lots are different statistically from the mean population. A statistical study was designed to study and compare vehicle performance of the MechaCar vehicles against vehicls from other manufacturers and interpret respective findings. 

<hr>

## Linear Regression to Predict MPG

![mecha_df_summary](https://user-images.githubusercontent.com/94864663/163631833-f0485712-f186-49ce-8de4-019713ff27ae.png)


Write a short summary using a screenshot of the output from the linear regression, and address the following questions:

- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
- Is the slope of the linear model considered to be zero? Why or why not?
- Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?




The linear regression summary shows that the vehicle lengts and vehicle ground cleareance are 




The linear regression summary shows that the dataset fits within normal parameters 
- R-squared is around 70% which means abot 7-% of the variablity of (DV) is explained using this linear model. 
- p-value is much lower than a significance level of 0.005, safe to reject the null hypothesis

<hr>

## Summary Statistics on Suspension Coils

<b>Total Summary</b>

![total_summary](https://user-images.githubusercontent.com/94864663/163631903-cfce722c-fdc0-4f00-a12a-c0f55e5b98a5.png)

<br>

<b>Lot Summary</b>

![lot_summary](https://user-images.githubusercontent.com/94864663/163631949-38ac5280-0817-45ee-a9f2-a2f3868c5ebf.png)


write a short summary using screenshots from your total_summary and lot_summary dataframes, and address the following question:

- The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. 
- Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

<hr>

## T-Tests on Suspension Coils

<b>Suspension Coils t-test Results</b>

![D3ttest](https://user-images.githubusercontent.com/94864663/163632217-d2e2ea9b-d75f-4819-819c-d0c57959061a.png)



Briefly summarize your interpretation and findings for the t-test results. Include screenshots of the t-test to support your summary.

<hr>

## Study Design: MechaCar vs Competition

Using your knowledge of R, design a statistical study to compare performance of the MechaCar vehicles against performance of vehicles from other manufacturers.

Write a short description of a statistical study that can quantify how the MechaCar performs against the competition. In your study design, think critically about what metrics would be of interest to a consumer: for a few examples, cost, city or highway fuel efficiency, horse power, maintenance cost, or safety rating.

In your description, address the following questions:
- What metric or metrics are you going to test?
- What is the null hypothesis or alternative hypothesis?
- What statistical test would you use to test the hypothesis? And why?
- What data is needed to run the statistical test?
