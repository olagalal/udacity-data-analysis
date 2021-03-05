# Loan Data Exploration
## by Ola Galal


## Dataset

This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others. The dataset can be downloaded from [here](https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv), 
with documentation available [here](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0)

In this exploration, I wanted to look at the characteristics of loans that could be used to predict their borrower APR. The main focus was on the original loan amount, borrower's Prosper rating, loan term, borrower's stated monthly income. Also, I will try to solve the following questions:

##### What factors affect a loan’s outcome status?
##### What affects the borrower’s APR or interest rate?
##### Are there differences between loans depending on how large the original loan amount was?

## Summary of Findings

From all visualizations created from univariate exploration to multivariate exploration, many variable are found to be negatively correlated to BorrowerAPR, whereas ProspoerScore gives the strongest negative relationship.

## Key Insights of Presentation

1. The distribution of APR looks multimodal. A small peak centered at 0.1, a large peak centered at 0.2. There is also a small peak centered 0.3. Additionally, there is a very shape peak between 0.35 and 0.36. Only very few loans have APR greater than 0.43.

2. Listing Categories indicates that most of Prosper loans are debt consolidation. And, its followed by not available and other kinds of loans, indicating that Prosper should do a better job to correctly classify its loans.

3. The CurrentCreditLines and OpenRevolvingAccounts dimensions are all highly correlated with one another. 

4. The  Prosper Rating assigned at the time the listing was created: 0 - N/A, 1 - HR, 2 - E, 3 - D, 4 - C, 5 - B, 6 - A, 7 - AA.  Applicable for loans originated after July 2009. The plot show a strong relation between the score factor and borrower's rate. We see that the higher the score, the lower the rate.

5. The plot show that at different size of the loan amount, the APR has a large range, but the range of APR decrease with the increase of loan amount.

6. There are negative correlation between CreditScoreRangeUpper and BorrowerAPR. And Also from the right-side plot, ProsperScore has negative correlation with BorrowAPR.