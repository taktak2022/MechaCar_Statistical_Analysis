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

![MOD 15 CHALLENGE DEL II - SUMMARY OF SUSPENSION COIL](https://user-images.githubusercontent.com/99851509/175838145-decc5c91-7cd0-4ca6-be72-1de10b01e276.png)
![MOD 15 CHALLENGE DEL II - SUMMARY (ENLARGED)](https://user-images.githubusercontent.com/99851509/175838645-f6e129ac-76e1-4a12-9276-368038f5360c.png)


