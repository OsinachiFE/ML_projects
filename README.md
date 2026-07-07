# ML_projects
A curated collection of machine learning projects from university coursework and personal exploration, showcasing core techniques, model building, and applied problem-solving.
Mini Project - COMP7019
1. Business Overview: Airline Passenger Satisfaction
1.1 Overview
Airline passenger satisfaction is a key driver of customer loyalty, brand reputation, and long-term revenue. Understanding passenger experiences allows airlines to proactively improve services, reduce complaints, and increase repeat bookings.

This project focuses on predicting passenger satisfaction based on survey data covering travel experience, service quality, flight delays, and passenger demographics. By analyzing these factors, the airline can make data-driven decisions to enhance customer experience.

1.2 Reason for the Project
The airline industry is highly competitive, and retaining customers is critical. Passenger feedback indicates that even small service improvements, such as faster boarding, better WiFi, or more comfortable seating, can significantly impact satisfaction.

Currently, airlines rely on post-flight surveys and anecdotal feedback, which are reactive. Predictive modeling allows the airline to anticipate passenger dissatisfaction before it occurs and implement targeted interventions.

1.3 Business Objectives
The main objectives of this project are:

Predict Passenger Satisfaction: Identify passengers likely to be satisfied or dissatisfied based on their travel and service experience.
Identify Key Drivers of Satisfaction: Determine which factors (e.g., inflight WiFi, seat comfort, boarding process) most strongly influence passenger satisfaction.
Support Strategic Decisions: Provide actionable insights to improve services, optimize operations, and increase customer loyalty.
1.4 Expected Business Impact
Proactive Service Improvements: Focus on areas that most influence satisfaction to prevent dissatisfaction.
Enhanced Customer Loyalty: Increase repeat bookings by ensuring a consistently positive travel experience.
Operational Efficiency: Optimize resource allocation (e.g., staffing, in-flight services) based on predicted passenger needs.
Revenue Growth: Satisfied passengers are more likely to purchase premium services and recommend the airline to others, driving revenue.
By using predictive modeling to anticipate passenger satisfaction, the airline can move from a reactive to a proactive approach in managing customer experience, improving overall competitiveness in the market.

1.5 How the System Will Be Used
The predictive system will be integrated into the airline’s operational dashboard and used as follows:

Pre-Flight/Booking Phase: Flag passengers with higher risk of dissatisfaction based on their profile or travel history.
Operational Adjustments: Allocate resources such as premium support, seating adjustments, or priority boarding to improve satisfaction.
Post-Flight Analysis: Validate predictions against actual satisfaction surveys to refine and retrain the model.
Management Reporting: Provide actionable insights to service and marketing teams about key satisfaction drivers.
This system allows the airline to move from reactive service improvements to proactive, data-driven strategies.

1.6 Problem Framing
This is a supervised machine learning classification problem because:

We have a target variable: Satisfaction (Satisfied vs Neutral/Dissatisfied).
Input features include numerical and categorical variables such as age, flight distance, class, type of travel, and ratings for various services.
Alternative problem framings could include regression (predicting satisfaction on a continuous scale), but for practical business decisions, binary classification is sufficient.

1.7 Performance Measurement
Model performance will be measured using metrics that assess classification quality:

Accuracy: Overall percentage of correct predictions.
Precision & Recall: To understand how well the model identifies dissatisfied passengers (important for proactive interventions).
F1 Score: Balances precision and recall, useful for imbalanced datasets.
Confusion Matrix: To visualise correct and incorrect classifications.
High accuracy is important, but the business priority is correctly identifying passengers at risk of dissatisfaction, so precision and recall are critical.

1.8 Comparable Problems and Tools
This problem is similar to:

Customer churn prediction: Predicting whether a customer will leave a service.
Product satisfaction analysis: Predicting satisfaction scores based on service or product features.
Hotel or airline review prediction: Using structured survey data to forecast ratings.
Tools and techniques from these domains, such as Random Forest, Gradient Boosting, SVM, and neural networks, can be directly applied. Feature importance methods and cross-validation strategies from churn prediction can also be reused.

1.9 Assumptions Made
Passenger satisfaction can be reasonably predicted using the available survey and travel data.
The dataset is representative of the airline’s passenger population.
Ratings from 0–5 for service aspects (e.g., seat comfort, online boarding) are reliable and consistently reported.
Passengers’ demographic attributes (age, type of travel) are useful predictors of satisfaction.
The business objective focuses on binary satisfaction (Satisfied vs Neutral/Dissatisfied), rather than predicting a multi-class or continuous score.
The operational environment allows the airline to act on predictions (e.g., adjust boarding, assign staff, or improve services).
These assumptions guide both data preprocessing and model selection, ensuring that the system is feasible and actionable.

2. Data Information
2.1 Data Requirements
To predict airline passenger satisfaction, the following data is required:

Data Category	Description	Reason for Use
Passenger Demographics	Gender, Age	Understand how different passenger types affect satisfaction
Travel Information	Customer type (loyal/disloyal), Type of travel (business/personal), Flight distance, Class	Capture passenger travel context and expectations
Service Ratings	Inflight WiFi, Online booking, Gate location, Food & Drink, Seat comfort, Inflight entertainment, Online boarding, Onboard service, Leg room service, Baggage handling, Check-in service, Inflight service, Cleanliness	Measure passenger experience across multiple service touchpoints
Operational Metrics	Departure delay, Arrival delay	Understand impact of delays on satisfaction
Target Variable	Satisfaction (Satisfied / Neutral or Dissatisfied)	Outcome to predict
The dataset contains 129,880 passenger survey responses, which is a large and representative sample for training machine learning models. This volume ensures that the models can learn complex patterns and generalize well to new data.

2.2 Data Source
The dataset comes from the US Airline Passenger Satisfaction Survey, publicly available online or provided for the assignment.
Structured in tabular format (CSV), with one row per passenger and columns representing features or target variables.
2.3 Legal, Privacy, and Ethical Considerations
The dataset is anonymized, containing no personally identifiable information (PII).
Usage is consistent with ethical standards for research and analytics.
Assumption: Data was collected with passenger consent for survey purposes.
2.4 Data Organization
Loaded into a pandas DataFrame for processing in Python.
Categorical variables (e.g., Gender, Class, Type of Travel) remain unencoded at this stage.
Numerical variables (e.g., Age, Flight Distance, Delay Minutes) are intact.
A copy of the raw dataset is maintained to preserve the original data for reproducibility.
