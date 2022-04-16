# MechaCar_Statistical_Analysis

## Overview

### Purpose

The purpose of this analysis was to review the produciton data for insights on some produciton troubles blocking the manufacturing team's progress on the MechaCar a new prototype by AutosRUs. The analysis included perfomring multiple linear regrssion analysis, collecting summary statistics, conducting t-tests to determine whether the lots are different statistically from the mean population. A statistical study was designed to study and compare vehicle performance of the MechaCar vehicles against vehicls from other manufacturers and interpret respective findings. 

<hr>

## Linear Regression to Predict MPG

![mecha_df_summary](https://user-images.githubusercontent.com/94864663/163631833-f0485712-f186-49ce-8de4-019713ff27ae.png)


The linear regression summary shows that the vehicle lengths and vehicle ground cleareance have very low probabilitis of observing any value equal or larger than the t value. This means there it would be extremely unlikely that the realtionship between vehivle length and mpg values and the relationship between ground clearance and mpg values would be due to chance alone. 

The summay also shows that the p-value for this model is 5.35e-11 which is smaller than a 0.05 significance level, providing more than enough evidence to reject the null hypothesis. This also provides evidence to assume the slope of the linear model will not be zero. This can be concluded because the p-value shows a a very low probability that th relationship shown in the data occured under the assumption of the null hypohthesis. 

Looking at the multiple r-squared value of 0.7149, this shows that about 71.5% of all predictions for mpg can be attribted to the model. Even adjusting for the number of independent variabels in the model, looking at the adjusted R-squared value of 0.6825 still shows a large percentage of predictions for mpg are determined by the model. Therfore, it is safe to assume the model is able to predict the mpg of the MechaCar prototypes by AutosRUs rather effectively. 



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


The total smmary shows a mean of 1498.78 which is very close to the median of 1500, meaning the we can assume the data follows a symmetrical normal distribution. Looking at the variance of 62.29 PSI, the suspension coil variance is well below the criteria of 100 pounds per square inch therefore the overall it appears the design specifications are met. However, the lot summary above shows that lot 1 and 2 with variances of about 0.98 and 7.47 respectively are well below the design criteria and also much lower than the variance for the entire population. Lot 3 with a variance of 170.3 however has a variance much higher than the acceptable limit and of course higher than the variance for the entire popilaiton. Therefore while it appears as if the entire populations meets the criteria, in reality, only variances for lot 1 and 2 fall well below 100 pounds per square inch.



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
