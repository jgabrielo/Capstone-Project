# Capstone-Project
## MANAOG, Beanca A. & SALES, Julian Gabrielo B.


### Youtube Presentation Link: https://youtu.be/GX91Ev69_Yk

A student performance project analyzing lifestyle habits and academic outcomes using machine learning.

This programming project investigates how students’ day-to-day behaviors—like studying, sleeping, screen usage, and health practices—are linked to their final exam scores. With 1,000 simulated student records, we dive into data exploration, clustering, and predictive modeling to understand and forecast academic performance.



## Project Goals:
* Analyze relationships between lifestyle choices and final exam results

* Group students by common lifestyle traits using clustering

* Predict exam performance using regression models

* Optionally, classify students by performance level

* Derive actionable insights to support student success strategies


## Dataset:
Name: student_habits_performance.csv

Source: Kaggle

The dataset includes the following information:

* Lifestyle metrics (e.g., study_hours_per_day, sleep_hours, screen time, health indicators)

* Final exam score (target variable)

* Engineered features like health_score and engagement_score

## Methods and Workflow
### 1. Data Preprocessing
* Cleaned and encoded categorical data

* Standardized numeric values

* Created features to summarize health and engagement levels

### 2. Exploratory Data Analysis (EDA)
* Used visualizations like histograms and scatter plots to uncover trends

* Analyzed correlations to identify influential predictors

### 3. Clustering
* Ran K-Means clustering on scaled features

* Chose optimal cluster count using Elbow and Silhouette methods

* Labeled student groups based on shared behaviors

### 4. Regression Models
To predict the final exam score:

| Model                   | MAE (CV) | RMSE (CV) | R² (CV) |
| ----------------------- | -------- | --------- | ------- |
| Linear Regression       | 4.28     | 5.39      | 0.90    |
| Decision Tree Regressor | 6.68     | 8.57      | 0.74    |
| Random Forest Regressor | 4.69     | 5.90      | 0.88    |



### 5. Classification Models (Optional)
Converted exam scores into 3 performance levels:

* Low (bottom 33%)

* Average (middle 34%)

* High (top 33%)

| Model               | Accuracy (CV) | F1 Score (CV) |
| ------------------- | ------------- | ------------- |
| Logistic Regression | 0.82          | 0.82          |
| Decision Tree       | 0.72          | 0.72          |
| Random Forest       | 0.77          | 0.77          |


Logistic Regression gave the best classification results.

## Insights and Interpretations
### A. Top Predictors
Important factors influencing scores included:

* Hours studied

* Health and engagement scores

* Sleep time

* Screen time

* Attendance rate

This means that sleep time, screen time, hours studied, and health & engagement scores affected the students' performance

## B. Cluster Profiling
* Cluster 0: Low wellness, disengaged, underperformers

* Cluster 1: Balanced habits, mid-range scores

* Cluster 2: High study and health levels, top scorers

Patterns revealed that students who spent more time on screens tended to score lower, whereas those who got more sleep and dedicated more time to studying generally performed better.

## C. Model Performance

Linear regression models showed the best balance of accuracy and interpretability. Tree-based models offered competitive results but were more complex to explain.

## D. Real-World Implications

Students with healthier lifestyles and stronger academic habits generally scored better. A balanced mix of study time, rest, and limited screen exposure contributed to higher performance, underscoring the value of overall well-being.

## Conclusion

This project offered a closer look at how everyday habits can influence academic performance. By analyzing the data, we saw clear connections—students who kept a balanced routine with enough sleep and steady study hours generally did better on their exams. While more advanced models like Random Forest gave solid predictions, the transparency of linear regression made it a practical choice. Overall, the results highlight the real impact of lifestyle choices on learning, and they serve as a reminder that small daily habits can add up to big differences in outcomes.

## Repository Contents
* FINAL_PROJECT_TEECE_2.ipynb: Full notebook with code and commentary

* student_habits_performance.csv: Dataset used

* README.md: Project overview

* /Visuals: Contains saved plots and figures

