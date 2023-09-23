# credit-risk-classification
Evaluating borrower creditworthiness by examining historical borrowing behavior within a peer-to-peer lending service company.

Discovery:
- For this project, I followed a step-by-step approach to analyze data. First, I identified the main question: how to tell if someone is likely to pay back a loan or not. 

Data Preparation:
- Next, I prepared the data. Initially, I examined the provided data source and utilized Jupyter Notebook to visualize the data, inspecting its columns and rows. This allowed me to determine if the data was sufficiently cleaned and organized for comprehensible analysis. 

- The dataset at hand appeared to consist of loans extended to various individuals, encompassing diverse loan amounts, interest rates, and financial information related to the borrowers. Notably, the last column contained a crucial variable, "Loan status," where a value of 0 indicated a healthy loan, while a value of 1 signified a high risk of default.

Model Planning:
- The third step entailed devising a strategy for employing machine learning models that could accurately predict loan status (0 or 1) based on the given features or variables influencing the likelihood of either outcome. In this specific project, we opted to employ logistic regression models. These models effectively transformed the continuous data into percentage-based probabilities for successful binary outcomes.

Model Building:
- Machine Learning Model 1:
  - Split the data into training and testing datasets by using `train_test_split`. Followed up with fitting and predicting a linear regression model and scoring the accuracy of the actual and predicted outcomes using a balanced accuracy score, classification report, and a confusion matrix.
    1. Precision -  When the model predicts a loan as healthy (class 0), it's correct 100% of the time. When the model predicts a loan as risky (class 1), it's correct 87% of the time.
    2. Recall - Out of all the actual healthy loans (class 0), the model correctly identifies 100% of them. Out of all the actual risky loans (class 1), the model correctly identifies 89% of them.
    3. Accuracy - Overall, the model is correct 99% of the time in making predictions for all classes combined.

-  Machine Learning Model 2:
  -  Created a similar model to the first except this time used the RandomOverSampler module form imbalanced-learn to resample my imbalanced data.
     1. Precision - When the model predicts class 0, it's correct 99% of the time. When the model predicts class 1, it's correct 99% of the time.
     2. Recall - Out of all actual class 0 instances, the model correctly identifies 99% of them. Out of all actual class 1 instances, the model correctly identifies 99% of them.
     3. Accuracy - Overall, the model is correct 99% of the time in making predictions for all classes combined.

Outcomes: 
- Both models exhibit strong performance with an overall accuracy of approximately 99%. Model 1 demonstrates exceptional precision and recall for class 0, indicating high correctness and coverage in identifying healthy loans. However, it slightly lags in precision and recall for class 1 (risky loans) compared to Model 2.

- In contrast, Model 2 delivers equally impressive precision, recall, and F1-scores for both class 0 and class 1, indicating a well-balanced predictive capability across both categories.

Final summary:
- In summary, while Model 1 excels in predicting healthy loans, Model 2 maintains a high level of performance across both healthy and risky loan predictions. The choice between the two models may depend on the specific application and the importance of precision and recall in either class.
