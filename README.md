# MechaCar_Statistical_Analysis
# MODULE 15: STATISTICS and R

## Overview
Jeremy is 10-Year veteran employee of Autos-R-Us and has just been named as the Primary Analyst of the Data Analytics Team.  He and his team are in charge of the following:
* RETROSPECTIVE ANALYSIS OF HISTORICAL DATA
* ANALYTICAL VERIFICATION OF CURRENT AUTOMOTIVE SPECIFICATIONS
* STUDY DESIGN OF FUTURE PRODUCT EVALUATIONS & ASSESSMENTS

### NEW TOOLS
* R: a programming language for data analytics and statistics.
* RStudio: and IDE for the R language.

### ** CHALLENGE **
Jeremy and his team are asked by upper management to review production data for the company's newest prototype, the MechaCar which has not yet moved into the manufacturing stage as it is hampered by production issues.  Their insights with the analysis may help the manufacturing team graduate the prototype past the production stage.  They are given data on test results from 50 prototype vehicles that use multiple design specifications to do the following:
* DELIVERABLE I: Identify which variables predict the MPG of the MechaCar prototype
* DELIVERABLE II: Determine if the manufacturing process for suspension coils and their weight capacities is consistent by testing different metrics across different lots, centering on the coils' PSI.
* DELIVERABLE III: Given the Population mean of 1500 pounds per square inch, determine if the PSI across all manufacturing lots is statistically different.
* DELIVERABLE IV: Using a statistical study, compare quatifiable aspects of performance of the MechaCar against those of other manufacturers.

## DELIVERABLE I: USE LINEAR REGRESSION TO PREDICT MPG PROBABILITY VARIANCES
![MOD 15 CHALLENGE DEL I - SUMMARY OF LINEAR REGRESSION MODEL](https://user-images.githubusercontent.com/99851509/175805802-3884c4cb-5698-42ef-933c-b85ce00a6b10.png)
![MOD 15 CHALLENGE DEL I - SUMMARY (ENLARGED)](https://user-images.githubusercontent.com/99851509/175838250-7a5737e6-8474-43c2-b768-8d5886922110.png)

The PROBABILITY of VARIANCE for each COEFFICIENT or Pr(>|t|)-value for the variables were as follows:
* VEHICLE LENGTH: 0.00000000000260 ***
* VEHICLE WEIGHT: 0.0776
* SPOILER ANGLE: 0.3069
* GROUND CLEARANCE: 0.0000000521 ***
* ALL-WHEEL DRIVE (AWD): 0.1852

* p-VALUE: 0.0000000000535
* R-SQUARED VALUE: 0.7149

According to the results, VEHICLE LENGTH and GROUND CLEARANCE were statistically very unlikely to provide random amounts of variance so the impact on the prototype's MPG would be significant.  Additionally the p-VALUE was well below the significance level of 0.05 so we can reject the null hypothesis and therefore consider the slope for this linear model not to be zero.  the R-SQUARED VALUE is calculated as 0.7149 (or approximately 71% without rounding up) so while there may be other factors that can affect the predictive probability of this model, overall it is fairly good.  Some other variableS to consider that can affect MPG that were not in this model may include but are not limited to:
* WEATHER CONDITION, PARTICULARLY COLD (WINTER) WEATHER
* BAD FUEL INJECTION SYSTEMS
* DIRTY FUEL FILTERS
* DRIVER HABITS: SPEEDING, HEAVY BRAKING, ETC.


## DELIVERABLE II: SUMMARY STATISTICS ON SUSPENSION COILS

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch.

### SUMMARY OF TOTAL MANUFACTURING LOTS

![MOD 15 CHALLENGE DEL II - SUMMARY OF SUSPENSION COIL](https://user-images.githubusercontent.com/99851509/175838145-decc5c91-7cd0-4ca6-be72-1de10b01e276.png)
![MOD 15 CHALLENGE DEL II - SUMMARY (ENLARGED)](https://user-images.githubusercontent.com/99851509/175838645-f6e129ac-76e1-4a12-9276-368038f5360c.png)

The results of the TOTAL SUMMARY for all 3 lots are as follows:
* MEAN: 1498.78
* MEDIAN (RANGE): 1452 to 1505
* VARIANCE: 62.29356
* STANDARD DEVIATION: 7.892627

The results of the TOTAL SUMMARY for the Suspension Coils design specifications indicate the variance is within the 100 pounds per square inch tolerance limitations coming in at 62.29356 pounds per square inch.

### LOT SUMMARY BY EACH MANUFACTURING GROUP LOT

![MOD 15 CHALLENGE DEL II - LOT SUMMARY](https://user-images.githubusercontent.com/99851509/175841711-5574c468-a039-4f9d-a8df-efa640238818.png)
![MOD 15 CHALLENGE DEL II - LOT SUMMARY (ENLARGED)](https://user-images.githubusercontent.com/99851509/175841743-74a9966e-887e-4ed6-a3be-cd57b6c73834.png)

The results of the LOT SUMMARY is as follows, by LOT:
### LOT 1
* MEAN: 1500.00
* VARIANCE: 0.9795918
* STANDARD DEVIATION: 0.9897433

### LOT 2
* MEAN: 1500.20
* VARIANCE: 7.4693678
* STANDARD DEVIATION: 2.7330181

### LOT 3
* MEAN: 1496.14
* VARIANCE: 170.2861234
* STANDARD DEVIATION: 13.0493725

By comparing the statistical analysis for each group lot, we see that LOT 1 and LOT 2 has a variance below the 100 pounds per square inch tolerance limit, however LOT 3 has a variance level that is well above that limitation and does not meet design specifications in this regard.


## DELIVERABLE III: T-TESTS ON SUSPENSION COILS

Perform t-tests to determine if all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds per square inch.

### T-TEST FOR ALL LOTS
![MOD 15 CHALLENGE DEL III - ALL LOTS T-TEST](https://user-images.githubusercontent.com/99851509/175864032-1c4f934c-cfb3-42dd-8a9b-eac98ea76546.png)
* p-VALUE: 0.06028
* MEAN: 1498.78

### T-TEST FOR LOT 1
![MOD 15 CHALLENGE DEL III - LOT 1 T-TEST](https://user-images.githubusercontent.com/99851509/175864114-18c0ac4f-464d-4dde-960b-f19466e8c927.png)
* p-VALUE: 1
* MEAN: 1500

### T-TEST FOR LOT 2
![MOD 15 CHALLENGE DEL III - LOT 2 T-TEST](https://user-images.githubusercontent.com/99851509/175864189-b7b0aa9c-0401-4723-a9c6-4a3c52213409.png)
* p-VALUE: 0.6072
* MEAN: 1500.2

### T-TEST FOR LOT 3
![MOD 15 CHALLENGE DEL III - LOT 3 T-TEST](https://user-images.githubusercontent.com/99851509/175864269-a412b5fa-6060-469a-a0cf-e1bac829042f.png)
* p-VALUE: 0.04168
* MEAN: 1496.14















