
Customer Churn Analysis (EDA)

Overview
This project analyzes customer churn in a telecom dataset to understand why customers leave and which groups are at higher risk.
The focus of this project is on data cleaning, exploratory data analysis, and drawing business insights using Python.
No machine learning models are used, as the goal is to strengthen core data analysis skills.

This is my second data analysis project, built after a sales EDA project.

Dataset
The dataset contains around 7000 customer records with 21 columns.
It includes information such as customer tenure, contract type, monthly charges, total charges, internet services, support services, and demographic indicators.

The target column is Churn, where
1 means the customer left
0 means the customer stayed

Tools Used
Python
Pandas
Matplotlib
Seaborn
Jupyter Notebook

Data Cleaning
The following preprocessing steps were performed:

CustomerID was removed as it is only an identifier and not useful for analysis.
TotalCharges was converted from object type to numeric, with missing values handled for new customers.
Yes/No columns were converted into binary values (0 and 1).
Inconsistent categorical values such as "No internet service" were standardized.

Key Questions Explored

Does customer tenure affect churn?
Are higher monthly charges associated with churn?
How does contract type influence churn?
Does internet service type impact churn?
Do support services such as TechSupport and OnlineSecurity reduce churn?
Do senior citizens churn more than non-senior customers?

Main Insights

Contract type is the strongest driver of churn.
Month-to-month customers show very high churn, while long-term contract customers are much more stable.

Churn is concentrated in early customer tenure.
Customers who leave usually do so within the first few months, while long-term customers tend to stay.

Higher monthly charges are linked to higher churn.
Customers paying more per month are more likely to leave, especially when expectations are not met.

Internet service type strongly affects churn.
Fiber optic customers have the highest churn, followed by DSL users.
Customers without internet service churn the least.

Support services reduce churn significantly.
Customers without TechSupport or OnlineSecurity churn at nearly double the rate of those who have them.

Senior citizens churn more than non-senior customers.
This effect appears to be influenced by pricing, contract type, and support needs rather than age alone.

Business Takeaways

Retention efforts should focus on month-to-month customers.
The early customer lifecycle is critical and needs better onboarding and support.
Support services should be bundled or promoted for high-end plans.
Senior customers may benefit from simpler plans and stronger support.
Retention budgets should not be wasted on low-risk long-term customers.

Conclusion
This analysis shows that customer churn is not random.
It is driven mainly by contract commitment, pricing, service quality, and access to support.
Simple exploratory data analysis techniques were sufficient to uncover strong and actionable business insights.
