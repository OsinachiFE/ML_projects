# Airline Passenger Satisfaction Prediction

## Project Overview

This project develops a machine learning system to predict airline passenger satisfaction using survey data containing passenger demographics, travel information, service ratings, and flight operational factors.

The goal is to help airlines move from reactive customer service management to a proactive approach by identifying passengers who are likely to be dissatisfied and understanding the key factors that influence satisfaction.

## Business Objectives

* Predict whether passengers are satisfied or neutral/dissatisfied based on their travel experience.
* Identify the main drivers of passenger satisfaction.
* Provide actionable insights to improve customer experience, loyalty, and operational decision-making.

## Dataset

The project uses the US Airline Passenger Satisfaction Survey dataset containing 129,880 passenger records.

Features include:

* Passenger demographics (Age, Gender)
* Travel information (Customer Type, Travel Type, Class, Flight Distance)
* Service ratings (WiFi, Seat Comfort, Online Boarding, Entertainment, Food & Drink, Cleanliness, etc.)
* Operational factors (Departure and Arrival Delays)

Target variable:

* **Satisfaction**: Satisfied vs Neutral/Dissatisfied

## Methodology

The project follows an end-to-end machine learning workflow:

1. Data cleaning and preprocessing
2. Exploratory data analysis
3. Feature engineering and selection
4. Model training and evaluation
5. Feature importance analysis
6. Business insight generation

Several classification algorithms were evaluated, including ensemble models, with Random Forest selected as the final model.

## Results

The tuned Random Forest model achieved:

* **Accuracy:** 96.28%
* **AUC Score:** 0.99
* **5-Fold Cross-Validation Score:** 95.77%
* **Recall for dissatisfied passengers:** 0.98

The model demonstrates strong predictive performance and can reliably identify passengers at risk of dissatisfaction.

## Key Insights

Feature importance analysis identified the strongest satisfaction drivers:

* Online Boarding
* Inflight WiFi Service
* Inflight Entertainment
* Seat Comfort
* Leg Room Service

These findings show that digital services and onboard experience have a major impact on passenger satisfaction.

## Business Impact

The predictive system enables airlines to:

* Detect dissatisfied passengers early
* Improve service recovery strategies
* Prioritise investment in high-impact service areas
* Enhance customer loyalty and retention

## Future Improvements

* Deploy the model into a real-time dashboard using the exported model.
* Reduce survey complexity by focusing on the most influential features.
* Retrain the model regularly to adapt to changing passenger expectations.
