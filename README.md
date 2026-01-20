Customer Churn Analysis (EDA)
Overview

This project explores customer churn in a telecom dataset to understand why customers leave and which groups are at higher risk.
The focus is on data cleaning, exploratory data analysis (EDA), and business insights, not predictive modeling.

This is my second data analysis project, built after a sales EDA project, to strengthen my understanding of real-world datasets and analytical thinking.

Dataset

~7,000 customer records

21 features including:

Contract type

Tenure

Monthly & total charges

Internet services

Support services

Demographics

Target variable: Churn (1 = churned, 0 = retained)

Tools Used

Python

Pandas

Matplotlib

Seaborn

Jupyter Notebook

Data Cleaning

Key preprocessing steps:

Dropped customerID (identifier, not useful for analysis)

Converted TotalCharges from object to numeric

Handled missing values caused by new customers

Encoded Yes/No variables into binary (0/1)

Ensured consistency in categorical values (e.g. “No internet service” → “No”)

Key Questions Explored

Does churn depend on customer tenure?

Are higher monthly charges linked to churn?

How does contract type affect churn?

Does internet service type matter?

Do support services reduce churn?

Are senior citizens more likely to churn?

Main Insights

Contract type is the strongest churn driver

Month-to-month customers churn far more than long-term contract customers.

Churn happens early

Customers with short tenure are much more likely to leave.

Long-term customers are relatively stable.

Pricing and expectations matter

Higher monthly charges are associated with higher churn.

Fiber optic users show the highest churn rates.

Support services reduce churn

Customers without TechSupport or OnlineSecurity churn almost twice as much.

Support acts as a protective factor.

Senior citizens churn more

Senior customers show significantly higher churn, likely influenced by pricing, contract flexibility, and support needs.

Overall, churn appears to be driven more by service quality, pricing, and commitment level than by demographics alone.

Business Takeaways

Focus retention efforts on month-to-month customers

Improve early-stage customer experience

Bundle or promote support services for high-end plans

Design simpler, support-focused plans for senior customers

Avoid spending retention budget on low-risk long-term customers

Conclusion

This analysis shows that customer churn is not random and can be addressed through better contract strategies, pricing alignment, and service support.
The project demonstrates how simple EDA techniques can lead to meaningful business insights.
