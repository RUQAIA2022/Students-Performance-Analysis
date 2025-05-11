
Algorithms for Students Performance Analysis:

1. Hypothesis Testing Algorithm (Question a)
Algorithm: Test Preparation Course Impact Analysis
Input: StudentsPerformance dataset with math, reading, writing scores and test preparation status
Output: Hypothesis test results and visualizations

1. Load and preprocess the dataset
2. Split math scores into two groups:
   - Group 1: Students who completed test preparation (completed)
   - Group 2: Students who didn't complete test preparation (none)
   
3. Perform Welch's t-test (unequal variance) between groups:
   a. Calculate t-statistic and p-value for math scores
   b. Check variance equality using Levene's test
   
4. Visualize score distributions:
   a. Create overlapping histograms with KDE for both groups
   b. Add appropriate labels and legend
   
5. Repeat t-tests for reading and writing scores
6. Interpret results:
   - If p-value < 0.05: Significant effect
   - Else: No significant effect
2. Correlation Analysis Algorithm (Question b)
Algorithm: Score Correlation Analysis
Input: StudentsPerformance dataset with math, reading, writing scores
Output: Correlation matrix and heatmap visualization

1. Select numerical score columns (math, reading, writing)
2. Compute Pearson correlation matrix:
   a. Calculate pairwise correlations
   b. Store in matrix format
   
3. Visualize correlation matrix:
   a. Create heatmap with annotated values
   b. Use color gradient (coolwarm) to show strength
   
4. Identify strongest positive correlation:
   a. Exclude diagonal and lower triangle
   b. Find maximum correlation pair
   
5. Note potential multicollinearity issues
3. Linear Regression Modeling Algorithm (Question c)
Algorithm: Math Score Prediction Model
Input: StudentsPerformance dataset with encoded test preparation status
Output: Regression model summary and diagnostics

1. Feature engineering:
   a. Encode test preparation course (none→0, completed→1)
   
2. Build OLS regression model:
   a. Dependent variable: math score
   b. Independent variables: reading score and test preparation status
   
3. Fit model and compute statistics:
   a. Calculate coefficients and p-values
   b. Compute R-squared and other metrics
   
4. Generate model summary report
5. Interpret coefficients:
   a. Effect of reading score on math score
   b. Effect of test preparation on math score
   
6. Create residual plot:
   a. Plot fitted values vs residuals
   b. Add LOWESS smoothing line
   
7. Check model assumptions via visual diagnostics
These algorithms systematically analyze the relationship between test preparation and academic performance, examine correlations between different test scores, and build a predictive
model for math performance based on reading scores and test preparation status.


