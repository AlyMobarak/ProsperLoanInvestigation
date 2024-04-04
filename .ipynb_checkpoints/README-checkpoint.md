# Exploring Loan Data from Prosper
## by Aly Mobarak


## Dataset

> This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others. It comes from Prosper, an institution that introduced U.S. consumers to an innovative new approach to personal finance called peer-to-peer lending. Almost twenty years later, Prosper has helped over 1.7 million customers achieve financial well-being through a comprehensive suite of products.


## Summary of Findings

Univariate Observations

1. **Loan Status Distribution**: Most loans are in the "Current" status. This means that a majority of borrowers are actively repaying their loans. The "Completed" loans make up the second group, which shows that a good number of loans have been fully paid off. Finally, fewer loans are "Past Due", "Defaulted", or "Chargedoff", which points to a relatively healthy loan performance for Prosper. Great work!
2. **Prosper Score Distribution**: The Prosper Scores are mostly concentrated in the mid-range with the highest frequency at score 6. Very high and very low scores are less common, indicating that most borrowers are considered to be of moderate credit risk, typical of a financial institution like Prosper.
3. **Loan Term Frequencies**: The 36-month term is the dominant choice among borrowers. This is basically suggesting a preference for loans with a balance between monthly affordability and total interest cost. Shorter 12-month loans are least favored, while 60-month loans are less common, indicating that borrowers are less inclined towards both the higher monthly payments of short-term loans and the higher total interest of longer terms.
4. **Original Loan Amount Distribution**: There are several popular loan amounts with peaks around $4,000\$$, $10,000\$$, and $15,000\$$. The frequency of loans decreases for amounts greater than $15,000\$$, showing that larger loans are less common.
5. **Borrower APR Distribution**: The APRs vary widely, with a notable peak around 0.35, indicating that this rate is quite common among loans. The distribution suggests that while there is a range of interest rates applied, there is a clustering around certain APRs that are likely linked to specific borrower risk profiles.
6. **Listing Category Frequencies**: "Debt Consolidation" is the most common purpose for loans, significantly outnumbering other categories. Other frequent purposes include "Home Improvement" and "Business", while purposes such as "RV" and "Green Loans" are among the least common.
7. **Income Range Distribution**: Borrowers with income ranges between $25,000\$$ and $74,999\$$ dominate the platform, with fewer borrowers at the high and low ends of the income spectrum. This suggests that the platform is most frequently used by individuals with middle-income levels. This makes sense as people with high incomes won't readily rely on loans, and people with low income could be worried about interest rates.

Bivariate Observations

1. **Risk Assessment vs. Borrowing Costs**: There's a clear trend that shows as Prosper's Creditworthiness Score increases, the Borrower’s Annual Percentage Rate (APR) tends to decrease. This suggests that the Prosper Score is an effective measure for assessing credit risk and is used to determine the borrowing costs accordingly.
2. **Prosper Score vs. Fate of Loan**: Higher Prosper Scores generally correlate with a higher likelihood of loan completion and a lower likelihood of default or charge-off. This indicates that the Prosper Score is a reliable predictor of loan performance within the financial institution.
3. **Loan Original Amount vs. Monthly Loan Payment**: A direct relationship exists between the loan amount and the monthly payment, which means that higher loan amounts result in higher monthly payments. This relationship is expected, but the variability within loan amounts suggests that other factors like loan term and APR also affect the monthly payment amount.


Multivariate Observations

**Facet Plot Summary:**
This revealed that with shorter-term loans of 12 months, there is a noticeable trend where a higher Prosper Score correlates with a lower borrower APR. Additionally, for these shorter-term loans, the loan amounts are not particularly high. As we move to longer terms, such as 36 and 60 months, the same inverse relationship between Prosper Score and APR persists, but the loan amounts tend to be higher, likely due to the extended repayment period which reduces the monthly payment amount. Moreover, the presence of higher APRs for longer terms suggests that a compensation is often asked for the increased risk associated with longer loan durations. However, the wide range of loan amounts and APRs within specific Prosper Scores or loan terms suggests there are nuances in borrower profiles and loan structures not fully captured by the Prosper Score alone.

**Scatter Plot Summary:**
- Generally, the debt-to-income ratio is clustered at the lower end for most borrowers, regardless of the loan status. Borrowers on this platform typically do not have excessively high debt compared to their income.
- There is a range of APRs across all debt-to-income ratios, but particularly for debt-to-income ratios below 2, suggesting that factors other than the debt-to-income ratio may play a more significant role in determining APR.
- The size of the dots, representing the Prosper Score, does not show a clear pattern in relation to APR and debt-to-income ratio.
- Notably, loans that are "Chargedoff" or "Defaulted" do not seem to be confined to any specific debt-to-income range. This shows that the default is influenced by a complex interplay of factors beyond just the borrower's debt level relative to their income.

This overall analysis points out that while the Prosper Score, loan term, and debt-to-income ratio provide a framework for understanding loan performance and cost, the relationship between these factors is intricate. Other hidden variables or external factors may influence the loan outcome and APR. Ultimately, the analysis underscores the multifaceted nature of lending risk and the need for comprehensive risk assessment models.

## Key Insights for Presentation

1. **The Relationship Between Prosper Score and Loan Outcomes**:
   - **Design Changes**: Clearer labeling for the Prosper Score categories and more distinct color coding for different loan statuses. Simplified the loan status by classifying them into only two categories: successful payment (completed or near complete) and unsuccessful (chargedoff, pastdue, and defaulted).

2. **Loan Amount, Term, and Monthly Payment Dynamics**
   - **Design Changes**: Color coded term to drive my observations home and make them clearer.