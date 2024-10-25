# Fraud-Detection 
The dataset used for this project consists of credit card transactions, with features representing various attributes of the transactions and a binary target variable indicating whether the transaction is fraudulent (1) or valid (0). The dataset contains 247,578 transactions, characterized by 30 features along with the target variable.


The dataset was examined for any missing values or inconsistencies. It was determined that the target variable contained no NaN values, ensuring the integrity of the data used for model training. The dataset was split into feature variables (X) and the target variable (Y). This allowed for a clear distinction between input features and the output label for the classification task. The dataset was divided into training and testing sets using an 80-20 split. The training set was used to build the model, while the testing set was reserved for evaluating its performance. The Random Forest Classifier was selected for this project due to its robustness and effectiveness in handling classification problems, especially with imbalanced datasets. The model was trained on the training set, which allowed it to learn the underlying patterns associated with fraudulent and valid transactions.

Results: After training the model, predictions were made on the test set, and various performance metrics were computed:
•	Accuracy: 99.95% - The model achieved an accuracy of 99.95%, indicating that it correctly classified nearly all transactions in the test set.
•	Precision: 100% -  The precision of 100% signifies that every transaction flagged as fraudulent by the model was indeed fraudulent, meaning there were no false positives.
•	Recall: 78.46% - The recall of 78.46% indicates that the model was able to identify approximately 78.46% of actual fraudulent transactions, suggesting room for improvement in capturing more fraudulent cases.
•	F1-Score: 87.93% - The F1-score of 87.93% balances precision and recall, providing a single metric to assess the model’s performance.

The confusion matrix provides a detailed view of the model’s classification results:
•	True Negatives (TN): 26,096 (correctly identified valid transactions)
•	False Positives (FP): 0 (incorrectly flagged valid transactions as fraudulent)
•	False Negatives (FN): 14 (missed fraudulent transactions)
•	True Positives (TP): 51 (correctly identified fraudulent transactions)

The Random Forest model demonstrated exceptional performance in classifying transactions. The high accuracy and precision values indicate that the model is effective in reducing false alarms while maintaining a high level of correct identifications for valid transactions.
