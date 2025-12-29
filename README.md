# STEM-Income-Analysis_R
# STEM vs. Non-STEM Degrees: Income Analysis
# Statistical Modeling Project | UT Austin (SDS 320E) 

# Overview
This project evaluates the relationship between degree types (STEM vs. Non-STEM), age, and real income among employed workers in the US. Utilizing multivariate linear regression, I evaluated whether the public assumption of "STEM premium" is true when controlling for age.

# Key Results
- Degree Type (STEM/Non-STEM): On average, individuals with a STEM degree earned $12,540 more than those with a non-STEM degree (p = 0.033).
- Age: Each additional year of age was associated with an expected income increase of $905 (p < 0.001).
- Statistical Significance: Both age and degree type were found to be significant predictors of real income in this sample.

# Methods
- Language: R
- Environment: R Studio
- Statistical Method: Multivariate Linear Regression
- Diagnostics: Performed residual analysis to test for linearity, normality, and equal variance. Identified right-skewed residuals and a funnel shape, indicating areas for future model refinement.

# Descriptions
- `project_sampleFINAL1.csv`: The filtered dataset used for analysis.
- `[SDS 320E] Final Project.pdf`: The complete final presentation report.
- `FinalProject.R`: R script for data processing and visualization. (Will be posted soon.)

# Conclusion & Future Research
- While the model found significant predictors (p < 0.05), the adjusted R^2 of 0.074 suggests that 92.6% of income variation is explained by factors outside this model (e.g., occupation, location, and industry). 
- A key limitation of this current analysis is that outliers were not removed from the dataset, which is evidenced by the right-skewed residuals and the funnel shape in the residual scatter plot. These high-income outliers significantly affected the model's fit and contributed to the lower R^2 value.
- In future research, I plan to:
1. Handle Outliers: Implement robust data cleaning techniques to identify and manage outliers that skew the distribution.
2. Expand Predictors: Incorporate additional key variables such as work experience, specific occupation, and geographical location to improve the model's explanatory power and predictive accuracy.
