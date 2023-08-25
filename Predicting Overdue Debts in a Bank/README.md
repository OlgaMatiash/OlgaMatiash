# Borrowers Reliability Study

The **Borrowers Reliability Study** project involves analyzing client data from the credit department of a bank to determine whether factors like marital status and the number of children impact the timely repayment of loans. The project aims to provide insights that can be used in building a credit scoring model, which assesses a potential borrower's ability to repay a loan.

## Project Overview

1. **Data Overview**
   - Analyze the dataset to understand its structure and content.
   - Handle missing values, anomalies, and duplicate values.

2. **Exploratory Data Analysis**
   - Utilize `pandas`, `matplotlib`, and `seaborn` for data analysis and visualization.
   - Explore columns such as 'children', 'days_employed', 'dob_years', 'education', 'family_status', 'gender', 'income_type', 'debt', 'total_income', and 'purpose'.

3. **Data Preprocessing**
   - Address missing values in the 'days_employed' and 'total_income' columns.
   - Clean and categorize data in the 'education', 'family_status', and 'purpose' columns.
   - Remove outliers in the 'days_employed' column.
   - Categorize income levels based on 'total_income'.

4. **Loan Purpose Categorization**
   - Create a function to categorize loan purposes into common categories.
   - Generate a new column 'purpose_category' to store the categorized purposes.

5. **Data Analysis and Insights**
   - Analyze correlations between factors like the number of children, marital status, income level, loan purpose, and timely loan repayment.
   - Answer questions regarding these correlations using pivot tables and data visualization.

## Results and Conclusion

- The analysis indicates that factors like the number of children, marital status, income level, and loan purpose have limited influence on the likelihood of timely loan repayment.
- Through data preprocessing and analysis, missing values, anomalies, and duplicates have been addressed to ensure the accuracy of the insights.
- This project showcases the use of data exploration, cleaning, categorization, and analysis techniques to draw meaningful conclusions from a real-world dataset.

Feel free to explore the detailed code and analysis in the project files to gain deeper insights into each step of the process.

For any questions or further details, feel free to contact me.
