# MechaCar_Statistical_Analysis

## Overview of the Analysis
AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles. By running regression analyses and t-tests, I will review production data for AutoRU's newest prototype, the MechaCar, and provide insights that may help the manufacturing team. Additionally.

## Linear Regression to Predict MPG

![Mecha_car Summary](https://user-images.githubusercontent.com/53358476/202862380-8413994f-8e5a-43ff-958d-3e8ca61a90d9.PNG)

The linear regression model above estimates that:

mpg = (6.267)vehicle_length + (0.0012)vehicle_weight + (0.0688)spoiler_angle + (3.546)ground_clearance + (-3.411)AWD - 104.0

* Using the formula above, vehicle length, and ground clearance are statistically likely to provide non-random amounts of variance to the model or are most likely to affect the miles per gallon performance of the MechaCar's AutosRUs prototype.

* Given the model's p-value of 5.35e-11, which is lower than the 0.05 assumed statisticly significance, there is strong evidence against the null hypothesis (slope = 0). Therefore, we can accept the alternative hypothesis that the slope is not 0.

* The model's r-squared value of .7149 means that about 71% of the variance in mpg predictions can be explained by this model, while 29% cannot. In other words, the variables of vehicle length, spoiler angle, ground clearance, and AWD have a strong positive association with mpg. Therefore, this model effectively predicts mpg of MechaCar prototypes.

## Summary Statistics on Suspension Coils

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Looking at the PSI data for all three manufacturing lots, provided in the PSI summary chart below

![Total_Summary](https://user-images.githubusercontent.com/53358476/202862625-822b2018-ae2d-4c44-bc46-8a0d9784d982.PNG)

When we break the manufacturing data by the three lots, shown below, we see that on the one hand Lot 1 and 2 have variances of 0.98 and 7.47 that are well below the design specification of 100 pounds per square inch

![Lot_Summary](https://user-images.githubusercontent.com/53358476/202862678-10eda2db-d4d5-49ab-b096-796cb72d6dba.PNG)

 On the other hand, Lot 3, has a much larger variance of 170.29 that is well above the design specification.


##  T-Tests on Suspension Coils

t-test was used to determine if the PSI across all manufacturing lots is statistically different from the population mean of 1,500 pounds per square inch. The result of the t-test showed that there was a sample mean of 1,498.78 and a p-value of 0.06.

![Sample test 1](https://user-images.githubusercontent.com/53358476/202862859-5d8891c5-f937-4017-ac4b-4489fc8a5e87.PNG)

![Sample t-test 2](https://user-images.githubusercontent.com/53358476/202862919-d3281980-83fd-491f-b094-1539e4cda8df.PNG)

![Samplet-test 3](https://user-images.githubusercontent.com/53358476/202862925-3a866991-3945-4497-b978-72f48d21693e.PNG)

![Total_Summary2](https://user-images.githubusercontent.com/53358476/202862954-4bbe88f7-b167-44f8-9962-6796cb1546aa.PNG)

## Study Design: MechaCar vs Competition

To Many custoers, families value sevral things about a vehical, none other then the reliability and over all safety such as the time and pressure needed for the breaks.
To test the safety rating against its competition, we need to create a null and alternative hypothesis.


* H0 **Null Hypothesis**: MechaCar's vehicle safety ratings are no different from its competitors
* Ha **Alternative Hypothesis**: MechaCar's vehicle safety ratings are different from its competitors

To test these, we'd need to collect safety ratings on MechaCar's models as well as its competitors from the Institute for Highway Safety, which determines saftey ratings based on safety belts, crash dummies, breaking speed, and Air bag deployment. Using that data, we could t-test the population of vehicles and each carmaker. This will help us determine if MechaCar's vehicles' safety rating scores are statistically different from its competitors as a whole and then statistically different from each competitor.
