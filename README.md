# MechaCar_Statistical_Analysis-
# Purpose:
•	Load, clean up, and reshape datasets using tidyverse in R. <br>
•	Visualize datasets with basic plots such as line, bar, and scatter plots using ggplot2.<br>
•	Generate and interpret more complex plots such as boxplots and heatmaps using ggplot2.<br>
•	Plot and identify distribution characteristics of a given dataset.<br>
•	Formulate null and alternative hypothesis tests for a given data problem.<br>
•	Implement and evaluate simple linear regression and multiple linear regression models for a given dataset.<br>
•	Implement and evaluate the one-sample t-Tests, two-sample t-Tests, and analysis of variance (ANOVA) models for a given dataset.<br>
•	Implement and evaluate a chi-squared test for a given dataset.<br>
•	Identify key characteristics of A/B and A/A testing.<br>
•	Determine the most appropriate statistical test for a given hypothesis and dataset.

# Results: 
## Linear Regression to Predict MPG
 ![image](https://user-images.githubusercontent.com/120526544/229679445-bf0ed361-2818-47f7-beac-12d63d9ec177.png)

#####	Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset? <br>
  -	As from the above picture we can see that the non-random amount of variance to the mpg value in the dataset provided are Vehicle length, Ground Clearance and AWD. The p-value: 5.35e-11, which is less than 0.05 indicates statistically significant in predicting the mpg values.<br>

#####	Is the slope of the linear model considered to be zero? Why or why not?<br>
  -	The slope of the linear model is not considered to be zero. The p-value: 5.35e-11 is less than 0.05, which indicates that it can reject or null hypothesis. <br>

#####	Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?<br>
  -	The R-squared value of linear model is  0.7149, which is approximately 71.49% of all mpg projections in the linear progression model. R-square is not the only dataset which is effective, there might be other variables that are not included in the dataset that may also affect the mpg in the dataset.
## Summary Statistics on Suspension Coils
### Total Summary:
 ![image](https://user-images.githubusercontent.com/120526544/229680188-1e1a9128-e2a3-42d0-8b32-fba98ecdde02.png)

### Lot_Summary:
 ![image](https://user-images.githubusercontent.com/120526544/229680204-199614f9-eb3c-4e68-b5d2-a9c05974d08f.png)


#####	The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not? 
- The overall variance of the total summary is under 100 psi, which meets the expectations of the design. However, in Lot 3 has a variance about 170.28 which is above the design specifications of 100 psi.<br>
- In short, manufacturing data meets the design specifications for all the lots, except lot 3.
## T-Tests on Suspension Coils
•	Summarize your interpretation and findings for the t-test results. Include screenshots of the t-test to support your summary.
 ![image](https://user-images.githubusercontent.com/120526544/229680658-d0c4db0a-5ba7-4b57-99ae-9d1eac69a337.png)

##### LOT 1:
•	p-Value for the lot1 is 1 which is greater than the significance value of 0.05, which shows not enough data to reject the null hypothesis and population mean PSI is not different than 1500
![image](https://user-images.githubusercontent.com/120526544/229680688-086d2651-5ec6-458c-86b8-0adb368e1292.png)

 
##### LOT 2:
•	Lot 2, p-value = 0.6072 is greater than significance level of 0.05, which is not enough to reject the null hypothesis. The sample mean PSI is not different from 1500.
 ![image](https://user-images.githubusercontent.com/120526544/229680746-cc18901e-c2d5-49b7-8f86-e9104b685638.png)

##### LOT 3:
•	Lot 3 p-value = 0.04168 < significance level of 0.05. The suspension coil for Lot 3 are different from the population mean PSI to reject the null hypothesis
•	
 
•	In conclusion we can say that the t.test for PSI across all manufacturing lots shows the p-Value of the total suspension coil dataset is greater than the significance level of 0.05, which fail to reject the null hypothesis except for the Lot 3 which has p-Value less than significance level of 0.05 and therefore, we reject the hypothesis. 
## Study Design: MechaCar vs Competition.
1.	Write a short description of a statistical study that can quantify how the MechaCar performs against the competition. In your study design, think critically about what metrics would be of interest to a consumer: for a few examples, cost, city or highway fuel efficiency, horsepower, maintenance cost, or safety rating.

•	There are many factors, but one possible concern for many consumers could be the focus on fuel efficiency. The study would involve in collecting the data on fuel efficiency in city and HWY of MechaCar against competitors and then using to compare it with different vehicle performance. <br>
#####	What metric or metrics are you going to test?
-  	Metric to be tested would be the fuel efficiency as compared to its competitors in terms of city and HWY. <br>
#####	What is the null hypothesis or alternative hypothesis?
-   Null hypothesis is MechaCar is not different from its competitors in terms of fuel efficiency.
-   Fuel efficiency is different from its competitors. <br>
#####	What statistical test would you use to test the hypothesis? And why?
-  	The best statistical test would be two-sample test and linear regression summary. <br>
#####	What data is needed to run the statistical test?
-  	To run this, we would need the data on fuel efficiency of MechaCar and its competitors in city and HWY.
-  	 Collecting the data in similar conditions to measure the fuel efficiency and then need the mean, variance to perform the test.
-  	Another data that might be helpful would be size of engine that could affect the fuel efficiency.

