Task 03 – Decision Tree Classifier (Bank Marketing Dataset)


📌 Objective

Build a Decision Tree Classifier to predict whether a customer will subscribe to a term deposit based on demographic and behavioral data from the UCI Bank Marketing Dataset.



📊 Dataset Used

Dataset: bank.csv (converted from the UCI Bank Marketing dataset)

Total rows: ~4500

Features include:

age, job, marital, education,

default, housing, loan,

contact, month, duration,

campaign, pdays, previous,

poutcome, emp.var.rate,

euribor3m, nr.employed, etc.

Target variable: y (whether the client subscribed)

"yes" → customer subscribed

"no" → customer did not subscribe



🧹 Steps Performed

1️⃣ Data Loading & Cleaning

Loaded CSV file

Converted categorical values using Label Encoding

Handled missing values

Scaled numerical features where needed



2️⃣ Model Building

Split data into train/test

Used DecisionTreeClassifier from Scikit-learn

Tuned basic parameters for performance



3️⃣ Model Evaluation

Two key evaluation visuals were generated:


📌 Feature Importance Plot

Shows which features influence the prediction the most.

duration was the most important factor

Followed by nr.employed, age, euribor3m, etc.

(📎 feature_importances.png included in repository)


📌 Confusion Matrix

Displays performance on the test set:

(📎 confusion_matrix.png included in repository)

Metrics interpreted:

Strong accuracy in predicting non-subscription

Model correctly identifies a smaller portion of actual subscribers



📁 Files in This Folder
Task3_DecisionTree_BankMarketing.ipynb
bank.csv
feature_importances.png
confusion_matrix.png
README.md


🚀 Conclusion

This Decision Tree model provides useful insights into customer behavior:

Call duration heavily influences subscription outcome

Macro-economic features like euribor3m and nr.employed are important

The model performs reasonably well but could be improved with

Ensemble methods (Random Forest, XGBoost)

Hyperparameter tuning

Feature engineering


👨‍💻 Author

Sethuraman Shanmugasundaram
PRODIGY InfoTech – Data Science Internship (Task 03)
