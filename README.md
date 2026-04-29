Customer Churn Analysis | Telecom

 Overview
 
Analyzed multi-month telecom customer data to identify early signals of churn and translate behavioral patterns into actionable retention strategies. The project focuses on **trend-based analysis and feature engineering** to uncover why customers disengage.

 Problem Statement
Customer churn leads to significant revenue loss in telecom businesses. The objective was to:
* Detect early behavioral indicators of churn
* Understand usage and revenue decline patterns
* Provide data-driven recommendations to reduce churn risk

 Dataset

Telecom customer activity data spanning **June–September**, including:
* Revenue metrics (ARPU)
* Call and data usage patterns
* Service engagement indicators
* Customer tenure (AON)

Churn was defined as low or no revenue activity in the final month.

 Approach

 1. Data Preparation
* Cleaned high-dimensional dataset (200+ features)
* Removed columns with excessive missing values (>70%)
* Standardized date formats and handled null values
* Constructed a custom churn label

 2. Feature Engineering
Engineered features to capture temporal behavior:
* Avg ARPU (Jun–Aug) → baseline customer value
* ARPU Drop (Aug → Sep) → churn signal
* Total Data Usage → engagement indicator

 3. Exploratory Analysis
Performed targeted EDA to compare churn vs non-churn segments:

* Revenue distribution across customer groups
* Usage decline patterns prior to churn
* Feature correlation analysis

 Key Findings
* Revenue decline is the strongest churn signal
* Customers with low engagement (data usage) show higher churn rates
* Early-stage users (low tenure) are more likely to churn
* Behavioral changes 1 month prior provide a clear churn indicator

 Business Impact
* Enables early identification of at-risk customers
* Supports targeted retention campaigns based on usage decline
* Helps prioritize high-value customers with falling engagement
* Demonstrates how simple behavioral features can drive decision-making without complex models

 Tech Stack
 
Python • Pandas • NumPy • Matplotlib • Seaborn

 Extensions
* Time-series churn analysis
* Cohort-based retention insights
* Interactive dashboard (Streamlit)

How to Run

Clone the repository:
git clone https://github.com/safrz110/Customer-Churn-Analysis

Install dependencies:
pip install -r requirements.txt

Launch Jupyter Notebook:
jupyter notebook

Future Improvements

Build predictive models for churn detection
Create interactive dashboards (Streamlit/Power BI)
Perform cohort and time-series analysis
Enhance feature engineering with domain-specific insights

Conclusion

This project demonstrates how exploratory data analysis and feature engineering can uncover meaningful customer behavior patterns. The insights derived can help telecom companies proactively reduce churn and improve customer retention strategies.

 Author
 
Sarfaraz Ali
