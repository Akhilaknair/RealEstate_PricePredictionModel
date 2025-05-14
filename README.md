
This project uses machine learning to predict house prices based on the Boston Housing dataset.
It demonstrates a complete ML pipeline, including data preprocessing, feature engineering, model training, evaluation, and deployment using Python and Scikit-Learn.


🏡 Real Estate Price Predictor – Project Workflow
1️⃣ Data Exploration 🔍
Used pandas and matplotlib for initial data exploration and visualization.


2️⃣ Train-Test Split ✂️
Applied both a custom train-test split and StratifiedShuffleSplit to ensure proper class distribution of CHAS in both sets.

3️⃣ Correlation Analysis 📊
Computed correlation matrix with .corr()

Identified key features positively (RM, B, ZN) and negatively (LSTAT, PTRATIO, INDUS) correlated with MEDV.

4️⃣ Feature Engineering 🛠️
Created a new derived feature:
TAXRM = TAX / RM
to capture interaction between taxation and average number of rooms.

5️⃣ Data Preprocessing ⚙️
Handled missing values using SimpleImputer (strategy: median).

Scaled features with StandardScaler.Built a data pipeline using Pipeline for clean and efficient preprocessing.

6️⃣ Model Training 🧠
Tried multiple models:
✅ Linear Regression
✅ Decision Tree Regressor (Selected for final deployment)

7️⃣ Model Evaluation 📈
Measured model performance using:
📉 RMSE (Root Mean Squared Error)
🔁 cross_val_score with 10-fold cross-validation


8️⃣ Model Deployment 🚀
Model saved using joblib

Successfully loaded and tested with a sample input using .predict() method ✅

🛠 Tech Stack
Language: Python

Libraries: pandas, numpy, matplotlib, scikit-learn, joblib

Made using Python and Scikit-Learn and utmost determination ! 🔥
~ Akhila 👩‍💻




