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
Machine Learning Model 1:  Split the data into training and testing datasets by using `train_test_split`. Followed up with fitting and predicting a linear regression model and scoring the accuracy of the actual and predicted outcomes using a balanced accuracy score, classification report, and a confusion matrix.

- 
