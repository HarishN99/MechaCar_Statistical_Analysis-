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


The total smmary shows a mean of 1498.78 which is very close to the median of 1500, meaning the we can assume the data follows a symmetrical normal distribution. Looking at the variance of 62.29 PSI, the suspension coil variance is well below the criteria of 100 pounds per square inch therefore the overall it appears the design specifications are met. However, the lot summary above shows that lot 1 and 2 with variances of about 0.98 and 7.47 respectively are well below the design criteria and also much lower than the variance for the entire population. Lot 3 with a variance of 170.3 however has a variance much higher than the acceptable limit and of course higher than the variance for the entire popilaiton. Therefore while it appears as if the entire populations meets the criteria, in reality, only variances for lot 1 and 2 fall well below 100 pounds per square inch.



<hr>

## T-Tests on Suspension Coils

<b>Suspension Coils t-test Results</b>

![D3ttest](https://user-images.githubusercontent.com/94864663/163632217-d2e2ea9b-d75f-4819-819c-d0c57959061a.png)

<br>

<b>Lot 1 t-test Results</b>

![Lot1_ttest](https://user-images.githubusercontent.com/94864663/163687994-0f008f68-215a-4ba2-855f-44378a184cc1.png)

<br>


<b>Lot 2 t-test Results</b>

![Lot2_ttest](https://user-images.githubusercontent.com/94864663/163687996-d5493084-d761-4cb0-891e-b411e4bf273d.png)

<br>


<b>Lot 3 t-test Results</b>

![Lot3_ttest](https://user-images.githubusercontent.com/94864663/163687998-8f1acc58-caa1-4799-bafa-7f89e8993e48.png)
<br>


The resutls of the t-test show a mean of 1498.78 compared with an expected null hypotheiss mean of 1500, with a p-value of 0.06, there is not enough evidence to support rejecting the null hypothesis. This is because the p-value is greater than a significance level of 0.05, meanign there is enough of a chance that the findings within the data are in support of the null. Therefore, we fail to reject the null and assume the mean of all three manufacturing lots are statistically similar to the expected populaiton mean of 1500. Looking at the lots individually,  both lots 1 and 2 with p-values of 1 and 0.61 also follow this pattern where their respective p-values are greater than a significance level of 0.05. However, the t-test for lot 3 shows a p-value of 0.042 which is lower than the significance level, allowing us to conclude the mean for lot 3 is statistically different from teh expeced mean of 1500. Ultimatly, this means there is somehting outside the realm of chance and random variance going on with lot 3. 

<hr>

## Study Design: MechaCar vs Competition

In order to determine how the MechaCar performs against the competition we can compare metrics such as customer satisfaction scores, horse power, and engine noise levels. The study will inolve collecting data on these metrics for the MechaCar as well as its top 3 competertors within a set time frame such as 1 year. 

The study will be conducted to see if the mean values for cost, horse power, and engine noise levels for the MechaCar will be any different from 3 of its competitors. An example of a null and alternative hypothesis for one of the metrics will be as follows:

H0: The difference in mean customer satisfaction score between the MechaCar and it's competitor will be 0.
Ha: The difference in mean customer satisfaction score between the MechaCar and it's competitor will be greater than 0.

A two-sample t-test will be used to compare the means of the MechaCar and three of its top competitors for each of the metrics mentioned above. This is appropriate because the two sample t-test is a method used to test wither the means of two indpendent groups are equal or not. 

Data on customer satisfaction scores for the MechaCar and its competitors on a scale from 1 - 5 sent to various consumers for a year would be required along with measured horsepower values in hp for the cars and measured engine noise levels in decibels (dB). Ideally we would want to test for satisfaction scores and horsepower being higher and engine noise levels being lower for the MechaCar. 




