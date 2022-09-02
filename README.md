# Prosper-Loan

# **Prosper Loan Data Exploration** 

by ***Adeniran Ridwan***

**Dataset**

The dataset used for this project is called the Prosper Loan Dataset provided by udacity. This dataset consists of borrowers and loan's informations with 113,937 rows and 81 features.

During analysis, a subset dataset was created to focus on only the features of interest.

The features of interest:

- ListingKey: Unique key for each listing, same value as the 'key' used in the listing object in the API.
- ListingCreationDate: The date the listing was created.
- MemberKey: The unique key that is associated with the borrower. This is the same identifier that is used in the API member object.
- EmploymentStatus:The employment status of the borrower at the time they posted the listing.
- Occupation:The Occupation selected by the Borrower at the time they created the listing.
- IncomeVerifiable: The borrower indicated they have the required documentation to support their income.
- StatedMonthlyIncome: The monthly income the borrower stated at the time the listing was created.
- IncomeRange: The income range of the borrower at the time the listing was created.
- BorrowerAPR:The Borrower's Annual Percentage Rate (APR) for the loan.
- BorrowerRate:The Borrower's interest rate for this loan.
- BorrowerState: The two letter abbreviation of the state of the address of the borrower at the time the Listing was created.
- DebtToIncomeRatio: The debt to income ratio of the borrower at the time the credit profile was pulled. This value is Null if the debt to income ratio is not available. This value is capped at 10.01 (any debt to income ratio larger than 1000% will be returned as 1001%).
- IsBorrowerHomeowner: A Borrower will be classified as a homowner if they have a mortgage on their credit profile or provide documentation confirming they are a homeowner.
- CreditScoreRangeLower: The lower value representing the range of the borrower's credit score as provided by a consumer credit rating agency.
- CreditScoreRangeUpper: The upper value representing the range of the borrower's credit score as provided by a consumer credit rating agency.
- LoanStatus: The current status of the loan: Cancelled, Chargedoff, Completed, Current, Defaulted, FinalPaymentInProgress,
- LoanKey: Unique key for each loan. This is the same key that is used in the API.
- LoanOriginalAmount: The origination amount of the loan.
- Term: The length of the loan expressed in months.
- LoanOriginationDate: The date the loan was originated.
- LoanOriginationQuarter: The quarter in which the loan was originated.
- ClosedDate: Closed date is applicable for Cancelled, Completed, Chargedoff and Defaulted loan statuses.
- TotalProsperLoans: Number of Prosper loans the borrower at the time they created this listing. This value will be null if the borrower had no prior loans.

**Summary of Findings:**

During the investigation of the Prosper Loan, I focused more on the specific features of interest listed. Exploratory analysis was performed on individual variables as well as the relationship between two or more variables.

From the Univariant Analysis, It was deduced that Most borrowers are employed,very few of them are retired, they are mostly Professional and least of them are clerical. many of the borrower have an income range from ($)25,000-74,999 and most of them have stated monthly income that is less than 5000 Their income ratio is right skewed. Exploring the distribution of different states,it was found out that the state CA have the highest number of borrowers. Most loans were Listed and originated on Tuesday while the least was Listed on Sunday and originated on monday. This year 2013 have the highest count of loan origination

From the Bivariant Exploration during which the relationship between two features were studied. At first, the correlations between different numerical features was discovered with heatmap, the correlation between the Borrower APR and Borrower Rate was the highest which is 0.99. moreso, It was discovered that the borrower interest Rate and loan original amount are negatively correlated, which means the more the loan amount, the lower the Borrower Rate. however,The loan original amount is positively correlated to the stated monthly income. That is, the higher their stated monthly income, the higher the loan amount borrowed.

The relationship between the each Employment status and original loan amount shows that those who are employed and fulltime on average take out larger loans than other groups. in the case of original loan amount and terms,their relationship indicates that the higher the orignal amount of the loan, the higher length of the loan express in months.

Investigating further on Multivariate Exploration where relationship between three or more features were studied and also explore how each of those feature influenced one another. It was deduced that those with an Income verifiable tends to borrow an higher amount of loan and have a longer term. Also Debt To Income were higher in 2007 when we have a term of 35 months

**Key Insights for Presentation**

For the presentation, I explore various features of interest to discover the relationship between the borrowers and the loans they took. shows how dependent and independent each feature are to another. Features include: Borrowers' employment status, their income range, stated monthly income and the loan original amount.
