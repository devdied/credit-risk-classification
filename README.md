# credit-risk-classification
**Overview:**

The purpose of this credit risk analysis is to develop a machine learning model that accurately predicts the creditworthiness of borrowers using a dataset of historical lending activity from a peer-to-peer lending services company. The goal is to create a model that can effectively differentiate between "healthy loans" (low risk) and "high-risk loans" based on various features in the dataset.

The model was trained on loan size, interest rate, borrower income, debt to income, number of bank accounts, derogatory marks, total debt, and loan status to predict if the loan is low/high risk.

The distribution of loan status in the dataset-
* low risk loan -    75036
* high risk loan -     2500

**Classification Report - Linear Regression Model:**

- **Accuracy:** The initial machine learning model achieves a high accuracy score of 99%, indicating that it correctly classifies nearly all instances in the dataset.

- **Precision:** For "healthy loans," precision is 100%, meaning that all instances predicted as "healthy loans" are indeed "healthy loans." For "high-risk loans," precision is 87%, indicating that 87% of the instances predicted as "high-risk loans" are genuinely "high-risk loans."

- **Recall:** For "healthy loans," recall is 100%, signifying that the model correctly identifies all actual "healthy loans." For "high-risk loans," recall is 89%, showing that 89% of the actual "high-risk loans" are correctly predicted.

**Classification Report - Linear Regression with Random Oversampling:**

- **Accuracy:** The linear regression model with random oversampling achieves an even higher accuracy score of 100%, indicating that it accurately classifies all instances in the dataset.

- **Precision:** For "healthy loans," precision remains at 100%, meaning that all instances predicted as "healthy loans" are indeed "healthy loans." For "high-risk loans," precision improves to 87%, indicating that 87% of the instances predicted as "high-risk loans" are genuinely "high-risk loans."

- **Recall:** For "healthy loans," recall remains at 100%, signifying that the model correctly identifies all actual "healthy loans." For "high-risk loans," recall increases to 100%, showing that all actual "high-risk loans" are correctly predicted.

**Summary and Recommendation:**

The machine learning model, initially and with linear regression and random oversampling, demonstrates remarkable performance in terms of accuracy, precision, and recall. It effectively distinguishes between "healthy loans" and "high-risk loans" with high precision, minimizing false positives. Moreover, it maintains high recall, minimizing false negatives.

**Recommendation:** Based on the outstanding performance metrics achieved, I would recommend using the linear regression model with random oversampling for credit risk assessment. This model can reliably identify creditworthy borrowers while effectively flagging high-risk applicants. It strikes an excellent balance between precision and recall, making it suitable for practical use by the lending company.

This model can significantly assist the company in making informed lending decisions, reducing the risk of default, and ultimately improving its lending portfolio's performance. However, it's essential to ensure that this model is evaluated on unseen data to assess its generalization performance. Make sure that the model is not overfitting and avoid data leakage. Additionally, continuous monitoring and periodic model retraining are advisable to adapt to evolving lending patterns and risks.
