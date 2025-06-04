# **Employee Turnover Prediction Model for Salifort Motors**

This repository contains my **capstone project** for the **Google Advanced Data Analytics Professional Certificate**. In this project, I applied data analytics techniques and machine learning models to predict employee turnover at **Salifort Motors**, a fictional alternative energy vehicle manufacturer. The goal was to identify key factors contributing to employee departure and build predictive models that can inform business decisions aimed at improving employee retention.

## **Table of Contents**
1. [Introduction](#1-introduction)
2. [Scenario](#2-scenario)
3. [PACE Stages](#3-pace-stages)
4. [Result](#4-result)
5. [Dataset](#5-dataset)
6. [Tools Used](#6-tools-used)
7. [Model Evaluation](#7-model-evaluation)
8. [Insights and Recommendations](#8-insights-and-recommendations)
9. [Conclusion](#9-conclusion)
10. [Files in this Repository](#10-files-in-this-repository)

---

## **1. Introduction**

This project is part of my **capstone** for the **Google Advanced Data Analytics Professional Certificate**. The objective was to address a real-world business problem: understanding what factors contribute to employee turnover at **Salifort Motors** and using this information to predict future employee departures. The project involved analyzing a dataset of employee surveys and applying data analytics and machine learning techniques to derive actionable insights.

The primary question addressed was: **What’s likely to make an employee leave the company?** To answer this, I analyzed various employee characteristics (such as satisfaction level, department, number of projects, and monthly hours worked) and built predictive models to forecast employee turnover.

---

## **2. Scenario**

Salifort Motors is experiencing high employee turnover, which is not only costly in terms of recruitment and training but also disrupts operations and company culture. To address this, the HR department conducted a survey to understand employee sentiments and gather data that could explain why employees are leaving.

The HR department has tasked me with:
- Analyzing the employee survey data to identify key factors driving turnover.
- Building a model to predict the likelihood of an employee leaving the company.
- Providing actionable recommendations to improve employee retention.

### **Dataset Overview**
The dataset used for this analysis contains 15,000 rows and 10 columns, each representing important features of the employees. These features include both employee demographics and job-related variables.

| Variable                  | Description                                                 |
|---------------------------|-------------------------------------------------------------|
| **satisfaction_level**     | Employee-reported job satisfaction level [0–1]              |
| **last_evaluation**        | Score of employee's last performance review [0–1]           |
| **number_project**         | Number of projects the employee contributes to              |
| **average_monthly_hours** | Average number of hours the employee worked per month       |
| **time_spend_company**     | How long the employee has been with the company (in years)  |
| **work_accident**          | Whether or not the employee experienced a work accident     |
| **left**                   | Whether the employee left the company (target variable)     |
| **promotion_last_5years**  | Whether the employee was promoted in the last 5 years       |
| **department**             | The employee's department                                   |
| **salary**                 | The employee's salary (in USD)                              |

---

## **3. PACE Stages**

This project followed the **PACE** methodology to ensure a structured approach to the analysis:

- **P - Plan**: 
   - Defined the business problem (employee turnover) and set clear goals (predict turnover and identify contributing factors).
   - Selected the dataset to work with and understood the features and their relevance.

- **A - Analyze**: 
   - Explored the data using **Exploratory Data Analysis (EDA)** techniques.
   - Cleaned the dataset (handling missing values, encoding categorical variables, etc.).
   - Conducted feature analysis to identify which factors were most associated with employee turnover.

- **C - Create**: 
   - Built various **machine learning models**, including **Logistic Regression**, **Random Forest**, and **XGBoost**.
   - Evaluated model performance and compared results based on key metrics (accuracy, precision, recall, etc.).

- **E - Evaluate**: 
   - Assessed model performance using evaluation metrics such as **AUC-ROC**, **F1-score**, and **accuracy**.
   - Analyzed the importance of each feature in predicting employee turnover.

For detailed steps and code, refer to the [**Jupyter Notebook**](Salifort_Motors_Study_Case.ipynb).

---

## **4. Result**

### **Executive Summary**
The project involved predicting employee turnover at Salifort Motors using multiple machine learning models. The key findings are summarized below:

### **Summary of Model Results**
- **Logistic Regression:**
  - Precision: 80%
  - Recall: 83%
  - F1-Score: 80%
  - Accuracy: 83%
  - AUC Score: 89%

- **Tree-based Models (Random Forest and XGBoost):**
  - **Random Forest:**
    - Precision: 99%
    - Recall: 90%
    - F1-Score: 94%
    - Accuracy: 98%
    - AUC Score: 98%
  - **XGBoost:**
    - Precision: 98%
    - Recall: 89%
    - F1-Score: 94%
    - Accuracy: 98%
    - AUC Score: 98%

### **Feature Importance**
- **Important Features (All Models):**
  - **Satisfaction Level**
  - **Number of Projects**
  - **Tenure**
  - **Average Monthly Hours**
  - **Last Evaluation**

These features were found to have the most significant influence on whether an employee would leave Salifort Motors.

---

## **5. Dataset**

The **HR_capstone_dataset** used for the analysis contains various employee attributes that were critical for building the predictive models. This dataset was sourced from Kaggle and contains detailed records for each employee, including job satisfaction, work hours, and turnover status.

---

## **6. Tools Used**

The following tools and libraries were used for this project:
- **Python**: The primary programming language for data analysis and machine learning.
- **pandas**: For data manipulation and exploration.
- **matplotlib** & **seaborn**: For data visualization.
- **scikit-learn**: For building machine learning models and model evaluation.
- **xgboost**: For implementing the XGBoost model.
- **Jupyter Notebook**: For running the analysis, documenting steps, and presenting results.

---

## **7. Model Evaluation**

### **Logistic Regression:**
This model was useful for understanding the relationship between employee features and turnover. It achieved decent performance but was outperformed by tree-based models.

### **Random Forest & XGBoost:**
Both models demonstrated superior performance. **Random Forest** and **XGBoost** achieved nearly identical results, with high accuracy and AUC scores, making them highly effective for predicting employee turnover. These models provided important insights into feature importance, helping identify the key variables influencing turnover.

---

## **8. Insights and Recommendations**

Based on the analysis and model results, the following insights and recommendations were derived:

### **Key Insights:**
- **Satisfaction Level** is the most important predictor of employee turnover. Employees with lower satisfaction levels are more likely to leave.
- **Workload**: Employees who work longer hours or handle more projects are more likely to leave. A significant factor in turnover is overwork.
- **Tenure**: Employees with shorter tenure are more likely to leave. Employee retention strategies should focus on newer employees.
- **Performance Evaluations**: Employees with poor performance evaluations may be at risk of leaving.

### **Recommendations:**
- **Reduce Workload**: Cap the number of projects an employee can work on to avoid burnout.
- **Enhance Job Satisfaction**: Implement employee engagement programs to improve job satisfaction.
- **Recognition and Promotion**: Ensure employees are recognized for their contributions, and promotions are based on performance, not just workload.
- **Monitor Satisfaction Levels**: Regularly assess employee satisfaction to identify potential retention risks early.

---

## **9. Conclusion**

This project successfully demonstrated the ability to predict employee turnover using machine learning models. By focusing on key features such as **satisfaction level**, **number of projects**, **work hours**, and **tenure**, Salifort Motors can proactively reduce turnover by implementing targeted retention strategies. The findings and model results provide valuable insights that can help Salifort improve its employee retention rates, reduce recruitment costs, and create a more positive work environment.

---

## **10. Files in this Repository**

- **HR_capstone_dataset**: The dataset used for analysis.
- **Salifort Motors Study Case.ipynb**: The Jupyter notebook containing detailed steps of data analysis, model building, and evaluation.
- **PACE_stage_image.png**: A visual representation of the **PACE** stages used in the project.
- **Employee Turnover Prediction Report**: The final report summarizing the analysis, results, and recommendations.

---

