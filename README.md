# MechaCar_Statistical_Analysis

##Overview
AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management would like a review of the production data for insights that may help the manufacturing team.

##Results

Deliverable 1

![Photo_1](https://user-images.githubusercontent.com/105950742/189543840-28d7ef7d-9ce7-4561-b9e8-8ef3cbf32236.png)

From the above output we can see that:

The vehicle length, and vehicle ground clearance are statistically likely to provide non-random amounts of variance to the model. The vehicle length and vehicle ground clearance have a significant impact on miles per gallon on the MechaCar prototype.

The  p-Value: 5.35e-11, is much smaller than the assumed significance level of 0.05%. This indicates there is sufficient evidence to reject our null hypothesis.

This linear model has an r-squared value of 0.7149, which means that approximately 71% of all mpg predictions will be determined by this model.

Deliverable 2

The Suspension Coil dataset provided for the MechaCar contains the results of testing the weight capacities of multiple suspension coils from multiple production lots to determine consistency.

All manufacturing lots:

![Photo_2](https://user-images.githubusercontent.com/105950742/189543834-639d510e-fb26-4261-969c-47945cabd050.png)

Each Lot (3):

![Photo_3](https://user-images.githubusercontent.com/105950742/189543836-95074aa2-cdd1-410a-8b92-03790c23830a.png)

The MechaCar suspension coils mandate that the variance of the suspension coils cannot exceed 100 pounds per square inch (PSI). When looking at the entire population of the production lot, the variance of the coils is 62.29 PSI, which is well within the 100 PSI variance requirement.

Similarly, but significantly more consistent, Lot 1 and Lot 2 are well within the 100 PSI variance requirement; with variances of 0.98 and 7.47 respectively. However, it is Lot 3 that is showing much larger variance in performance and consistency, with a variance of 170.29. It is Lot 3 that is disproportionately causing the variance at the full lot level.

Boxplot shpwing the differences between the lots:

![Rplot](https://user-images.githubusercontent.com/105950742/189543839-37a27f65-c9d6-4a30-b8ab-860155a602cb.png)

Deliverable 3

![Photo_5](https://user-images.githubusercontent.com/105950742/189544000-97f70b2a-50f1-4e6b-9222-4163664b60c9.png)

Lot 1 sample actually has the true sample mean of 1500, again as we saw in the summary statistics above. With a p-Value of 1, clearly we cannot reject the null hypothesis that there is no statistical difference between the observed sample mean and the presumed population mean (1500).

![Photo_6](https://user-images.githubusercontent.com/105950742/189543999-93a879f6-f360-4841-b74b-0f51d7dba56f.png)

Lot 2 has essentially the same outcome with a sample mean of 1500.02, a p-Value of 0.61; the null hypothesis cannot be rejected, and the sample mean and the population mean of 1500 are statistically similar.

![Photo_4](https://user-images.githubusercontent.com/105950742/189544046-8ec7c46b-b47b-4b50-b32d-1daeed49ed0e.png)

However, Lot 3,the sample mean is 1496.14 and the p-Value is 0.04, which is lower than the common significance level of 0.05. All indicating to reject the null hypothesis that this sample mean and the presumed population mean are not statistically different.


Deliverable 4:

Metrics

Safety Feature Rating: Independent Variable
Current Price (Selling): Dependent Variable
Drive Package : Independent Variable
Engine (Electric, Hybrid, Gasoline / Conventional): Independent Variable
Resale Value: Independent Variable
Average Annual Cost of ownership (Maintenance): Independent Variable
MPG (Gasoline Efficiency): Independent Variable

Hypothesis: Null and Alternative
Null Hypothesis: MechaCar is priced correctly based on its performance of key factors for its genre.

Alternative Hypothesis: MechaCar is NOT priced correctly based on performance of key factors for its genre.

Statistical Tests

A multiple linear regression would be used to determine the factors that have the highest correlation/predictability with the list selling price (dependent variable); which combination has the greatest impact on price (it may be all of them!)
