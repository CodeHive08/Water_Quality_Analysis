# Water_Quality_Analysis

This project aims to predict the **potability of water** using machine learning algorithms based on various water quality parameters.

---

## 📂 Dataset

The dataset used in this project is `water_potability.csv`.The link to the dataset is:https://www.kaggle.com/datasets/adityakadiwal/water-potability  
It includes the following water quality metrics:

- pH
- Hardness
- Solids
- Chloramines
- Sulfate
- Conductivity
- Organic Carbon
- Trihalomethanes
- Turbidity
- **Potability** (Target Variable: 0 = Not Potable, 1 = Potable)

---

## 📌 Project Overview

The project follows a structured machine learning pipeline:

1. **Data Loading and Exploration**  
   Load the dataset and inspect its structure, size, and initial statistics.

2. **Data Preprocessing**  
   Handle missing values (notably in `ph`, `Sulfate`, and `Trihalomethanes`) using imputation strategies based on the `Potability` class.

3. **Exploratory Data Analysis (EDA)**  
   Visualize data distributions, correlations, and missing value patterns to gain insights.

4. **Feature Selection and Target Variable**  
   Define independent features (X) and the dependent target variable (y).

5. **Data Splitting**  
   Split the dataset into training and testing sets (e.g., 80-20 split).

6. **Feature Scaling**  
   Normalize the features using `StandardScaler` to bring them to a common scale.

7. **Model Training**  
   Train a **Random Forest Classifier** on the training data.

8. **Hyperparameter Tuning**  
   Use `RandomizedSearchCV` to optimize the performance of the Random Forest model.

9. **Model Evaluation**  
   Evaluate model performance using:
   - Accuracy Score
   - Confusion Matrix
   - Classification Report

10. **Prediction on Sample Input**  
    Demonstrate model prediction for new, unseen data.

11. **XGBoost Classifier**  
    Train and evaluate an **XGBoost Classifier** to compare results with the Random Forest.

---

## 🧰 Requirements

Install the required Python libraries:

```bash
pip install pandas numpy matplotlib seaborn scipy scikit-learn plotly xgboost
```
### ▶️ Usage
Clone the repository or download the project files.

Open the Jupyter Notebook or Google Colab file.

Run each code cell sequentially to execute all steps:

Data loading

Preprocessing

Model training

Evaluation

### 📊 Results
The notebook will output:

Descriptive statistics and summary of the dataset

Visualizations: distribution plots, heatmaps, correlation matrices
![download](https://github.com/user-attachments/assets/df13d955-0329-4b86-a4e5-d2455ecb3d14)

Trained model performance:

Confusion Matrix:


![download](https://github.com/user-attachments/assets/c2f75f3c-6a99-4221-89e9-5dea5ccb0ee7)
![download](https://github.com/user-attachments/assets/651f496f-d353-4f5c-a6ff-b1ab04312efa)

Predictions on a sample water quality input
![image](https://github.com/user-attachments/assets/896565e0-04a0-41c8-b215-37ac036b686d)

### 👤 Author
Sandeep Singh Mehta
### 📎 License
This project is licensed under the MIT License - see the LICENSE file for details.

