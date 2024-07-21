# Pain
A series of statistical analysis regarding pain, fibromyalgia etc

## Results and interpretations from the fibromyalgia notebook:
All of the variables have weak (height being VERY weak) but statistically significant correlation to fibromyalgia (bmi - weight - skin area - height in order of strength high to low)

None of the independent variables (height, weight, skin area, BMI) show a strong or statistically significant direct relationship with fibromyalgia status after controlling for the other variables. The only significant result is the partial correlation between height and fibromyalgia status, but the effect size is very small and might not be practically significant.

People who have fibromyalgia are, in average, older, shorter, heavier, has a higher BMI and skin area than those who don't have fibromyalgia. These differences are statistically significant as shown in the t-test. 

Mean X of people without and with fibromyalgia:

height: 1.623 - 1.616

weight: 68.740 - 73.939 

BMI: 26.117 - 28.316

BSA: 1.728 - 1.776

age: 10.081 - 11.624 (Age scale is different, it apprxmtly means age 50 - age 58)

## Result of logistic regressions:
### height - bmi -> fibromyalgia
For height, the odds ratio of 0.310 indicates that for each unit (per meters) increase in height (in meters), the odds of having fibromyalgia decrease by approximately 69% (since 1 - 0.310 = 0.69).
For each centimeter increase in height, the odds of having fibromyalgia decrease by about 1.2% (since 1 - 0.988 = 0.012 or 1.2%).

For BMI, the odds ratio of 1.084 suggests that for each unit increase in BMI, the odds of having fibromyalgia increase by about 8.4%. (?) It is suprising how height has weaker correlation but is a better predictor of fibromyalgia

### height - bmi - age -> fibromyalgia 
It seems that hight looses it statistical significany (even though by a very close margin) when we include age. This might be due to the fact that people tends to lose some height as they grow older after a certain age because of the spine compression and posture problems.

### weight - bmi -> fibromyalgia 
For weight, the odds ratio of 0.987 indicates that for each unit increase in weight (in kilograms), the odds of having fibromyalgia decrease by approximately 1.3% (since 1 - 0.987 = 0.013 or 1.3%). For BMI, the odds ratio of 1.123 suggests that for each unit increase in BMI, the odds of having fibromyalgia increase by about 12.3%. The VIF (Variance Inflation Factor) values for both weight and BMI are around 6.970, indicating some level of multicollinearity, but it is generally considered acceptable as it is below 10.

### weight - bmi - age -> fibromyalgia 
For weight, the odds ratio of 1.012 indicates that for each unit increase in weight (in kilograms), the odds of having fibromyalgia increase by approximately 1.2%.
For BMI, the odds ratio of 1.036 suggests that for each unit increase in BMI, the odds of having fibromyalgia increase by about 3.6%.
For age, the odds ratio of 1.163 indicates that for each unit increase in age (in years), the odds of having fibromyalgia increase by approximately 16.3%.
The VIF (Variance Inflation Factor) values indicate that there is some multicollinearity between weight and BMI (with VIFs around 7), but it is generally considered acceptable as it is below 10. Age shows a low VIF, indicating low multicollinearity with other variables.

In our case a unit increase in age is usually 5 year age gaps. Look at the notebook for more detail.

##### The fact that predictive power of weight stays stable but BMI lessens when we include age might be due to the fact that people grow shorter after a certain age which affects BMI.


### weight - skin area - age -> fibromyalgia 
Nothing significant because of high multicollinearity
### skin area - BMI - age -> fibromyalgia 
Effect of skin size independet of BMI is not significant





