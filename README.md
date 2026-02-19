Customer Churn Analysis (EDA)

Project Overview

This project performs Exploratory Data Analysis (EDA) on a telecom customer dataset to understand the key drivers behind customer churn.

The objective is to analyze customer behavior, identify high-risk groups, and extract actionable business insights using Python. No machine learning models are used in this project. The focus is on data cleaning, structured analysis, and business interpretation.

This is the second data analysis project, built after a sales EDA project.


Problem Statement

Customer churn directly impacts company revenue. Understanding which customers are likely to leave and why is critical for improving retention strategies. This project analyzes churn patterns based on tenure, pricing, contracts, services, and demographics.


Dataset Information

- Approximately 7000 customer records
- 21 columns
- Features include:
  tenure
  contract type
  monthly charges
  total charges
  internet services
  support services
  senior citizen indicator
  and more

Target Variable:
Churn
1 = Customer left
0 = Customer stayed


Tools and Technologies Used

- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook


Data Cleaning and Preprocessing

The following preprocessing steps were performed:

- Removed CustomerID as it is only an identifier
- Converted TotalCharges from object type to numeric
- Handled missing values for new customers
- Converted Yes/No columns into binary format (0 and 1)
- Standardized inconsistent categorical values such as "No internet service"


Key Questions Explored

- Does customer tenure affect churn?
- Are higher monthly charges associated with churn?
- How does contract type influence churn?
- Does internet service type impact churn?
- Do support services such as TechSupport and OnlineSecurity reduce churn?
- Do senior citizens churn more than non-senior customers?


Main Insights

- Contract type is the strongest driver of churn. Month-to-month customers show significantly higher churn compared to one-year and two-year contracts.

- Churn is concentrated in early tenure. Customers who leave typically do so within the first few months.

- Higher monthly charges are linked to higher churn rates.

- Fiber optic customers have the highest churn compared to DSL and customers without internet service.

- Customers without TechSupport or OnlineSecurity churn at nearly double the rate of those who have these services.

- Senior citizens show higher churn rates, though this appears influenced by pricing, contract type, and support needs rather than age alone.


Business Takeaways

- Focus retention strategies on month-to-month customers.
- Improve onboarding experience during the early customer lifecycle.
- Bundle or promote support services for high-value plans.
- Provide better assistance and simpler plans for senior customers.
- Allocate retention budget strategically toward high-risk segments.


Skills Demonstrated

- Data Cleaning and Transformation
- Categorical Encoding
- GroupBy and Aggregation
- Business Insight Extraction
- Visualization and Interpretation
- Risk Segmentation Analysis


Project Structure

customer-churn-analysis/
|
|-- churn_analysis.ipynb
|-- telecom_churn.csv
|-- README.md


How to Run

1. Clone the repository
2. Install required libraries:
   pip install pandas matplotlib seaborn
3. Open Jupyter Notebook:
   jupyter notebook churn_analysis.ipynb


Conclusion

This analysis demonstrates that customer churn is not random. It is strongly influenced by contract commitment, pricing, service type, and access to support services. Structured exploratory analysis was sufficient to uncover clear and actionable business insights.
