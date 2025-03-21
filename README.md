
# Lead Scoring Analysis for X Education

## Project Overview
This project aims to build a **Lead Scoring Model** for X Education, an online course provider, to enhance lead conversion rates. The model assigns a score (0-100) to each lead, helping the sales team prioritize high-potential leads efficiently.

**Challenge:** Low lead conversion rate (~30%) despite generating numerous leads daily. 
**Objective:** Develop a Lead Scoring Model using Logistic Regression. 
**Approach:** Assign a lead score between 0 and 100 to prioritize potential leads. 
**Goal:** Improve sales efficiency and increase the conversion rate to ~80%. 


## Repository Structure
This repository contains multiple files that document the entire process of building and evaluating the **Logistic Regression Model** used for lead scoring.

###  Files and Their Purpose

1. **Final - Logistic Regression Model - Education - Group Case Study.ipynb**
   - This Jupyter Notebook includes **data preprocessing, feature selection, model training, and evaluation**.
   - Steps covered:
     - Handling missing values and categorical encoding.
     - Recursive Feature Elimination (RFE) and Variance Inflation Factor (VIF) analysis for feature selection.
     - Logistic Regression Model training and performance evaluation.
     - Selection of **cut-off point (0.25)** based on Sensitivity-Specificity Intersection.
     - Final lead scoring assignment.

2. **Leads.csv**
   - The original dataset containing lead information such as **lead source, user activity, and engagement**.
   - The dataset has been preprocessed before modeling.

3. **Leads Data Dictionary.xlsx**
   - This file provides a description of each feature in the dataset, including categorical and numerical variables.

4. **Lead Score Assignment Presentation.pdf**
   - A PowerPoint-style presentation summarizing the **model building process, insights, and recommendations** for business stakeholders.

5. **Brief Summary Report.pdf**
   - A concise document explaining the **approach, key findings, and business takeaways** from the lead scoring analysis.

6. **Assignment Subjective Questions - Answer Included.pdf**
   - Contains additional insights and responses to subjective questions related to the model.

## Model Performance Summary
The model demonstrates **strong generalization** with the following performance metrics:

| Metric                    | Train Set  | Test Set  |
|---------------------------|-----------|-----------|
| **Accuracy**              | 91.3%     | 90.4%     |
| **Sensitivity (Recall)**  | 91.8%     | 91.7%     |
| **Specificity**           | 91%       | 89.7%     |
| **False Positive Rate**   | 9%        | 10%       |
| **Positive Predictive Value** | 86.5% | 83%       |
| **Negative Predictive Value** | 94.6% | 95.1%     |

## Business Recommendations
1. **Focus on Key Features for Lead Conversion:**
   - The **most influential variables** include **Total Time Spent on Website, Lead Source (Welingak Website), and Tags - Lost to EINS**.
   - Leads with **higher time spent** on the website are more likely to convert.
   - Leads from **Welingak Website** have a higher conversion rate compared to other sources.

2. **Improve Engagement Strategies:**
   - **Follow-up SMS and Emails** can enhance lead conversion rates.
   - Leads with **Last Notable Activity as SMS Sent** have a higher likelihood of conversion, indicating the effectiveness of direct communication.

3. **Optimize Lead Scoring for Business Cycles:**
   - During peak sales seasons (e.g., internship hiring), **increase outreach efforts** for high-scoring leads.
   - When conversion targets are met early, **focus on leads with higher positive predictive value** to minimize unnecessary follow-ups.
