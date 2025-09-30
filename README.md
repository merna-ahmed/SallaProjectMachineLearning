Project Summary
This project represents one of the first practical steps into Machine Learning, focusing on forecasting call volumes using real call center data. The main objective was to predict the Forecasted Calls for the upcoming three months (May, June, and July).

Dataset Features included:
Forecasted Calls
Calls Offered
Calls Handled
Calls Handled Within Threshold
ASA (Average Speed of Answer)
Answer Time
Agent Name
Methods Applied:
Simple Linear Regression (sklearn)
Input (X): Calls Offered
Target (y): Forecasted Calls

Multiple Linear Regression (sklearn)
Added additional features such as Calls Handled and Calls Handled Within Threshold
Compared Actual Forecasted Calls vs. Predicted Calls → Results showed a strong similarity, especially around the main data peaks

Time Series Forecasting (Prophet by Meta)
Modeled the time component to capture long-term patterns
Forecast revealed an upward trend in call volumes for the coming months
However, wide uncertainty intervals highlight the limitations of the relatively small dataset

Visualizations:
Density plots comparing actual vs. predicted distributions (showed strong overlap with minor differences at the extremes)
Forecast plots from Prophet showing trends and uncertainty intervals

Libraries Used:
pandas, matplotlib, seaborn → Data preprocessing & visualization
sklearn → Regression models
prophet → Time series forecasting

Key Insights:
Regression models captured the general relationship between offered and forecasted calls with good accuracy.
Time series analysis revealed an overall increasing trend in call volumes but emphasized the need for larger datasets to reduce uncertainty.
The project demonstrates how machine learning models can learn from real-world data and generate predictions that align with actual business trends.
