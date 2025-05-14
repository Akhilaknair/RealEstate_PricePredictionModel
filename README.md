# 🏡 Real Estate Price Predictor – Machine Learning Project

This project uses machine learning to predict house prices based on the **Boston Housing dataset**. It demonstrates a complete ML pipeline, including data preprocessing, feature engineering, model training, evaluation, and deployment using **Python** and **Scikit-learn**.

---

## 📊 Project Workflow

### 1️⃣ Data Exploration 🔍
- Used **pandas** and **matplotlib** for initial data exploration and visualization.
- Gained insights into the features and their relationships with the target variable (MEDV - Median Value of Houses).

### 2️⃣ Train-Test Split ✂️
- Applied both a **custom train-test split** and **StratifiedShuffleSplit** to ensure proper class distribution of **CHAS** (Charles River dummy variable) in both sets.

### 3️⃣ Correlation Analysis 📊
- Computed the **correlation matrix** using `.corr()`.
- Identified key features:
  - **Positively correlated**: RM, B, ZN
  - **Negatively correlated**: LSTAT, PTRATIO, INDUS

### 4️⃣ Feature Engineering 🛠️
- Created a new derived feature: `TAXRM = TAX / RM` to capture interaction between taxation and average number of rooms in a house.

### 5️⃣ Data Preprocessing ⚙️
- Handled missing values using **SimpleImputer** (strategy: **median**).
- Scaled features with **StandardScaler**.
- Built a **data pipeline** using **Pipeline** to ensure clean and efficient preprocessing.

### 6️⃣ Model Training 🧠
- Tried multiple models, including:
  - **Linear Regression**
  - **Decision Tree Regressor** (Selected for final deployment)

### 7️⃣ Model Evaluation 📈
- Measured model performance using:
  - **RMSE** (Root Mean Squared Error)
  - **cross_val_score** with **10-fold cross-validation** to validate the model's generalizability.

### 8️⃣ Model Deployment 🚀
- The final model was **saved** using **joblib**.
- Successfully **loaded and tested** the model with a sample input using the `.predict()` method.

---

## 🛠 Tech Stack

- **Programming Language**: Python
- **Libraries**:
  - **pandas**: For data manipulation
  - **numpy**: For numerical operations
  - **matplotlib**: For data visualization
  - **scikit-learn**: For machine learning and model evaluation
  - **joblib**: For model deployment and saving/loading

---

## 📈 Performance

The trained **Decision Tree Regressor** achieved a satisfactory performance in predicting house prices. Evaluations based on **RMSE** and **cross-validation** demonstrated its effectiveness.

---

## 🚀 Model Deployment

Once the model was trained and evaluated, it was saved using **joblib** and successfully loaded for real-world use. You can use the model to predict house prices based on various features such as the number of rooms, crime rate, and other housing characteristics.

---

## 🤖 Conclusion

This project demonstrates the end-to-end process of building a real estate price predictor, from data exploration to model deployment, using **Python** and **Scikit-learn**.


Made with love and utmost determination by **Akhila** 👩‍💻 🔥


