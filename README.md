# 🚨 Fraud Detection

# 📌 Project Overview

This project develops a machine learning pipeline for detecting fraudulent credit card transactions using a highly imbalanced dataset.

The project was completed as part of my Data Analytics Internship with Oasis Infobyte and demonstrates an end-to-end workflow covering data exploration, preprocessing, class imbalance handling, model development, evaluation, and feature importance analysis.



# 🎯 Objectives
🔍 Explore and understand the transaction dataset
⚖️ Analyze the class imbalance between fraudulent and legitimate transactions
🧹 Prepare the data for machine learning
🔄 Apply SMOTE to address class imbalance
🤖 Train and compare classification models
📊 Evaluate model performance using appropriate metrics
🔎 Analyze feature importance
🏆 Identify the stronger-performing model


# 📊 Dataset

The dataset contains 284,807 credit card transactions with anonymized numerical features.

The target variable identifies whether a transaction is legitimate or fraudulent.

The dataset is highly imbalanced, with fraudulent transactions representing a very small proportion of the total transactions.

The features V1 to V28 are anonymized PCA-derived variables, while transaction amount and time-related information are also included.


# ⚙️ Machine Learning Workflow
The project followed these major steps:

📥 Data loading and exploration
⚖️ Class distribution analysis
💰 Transaction amount analysis
🕐 Transaction activity analysis by hour
📈 Fraud rate analysis by hour of day
🧹 Data preparation
🔀 Stratified train-test splitting
🔄 Class imbalance handling using SMOTE
🤖 Model training
📏 Model evaluation
🔎 Feature importance analysis
⚖️ Model comparison


# 🤖 Models Used

Two classification algorithms were trained and evaluated:
📊 Logistic Regression
🌳 Random Forest Classifier

SMOTE was applied only to the training data to address class imbalance while preventing data leakage into the test set.

# 📈 Model Performance

📊 Logistic Regression
Accuracy: 98.95%
Precision: 13.06%
Recall: 89.80%
F1-score: 22.80%
AUC-ROC: 97.66%

🌳 Random Forest
Accuracy: 99.94%
Precision: 83.51%
Recall: 82.65%
F1-score: 83.08%
AUC-ROC: 96.36%


# 🏆 Model Comparison

Logistic Regression achieved a higher recall of 89.80%, meaning it identified a larger proportion of fraudulent transactions.

However, Random Forest achieved substantially higher precision and F1-score while maintaining a strong recall. It therefore provided a better overall balance between identifying fraudulent transactions and reducing false positives.

Based on the overall classification performance, Random Forest was the stronger-performing model for this project.


# 🔎 Feature Importance
Feature importance analysis was performed using Random Forest, while Logistic Regression coefficients were also examined.

The most important Random Forest features included:
V14
V10
V4
V12
V17
V11

V14 had the highest Random Forest feature importance at approximately 0.2165, followed by V10 at approximately 0.1591.

Because the V1–V28 variables are anonymized PCA-derived features, their individual real-world meanings cannot be directly interpreted from the dataset.


# 📏 Evaluation Metrics
Because fraud detection involves severe class imbalance, accuracy alone is not sufficient for evaluating model performance.

The project therefore considered:
✅ Accuracy
🎯 Precision
🔍 Recall
⚖️ F1-score
📈 AUC-ROC
📊 Confusion matrices
📋 Classification reports

These metrics provide a more meaningful assessment of fraud detection performance.

# 🛠️ Tools & Technologies
🐍 Python
🐼 Pandas
🔢 NumPy
🤖 Scikit-learn
⚖️ Imbalanced-learn
📊 Matplotlib
📈 Seaborn
📓 Jupyter Notebook


# 💡 Key Takeaways
⚠️ Fraud detection datasets can contain severe class imbalance, making appropriate evaluation essential.
🔄 SMOTE can help improve model learning when applied correctly to the training data.
📊 Accuracy should not be used as the only performance measure for fraud detection.
🎯 Logistic Regression achieved higher fraud recall.
🌳 Random Forest provided a stronger balance between precision and recall.
🏆 Random Forest achieved the highest overall F1-score and was selected as the stronger-performing model.


# 🚀 Scalability Considerations

The workflow can be extended to larger transaction datasets by optimizing data processing, using efficient feature engineering techniques, and applying scalable machine learning approaches.

For production environments, the model would also require continuous monitoring, periodic retraining, and evaluation against changing patterns of fraudulent activity.


# 📝 Conclusion

This project demonstrated an end-to-end machine learning approach to detecting fraudulent credit card transactions. The workflow included exploratory analysis, preprocessing, class imbalance handling with SMOTE, model development, evaluation, and feature importance analysis.

Although Logistic Regression achieved higher recall, Random Forest produced a substantially better balance between precision and recall and achieved the highest F1-score. Therefore, Random Forest was considered the stronger overall model for this fraud detection task.

The project also highlights the importance of selecting evaluation metrics that reflect the requirements of fraud detection rather than relying on accuracy alone.


# 🎓 Internship
Organization: Oasis Infobyte
Program: Data Analytics Internship
Hashtags: #OasisInfobyte #OIBSIP

# 👩🏽‍💻 Author
Adenike Adetuberu
