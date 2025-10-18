**Student Dropout Summative Assignment**

*Overview*

This project aims to analyze and predict student dropout likelihood based on academic performance, demographic, and behavioral factors. Using data preprocessing, feature correlation analysis, and classification modeling, the notebook explores patterns that influence student retention and identifies strategies for early intervention.


*Repository Structure*


student_dropout_summative_assignment/
│
├── student_dropout.ipynb       # Main notebook containing data preprocessing, EDA, and modeling
├── data/                       # Dataset files (if applicable)
├── images/                     # Visualization outputs (e.g., correlation heatmap, ROC curve)
└── README.md                   # Project documentation


*Project Objectives*

Identify factors most correlated with student dropout.

Build a predictive model to classify dropout vs. non-dropout cases.

Evaluate model performance using metrics like precision, recall, F1-score, and AUC.

Determine the optimal probability threshold for intervention.


*Key Findings*

1. Correlation Analysis

The correlation heatmap provides insights into the relationships between student dropout and various attributes.

Strong negative correlations were found between dropout and academic performance indicators such as:

Final_Grade (-0.66)

Grade_2 (-0.59)

Grade_1 (-0.56)

Positive correlations with dropout were observed for:

Number_of_Failures (0.38)

School_MS (0.30)

These results suggest that low grades and repeated failures are strong predictors of dropout risk, highlighting the importance of academic support systems.

2. ROC and Threshold Analysis

The Receiver Operating Characteristic (ROC) curve demonstrates strong model performance with an AUC ≈ 0.91, indicating excellent discriminative capability between dropout and non-dropout students.

A threshold analysis identified the optimal probability cutoff that maximizes the F1-score by balancing recall and precision.
The model slightly favored recall over precision to minimize the chance of missing students at risk of dropping out — a more critical concern than a few false alarms.


*Tools & Libraries*

Python (3.x)

pandas, numpy – Data manipulation and preprocessing

matplotlib, seaborn – Visualization

scikit-learn – Model training and evaluation


*How to Run*

Clone the repository:

git clone https://github.com/Peace3B/student_dropout_summative_assignment.git

cd student_dropout_summative_assignment


Install required dependencies:

pip install -r requirements.txt


Open the notebook:

jupyter notebook student_dropout.ipynb


Run all cells to reproduce the analysis and results.


Results Summary

AUC: 0.91

Best threshold: Achieved optimal F1-score with recall emphasis

Key predictors: Final grades, previous failures, and study time

*Conclusion*

The study demonstrates that academic performance metrics, particularly grades and failure counts, are crucial indicators of student dropout risk. By prioritizing recall in the prediction model, educational institutions can proactively identify and support at-risk students, ultimately reducing dropout rates.


*Author: KEZA PEACE*
