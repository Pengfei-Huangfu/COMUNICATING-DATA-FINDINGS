# COMUNICATING-DATA-FINDINGS
ANALYZE ON PROSPER LOAN DATA
### by Pengfei Huangfu

## Dataset

the dataset contains 113,937 loans with 81 variables. There are so many variables in this dataset. it is hard to find the main features of interest by just looking at the dataset. After some analysis I found that some features are more interesting than others. Through out the project I will work with Borrower APR, Prosper Score, Credit Score, Original Loan Amount, Borrower Occupation, Borrower State, Borrower Employment Status and some other feature if it seems interest later on. in my preliminary analysis, i selected columns that i was interested in to make futher investigation.

The dataset can be download here: https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv&sa=D&ust=1547358770029000
 
 ## Summary of Findings
after analyzing the main features of interest, i find that the distribution of borrowers APR looks multimodal. interestingly, there is a strong concentration at around 0.35. There are no unusual points and no need to perform any transformations. california, texas and new york are the states with biggest numbers of loans. besides, most loans have a life span either 3 years or 5 years.
It was also noticed there are some outliers in the StatedMonthlyIncome that are too far away from most of the values, in some charts these outliers are igonred by limiting the axis values.

The borrower APR is negatively correlated with the loan original amount, Prosper Score and Stated Monthly income. And also, the borrower APR is strongly and positively correlated to Lender Yield. On average, employed people got larger original amount than unemployed, part-time and retired people.

It was also noticed there are some outliers in the StatedMonthlyIncome that are too far away from most of the values, in some charts these outliers are igonred by limiting the axis values. Bar plot is very useful for  to make a clear rank from high to low and figure out what are the most frequent category for each variables.

## key Insight
1. Full-Time and part-time tend to have higher ProsperScore and lower BorrowerAPR
2. Not-Employed & Self-Employed tend to have lower ProsperScore and higher BorrowerAPR
3. Retired people have higher ProsperScore and lower BorrowerAPR
4. It was important and unsurprising to notice the fact that loans with higher LoanOriginalAmount are mostly taken by people with higher Prosper Score.
5. based on my data findings, lender yield, Prosper Score and Original Loan Amount could be input of machine learning algorithm to predict the Borrower APR. futher statistical analysis can be done to see whether they are good predictors or not.
